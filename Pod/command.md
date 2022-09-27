## Pods
### Create Pod (Imperative)
```
kubectl run redis --image=redis:alpine --labels=tier=db
```
### Create Pod
```
kubectl create -f file.yaml
```
### Edit Pod
```
kubectl edit pod redis
```
### Delete Pod
```
kubectl delete pod redis
```
### Extract pod definition in YAML format to a file
```
kubectl get pod redis -o yaml > file.yaml
```
### Replace
```
kubectl replace --force -f /tmp/kubect-edit-12346.yaml
```
### Getting into container
```
kubectl exec ubuntu-sleeper -- whoami
```