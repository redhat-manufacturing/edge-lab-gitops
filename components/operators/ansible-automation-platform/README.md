# Ansible Automation Platform

Install Ansible Automation Platform.

Do not use the `base` directory directly, as you will need to patch the `channel` based on the version of OpenShift you are using, or the version of the operator you want to use.

The current *overlays* available are for the following channels:

* [stable-2.3](operator/overlays/stable-2.3)
* [stable-2.3-cluster-scoped](operator/overlays/stable-2.3-cluster-scoped)
* [stable-2.4](operator/overlays/stable-2.4)
* [stable-2.4-cluster-scoped](operator/overlays/stable-2.4-cluster-scoped)

## Usage

If you have cloned the `gitops-catalog` repository, you can install Ansible Automation Platform based on the overlay of your choice by running from the root (`gitops-catalog`) directory.

```
oc apply -k ansible-automation-platform-operator/operator/overlays/<channel>
```

Or, without cloning:

```
oc apply -k https://github.com/redhat-cop/gitops-catalog/ansible-automation-platform-operator/operator/overlays/<channel>
```

As part of a different overlay in your own GitOps repo:

```
apiVersion: kustomize.config.k8s.io/v1beta1
kind: Kustomization
resources:
  - https://github.com/redhat-cop/gitops-catalog/ansible-automation-platform-operator/operator/overlays/<channel>?ref=main
```
