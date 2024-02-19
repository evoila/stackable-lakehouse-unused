# stackable-lakehouse
This repository documents the deployment of a production-ready lakehouse on kubernetes via stackable.
The deployment is helm-based and all corresponding files are located in the [helm-deployment folder](helm-deployment).
A step-by-step-guide is located in the [guide folder](guide).

# Prerequisites
You need a k8s-cluster with the following resources:
- 10 nodes with 4 cores/8 threads, 20GB RAM and 30GB HDD, i.e. Standard\_D4\_v2 in Azure
- multiple persistent volumes, 1TB total
For a guide how to setup this in Azure/the evoila lab, see [here](guide/setup_k8s.md).

Helm is needed, to install it follow [these official instructions](https://helm.sh/docs/intro/install/).
You also need stackablectl, for the installation follow [this official guide](https://docs.stackable.tech/management/stable/stackablectl/installation).

The necessary operators and everything else is explained in the mentioned [guide folder](guide).

We try to document as much as possible, so that even users with minimal knowledge can deploy this lakehouse. However, we cannot explain every technology that is used in detail.

The following technologies are used and you can search for the corresponding documentation online:
- kubernetes
- stackable
- minIO
- Hive Metastore
- Trino
- Superset
- Spark
- Kafka
- NiFi
- OPA
- TLS/SSL
