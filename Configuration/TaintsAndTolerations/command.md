### Get Nodes
```
kubectl get nodes
```
### Create a taint
```
kubectl taint node node01 spray=mortein:NoSchedule
```
### Remove taint
```
kubectl taint node node01 taintname-
```