**Replication Controller**

Replication controller helps us run multiple instances of a single pod in kubernetes cluster. 

For example, let's say a pod which is running on a node fails. replication controller helps to bring back the new pod

**Load balancing and scaling**

Replication controller spans across multiple nodes and pods and scales when the demand increases

**Replication controller and replicasets**
Replication controller and replicasets - both are having the same purpose but they are not same

Difference is **Selector**

replicaset can also manage pods that were not created as part of replicaset creation
for example: they were pods created before the creation of replicaset, it will add in replicaset if the selector label matches

Replicaset 


