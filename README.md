# Kubernetes-Scheduling-Examples
This is a set of examples for advanced scheduling in kubernetes along with a walk-through guide.

## Getting Started
Below are the prerequisites 

### Prerequisites
If you don't have the kubernetes cluster ready, you can set it up using [kops](https://github.com/kubernetes/kops) or [kubeadm](https://kubernetes.io/docs/setup/independent/create-cluster-kubeadm/).

This tutorial, however, assumes that you have a working kubernetes multi-node cluster and kubectl is properly configured to access it.
To verify this, run the following command
```
kubectl get nodes
```
You should be able to see the list of nodes available in the cluster,
```
NAME                          STATUS    ROLES     AGE       VERSION
node1.compute.infracloud.io   Ready     <none>    25m       v1.9.4
node2.compute.infracloud.io   Ready     <none>    25m       v1.9.4
node3.compute.infracloud.io   Ready     <none>    28m       v1.9.4
```

### Kubernetes Scheduling
* [Taints and Tolerations](taints/README.md)
* [Node Affinity](nodeAffinity/README.md)
* [Pod Affinity](podAffinity/README.md)