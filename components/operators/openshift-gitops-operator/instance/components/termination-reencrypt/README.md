# termination-reencrypt

## Purpose
This component is designed to enable reencrypt Termination on the ArgoCD route

## Usage

This component can be added to a base by adding the `components` section to your overlay `kustomization.yaml` file:

```
apiVersion: kustomize.config.k8s.io/v1beta1
kind: Kustomization

resources:
  - ../../base

components:
  - ../../components/termination-reencrypt
```