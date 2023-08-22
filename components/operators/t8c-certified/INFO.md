# t8c-certified

### Realtime Decision Automation for Multicloud Applications
Turbonomic Workload Automation for Multicloud simultaneously optimizes performance, compliance, and cost in real-time. Workloads are precisely resourced, automatically, to perform while satisfying business constraints:
* Continuous placement of workload across multiple clouds both on-prem and public clouds providers.
* Continuous scaling for applications and the underlying infrastructure.

It assures application performance by giving workloads the resources they need when they need them.

### How do I start?

Turbonomic platform installation and configuration documentation can be found on the IBM Turbonomic documentation site here https://www.ibm.com/docs/en/tarm/latest?topic=installation-installing-kubernetes-clusters
Carefully read through the prerequisites before beginning the installation.  Once ready, on the `Details` tab for the Turbonomic Platform Operator, under `Provided APIs`, click `Create instance`.
For samples of common configurations, refer to sample custom resource YAMLs provided here: https://github.com/turbonomic/t8c-install/tree/master/samples
Looking to upgrade your current deployment? Refer to documentation here: https://www.ibm.com/docs/en/tarm/latest?topic=version-updating-using-red-hat-openshift-operatorhub

### How does it work?
Turbonomic uses a public APIs already exposed by application and infrastructure instrumentation to discover and monitor your environment.
Turbonomic determines the right actions that drive continuous health, including continuous placement and continuous scaling for applications and the underlying cluster.
Turbonomic leverages the built-on orchestration provided by the application and infrastructure deployment tools and automates the execution of these actions to continiously meet the respective service level objective of each application service.