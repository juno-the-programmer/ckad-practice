
## ReplicaSets
### Explain replicaset definition
```
kubectl explain replicaset
```
### Create replicaset
```
kubectl create -f rc-definition.yaml
```

### List replicaset
```
kubectl get replicaset
```

### List replicaset (shortform)
```
kubectl get rs
```

### Delete replicaset
```
kubectl delete replicaset replicasetname
```

### Edit replicaset
```
kubectl edit replicaset replicasetname
```

### Replace replicaset
```
kubectl replace -f rc-definition.yaml
```

### Scale replicaset
```
kubectl scale replicaset replicasetname --replicas=5
```
