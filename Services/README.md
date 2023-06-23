**PERSISTENT VOLUME AND PERSISTENT VOLUME CLAIM**
 
PVs are volume plugins like Volumes, but have a lifecycle independent of any individual Pod that uses the PV. This API object captures the details of the implementation of the storage, be that NFS, iSCSI, or a cloud-provider-specific storage system. A PersistentVolumeClaim (PVC) is a request for storage by a user.

**NETWORK POLICIES**

Network policies are Kubernetes resources that control the traffic between pods and/or network endpoints. They uses labels to select pods and specify the traffic that is directed toward those pods using rules. Most CNI plugins support the implementation of network policies, however, if they don’t and we create a NetworkPolicy, then that resource will be ignored.

**STORAGE CLASS**

A Kubernetes StorageClass is a Kubernetes storage mechanism that lets you dynamically provision persistent volumes (PV) in a Kubernetes cluster. Kubernetes administrators define classes of storage, and then pods can dynamically request the specific type of storage they need.

# H1

