# Kubernetes basics

### Kubernetes cluster
A Kubernetes cluster is a set of nodes that run containerized applications. 

To see your cluster info, type:
```bash
kubectl cluster-info
```

### Kubernetes node
A Node is a `worker machine` in Kubernetes and may be either a virtual or a physical machine, depending on the cluster. Each Node is managed by the control plane. A Node can have multiple pods, and the Kubernetes control plane automatically handles scheduling the pods across the Nodes in the cluster.

To see all of your nodes, type:
```bash
kubectl get nodes
```

### Kubernetes namespace
![Alt text](image.png)

Namespaces are a way to organize clusters into virtual sub-clusters. they can be helpful when different teams or projects share a Kubernetes cluster. Any number of namespaces are supported within a cluster, each logically separated from others but with the ability to communicate with each other.

To see all of your namespaces, type:
```bash
kubectl get namespaces
```