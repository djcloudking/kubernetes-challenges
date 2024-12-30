# kubernetes (K8s) Architecture explained in simple words


Kubernetes is composed of 2 parts:

1- Control plane

2- Data plane


###  Control plane


Control plane is configured in the Kubernetes master. It has:

- **API server** exposes your kubernetes to the external world.

- **Scheduler** schedules your pod on nodes from information received from API server. 

- **etc d** stores key value pairs..

- **Controller manager**: Kubernetes supports auto-scaling through containers such as replica set. 

- **Cloud Controller Manager (CCM)**: Kubernetes can be run on cloud platform such as EKS. 


###  Data plane


Data plane is configured in the Kubernetes worker. It has:

- **Kubelet** ensures that the pod is always running. 

- **Kube-proxy** provides networking IP tables.

- **Container runtime** runs your container.

Kubernetes uses these 3 components to run your applications. 