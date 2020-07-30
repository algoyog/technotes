# Kubernetes

Kubernetes was first developed by a team at Google. It is based on their experience from running containers at scale for years. Later on, it was donated to Cloud Native Computing Foundation (CNCF). It is a true open source project with probably the highest velocity in history.

## Why Kubernetes? 
* Let’s discuss how Kubernetes is not only a container scheduler but a lot more.
* We can use it to deploy our services, to roll out new releases without downtime, and to scale (or de-scale) those services.
* It is portable.
* It can run on a public or private cloud.
* It can run on-premise or in a hybrid environment.
* We can move a Kubernetes cluster from one hosting vendor to another without changing (almost) any of the deployment and management processes.
* Kubernetes can be easily extended to serve nearly any needs. We can choose which modules we’ll use, and we can develop additional features ourselves and plug them in.
* Kubernetes will decide where to run something and how to maintain the state we specify.
* Kubernetes can place replicas of a service on the most appropriate server, restart them when needed, replicate them, and scale them.
* Self-healing is a feature included in its design from the start. On the other hand, self-adaptation is coming soon as well.
* Zero-downtime deployments, fault tolerance, high availability, scaling, scheduling, and self-healing add significant value in Kubernetes.
* We can use it to mount volumes for stateful applications.
* It allows us to store confidential information as secrets.
* We can use it to validate the health of our services.
* It can load balance requests and monitor resources.
* It provides service discovery and easy access to logs.

## Architecture

### System Architecture
![alt text][logo1]

[logo1]: components-of-kubernetes.png ""
#### Control Plane Components 
> The control plane's components make global decisions about the cluster (for example, scheduling), as well as detecting and responding to cluster events (for example, starting up a new pod when a deployment's replicas field is unsatisfied).
##### kube-apiserver 
> The API server is a component of the Kubernetes control plane that exposes the Kubernetes API. The API server is the front end for the Kubernetes control plane.
##### etcd
> Consistent and highly-available key value store used as Kubernetes' backing store for all cluster data.
##### kube-scheduler 
> Control plane component that watches for newly created Pods with no assigned node, and selects a node for them to run on.
##### kube-controller-manager 
> Control Plane component that runs controller processes.

> These controllers include:
> * Node controller: Responsible for noticing and responding when nodes go down.
> * Replication controller: Responsible for maintaining the correct number of pods for every replication controller object in the system.
> * Endpoints controller: Populates the Endpoints object (that is, joins Services & Pods).
> * Service Account & Token controllers: Create default accounts and API access tokens for new namespaces.

#### Node Components 
> Node components run on every node, maintaining running pods and providing the Kubernetes runtime environment.


##### kubelet 
> An agent that runs on each node in the cluster. It makes sure that containers are running in a Pod.

##### kube-proxy 
> kube-proxy is a network proxy that runs on each node in your cluster, implementing part of the Kubernetes **Service** concept.
> kube-proxy maintains network rules on nodes. These network rules allow network communication to your Pods from network sessions inside or outside of your cluster.

##### Container runtime 
> The container runtime is the software that is responsible for running containers.
> Kubernetes supports several container runtimes: Docker, containerd, CRI-O, and any implementation of the Kubernetes CRI (Container Runtime Interface).
 

### Developer Architecture

#### Runtime Architecture
![alt text][logo2]

[logo2]: devarch.png ""

##### POD
![alt text][logo3]

[logo3]: pod-seq.png ""

##### Replicaset
![alt text][logo4]    

[logo4]: repset-seq.png ""

##### Service
![alt text][logo5]    

[logo5]: ser-seq.png ""

![alt text][logo6]    

[logo6]: ser1-seq.png ""

![alt text][logo7]    

[logo7]: ser2-seq.png ""



##### Deployment
![alt text][logo4]    

[logo4]: repset-seq.png ""



##### The Table

|access|Desc|Object|
|------|------|-------|
|port|The port that will be exposed by this service.| Service|
|targetport|Number or name of the port to access on the pods targeted by the service. |Service|
|nodeport|The port on each node on which this service is exposed when type=NodePort or LoadBalancer. |Service 
|servicePort|Specifies the port of the referenced service.|Ingress

### Sysadmin Architecture


### Ref Implementation
> https://github.com/gearuprepo/reflab.git

## References
https://www.educative.io/courses/practical-guide-to-kubernetes<br>
https://kubernetes.io/docs/concepts/<br>
https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#serviceport-v1-core<br>