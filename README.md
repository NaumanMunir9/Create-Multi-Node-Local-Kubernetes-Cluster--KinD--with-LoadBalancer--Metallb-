# Create Multi-Node Local Kubernetes Cluster (KinD) with LoadBalancer (Metallb)

## Create Kubernetes Cluster with KinD

[KinD Documentation](https://kind.sigs.k8s.io/)

- kind is a tool for running local Kubernetes clusters using Docker container “nodes”.
- kind was primarily designed for testing Kubernetes itself, but may be used for local development or CI.

#### KinD config to create multi-node cluster

```yaml
kind: Cluster
apiVersion: kind.x-k8s.io/v1alpha4
nodes:
- role: control-plane
- role: worker
- role: worker
```
