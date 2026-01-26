FROM amazoncorretto:17.0.18

ARG VERSION
ARG RELEASE

LABEL name="Flex for Apache Flink" \
      maintainer="support@factorhouse.io" \
      vendor="Factor House" \
      version=$VERSION \
      release=$RELEASE \
      summary="Flex is a toolkit for engineers who build, manage, and maintain systems powered by Apache Flink." \
      description="Flex features a rich data-oriented UI, specialized dashboards that deliver instant visibility into Flink Clusters, and developer tools that allow engineers to get to the heart of their systems quickly."

COPY resources/eula.txt /licenses/eula.txt
COPY target/flex-java17-standalone.jar /opt/factorhouse/lib/flex.jar
COPY resources/entrypoint.sh /usr/local/bin/flex.sh

RUN yum install shadow-utils -y

RUN mkdir -p /opt/factorhouse

RUN groupadd -g 1001 factorhouse && \
    useradd -r -u 1001 -g factorhouse factorhouse

RUN chown -R factorhouse:factorhouse /opt/factorhouse

RUN yum remove shadow-utils -y

USER factorhouse

ENV JVM_OPTS="-server -XX:MaxInlineLevel=15 -Djava.awt.headless=true -XX:InitialRAMPercentage=70 -XX:MaxRAMPercentage=70"

EXPOSE 3000

CMD ["/usr/local/bin/flex.sh"]
