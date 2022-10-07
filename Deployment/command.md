### Create deployment
```
kubectl create deployment webapp --image=kodekloud/webapp-color --replicas=3
```
### Create deployment with namespace
```
kubectl create deployment redis-deploy --image=redis --replicas=2 -n dev-ns
```
### Get deployment
```
kubectl get deployments
```
### Update deployment
```
kubectl apply -f deployment-definition.yml
```
```
kubectl set image deployment/myapp-deployment nginx=nginx:1.9.1
```
### Get status 
```
kubectl rollout status deployment/myapp-deployment
```
```
kubectl rollout history deployment/myapp-deployment
```
### Rollback
```
kubectl rollout undo deployment/myapp-deployment
```