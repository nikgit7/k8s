**POD**

Pods are the fundamental building blocks of the Kubernetes system. They are used to deploy, scale, and manage containerized applications in a cluster.

**DEPLOYMENT**

A Deployment provides declarative updates for Pods and ReplicaSets.

We describe a desired state in a Deployment, and the Deployment Controller changes the actual state to the desired state at a controlled rate. You can define Deployments to create new ReplicaSets or to remove existing Deployments and adopt all their resources with new Deployments.

It's important to note that Deployment objects are used to manage stateless applications.

**Use cases:**

- Easy to deploy replica-sets and pods
- Easy to roll out to new deployments and roll back to previous deployments
- Scale deployments
- Pause and resume deployments
- Determine the status of deployments

**REPLICA-SET**

In Kubernetes, Deployments don't manage Pods directly. That's the job of the ReplicaSet object. When you create a Deployment in Kubernetes, a ReplicaSet is created automatically. The ReplicaSet ensures that the desired number of replicas (copies) are running at all times by creating or deleting Pods as needed.

**PERSISTENT VOLUME AND PERSISTENT VOLUME CLAIM**

PVs are volume plugins like Volumes, but have a lifecycle independent of any individual Pod that uses the PV. This API object captures the details of the implementation of the storage, be that NFS, iSCSI, or a cloud-provider-specific storage system. A PersistentVolumeClaim (PVC) is a request for storage by a user.

**NETWORK POLICIES**

Network policies are Kubernetes resources that control the traffic between pods and/or network endpoints. They uses labels to select pods and specify the traffic that is directed toward those pods using rules. Most CNI plugins support the implementation of network policies, however, if they don’t and we create a NetworkPolicy, then that resource will be ignored.


