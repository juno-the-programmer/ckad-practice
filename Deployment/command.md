### Create deployment
```
kubectl create deployment webapp --image=kodekloud/webapp-color --replicas=3
```
### Create deployment with namespace
```
kubectl create deployment redis-deploy --image=redis --replicas=2 -n dev-ns
```