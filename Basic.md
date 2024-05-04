# Kubernetes basics

### Kubernetes cluster
A Kubernetes cluster is a set of nodes that run containerized applications. 

To see your cluster info, type:
```bash
kubectl -- cluster-info
```

### Kubernetes node
A Node is a `worker machine` in Kubernetes and may be either a virtual or a physical machine, depending on the cluster. Each Node is managed by the control plane. A Node can have multiple pods, and the Kubernetes control plane automatically handles scheduling the pods across the Nodes in the cluster.

To see all of your nodes, type:
```bash
kubectl -- get nodes
```

### Kubernetes namespace
![Alt text](image.png)

Namespaces are a way to organize clusters into virtual sub-clusters. they can be helpful when different teams or projects share a Kubernetes cluster. Any number of namespaces are supported within a cluster, each logically separated from others but with the ability to communicate with each other.

To see all of your namespaces, type:
```bash
kubectl -- get namespaces
```

### Kubernetes service
A Kubernetes Service is an abstraction layer which defines a logical set of Pods and enables external `traffic exposure, load balancing and service discovery` for those Pods.

To see all of your services, type:
```bash
kubectl -- get services -A
```

### Kubernetes pods
A Kubernetes pod is a collection of one or more Linux® containers, and is the smallest unit of a Kubernetes application. Any given pod can be composed of multiple, tightly coupled containers (an advanced use case) or just a single container (a more common use case).

To see all of your pods, type:
```bash
kubectl -- get pods -A
```