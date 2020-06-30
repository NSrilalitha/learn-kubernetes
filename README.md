# learn-kubernetes

Kubernetes is a container management tool. 

In kubernetes the application containers will be running inside a pod, which resides inside worker nodes. In kubernetes, every thing arranged in nodes. There will be atleast one
master node which manages worker nodes.

Few key concepts of kubernetes :
1. Pod
2. Deployment
3. Service (internal, external)
4. configMap
5. Secret

When you create a deployment, automatically pods will be assigned with application containers based on CPU utilization and memory. These pods will reside in worker nodes. A node
can contain n no of pods. A pod should contain one container per application. Inorder to access these pods, we need service. This is the only way to access the application which
is running inside a container and managed by kubernetes.

The way of accessing a spring boot application (spring boot + MySQL) which is managed by Kubernetes:

request in browser -> spring app external service -> spring app pod -> this communicates with mysql db internal service -> this will communicate with mysql pod (authenticate 
request with credentials avaiable in secret)

Refer below links :

https://www.youtube.com/watch?v=VnvRFRk_51k

YAML explanation: https://www.youtube.com/watch?v=qmDzcu5uY1I

Kubernetes components
--------------------
https://www.youtube.com/watch?v=Krpb44XR0bk&list=PLy7NrYWoggjwPggqtFsI_zMAwvG0SqYCb&index=15

kubectl commands
----------------
https://www.youtube.com/watch?v=azuwXALfyRg&list=PLy7NrYWoggjwPggqtFsI_zMAwvG0SqYCb&index=19

For installation refer below urls:
----------------------------------
(Here I am using Kubeadm to work on kubernetes - with kubeadm we can create cluster and join worker nodes with master and establish connection between
nodes)

https://phoenixnap.com/kb/install-kubernetes-on-ubuntu 

https://dzone.com/articles/developing-a-spring-boot-application-for-kubernete-1?fromrel=true

For pod network, I am using flannel. we can use Calico as well.

Deploy application to kubernetes cluster:
------------------------------------------

https://dzone.com/articles/developing-a-spring-boot-application-for-kubernete-4?fromrel=true

https://www.callicoder.com/deploy-spring-mysql-react-nginx-kubernetes-persistent-volume-secret/

https://spring.io/guides/gs/spring-boot-kubernetes/

https://docs.oracle.com/en/operating-systems/olcne/orchestration/kubectl-run.html



