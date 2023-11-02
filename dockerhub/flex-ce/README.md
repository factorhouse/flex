[![Release to DockerHub](https://github.com/factorhouse/flex/actions/workflows/release.yml/badge.svg?branch=main)](https://github.com/factorhouse/flex/actions/workflows/release.yml)

Dockerfile for the community edition of [Flex](https://factorhouse.io/flex) - Accelerate with Flex for [Apache Flink®](https://flink.apache.org/)

**Note**: This repository is for the [Enterprise Edition](https://factorhouse.io/flex/pricing) of Flex.

*  The Enterprise Edition DockerHub repository can be found at [factorhouse/flex-ee](https://hub.docker.com/r/factorhouse/flex-ee)
*  The Standard Edition DockerHub repository can be found at [factorhouse/flex-se](https://hub.docker.com/r/factorhouse/flex-se)

View [Features](https://factorhouse.io/flex/features) to compare editions.

# Quick reference

* **Maintained by**: [the Factor House team](https://factorhouse.io)
* **Where to get help**: [GitHub](https://github.com/factorhouse/flex), [Flex documentation](http://docs.factorhouse.io/flex-ce/), [Support Hub](https://factorhouse.io/support)

# Supported tags respective `Dockerfile` links

<!--- StartReleaseLinks --->

* [92.2, latest](https://github.com/factorhouse/flex/blob/main/dockerfile/flex-ce/Dockerfile)

<!--- EndReleaseLinks --->

# Quick reference (cont.)

* **Where to file issues:** https://github.com/factorhouse/flex/issues
* **Published image artifact details:** [GitHub actions CI](https://github.com/factorhouse/flex/actions/workflows/build.yml)
* **Image updates**: https://github.com/factorhouse/flex/tags
* **Source of this description**: [dockerhub/flex-ce/README.md](https://github.com/factorhouse/flex/blob/main/dockerhub/flex-ce/README.md)

# What is Flex?

### An Engineering Toolkit for Apache Flink®

Flex combines an intuitive UI with a secure, powerful API and world-beating performance.

Once installed, Flex gathers information about your Flink resources every minute, stores the results locally, then provides custom telemetry and insights to you in a rich data-oriented UI.

![Flex - Toolkit for Apache Flink](https://docs.factorhouse.io/img/assets/flex.png)

### Streamline and simplify Flink with the first enterprise-ready tooling solution

Once installed, Flex gathers information about your Flink resources every minute, stores the results locally, then provides custom telemetry and insights to you in a rich data-oriented UI.

* **Simplicity**: Streamline Flink Management for All User Groups
    - Simplify organizational management with Flex, catering to diverse user groups from Infrastructure to developers.
    - Seamlessly align your business needs with Flex's user-friendly interface and intuitive controls.

* **Intuitive**: Insights at Your Fingertips with Integrated Telemetry
    - Gain rich insights into your Flink clusters through fully integrated metrics and telemetry.
    - Access comprehensive long-term metrics and aggregated consumption and production data, from cluster-level insights to individual job-level details.

* **Secure**: Air-Tight Protection and Seamless Integration
    - Run air-gapped and secure environments confidently, thanks to Flex's support for Okta, OpenID, LDAP, SAML, Keycloak, and HTTPS.
    - Ensure data security with features like Audit Log, backed by prominent tools like Prometheus and Slack integration.

* **Powerful**: Unleash the full potential of Apache Flink with Flex
    - Leverage the power of Factor House's unifying core tech with fine-grained role-based access control.
    - Unlock advanced multi-tenancy capabilities to manage Flink resources effectively while maintaining control over visibility and usage.

### Built for the Enterprise

Flex comes from a practical application of Flink to real-world requirements and provides:

* **User Authentication** via DB, File, LDAP, SAML, or OpenID configuration.
* **User Authorization** with Simple or Role Based Access Controls (RBAC).
* **Data Policies** for masking and redaction of sensitive data like Credit Card or PII.
* **Data Governance** with all user actions captured in the Flex audit log.
* **Slack Integration** to have user actions sent to an operations channel as they happen.
* **HTTPS** easily configured with your own certificates, or integrated with a reverse-proxy.
* **Prometheus** endpoints to integrate with your preferred metrics and alerting systems.
* **Multi-Cluster Monitoring** from a single installation for cost efficiency and simplicity.
* **All data remains local** makes Flex perfect for air-gapped environments.

# Quick start + local evaluation

Start a [30-day free trial](https://factorhouse.io/flex/get-started) of Flex.

Visit https://docs.factorhouse.io/flex-ce/ for more documentation on getting started with Flex

# License

Flex is proprietary software. Flex's EULA can be found in the [GitHub repository](https://github.com/factorhouse/flex/blob/main/resources/eula.txt) or at https://factorhouse.io/flex/eula/

The Dockerfile's and [flex](https://github.com/factorhouse/flex) repository are licensed under the Eclipse Public License 1.0 (EPL-1.0)
