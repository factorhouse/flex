FROM dhi.io/amazoncorretto:25-alpine3.23

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
COPY target/flex-java25-standalone.jar /opt/factorhouse/lib/flex.jar

EXPOSE 3000

ENTRYPOINT ["java"]

CMD ["-server", \
     "-XX:MaxInlineLevel=15", \
     "-Djava.awt.headless=true", \
     "-XX:InitialRAMPercentage=70", \
     "-XX:MaxRAMPercentage=70", \
     "--sun-misc-unsafe-memory-access=allow", \
     "--enable-native-access=ALL-UNNAMED", \
     "-XX:+UseCompactObjectHeaders", \
     "-XX:+UseStringDeduplication", \
     "-jar", \
     "/opt/factorhouse/lib/flex.jar"]
