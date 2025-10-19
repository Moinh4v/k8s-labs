## Kubernetes Networking - 101

Networking 101

Single node has ip address called `192.168.1.2`

and pod internally has assigned ip address `10.244.0.0`

**Cluster networking**

Now we have multiple nodes having the same internal ip address for pods that will lead to ip conflicts..

Kubernetes expects us to meet certain requirements
- All containers/PODs can communicate to one another without NAT
- All nodes can communicate with all containers and vice-cersa without NAT