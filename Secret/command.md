### Get secret
```
kubectl get secret
```
### Describe secret
```
kubectl describe secret default-token
```
### Create secret
```
kubectl create secret generic db-secret --from-literal=DB_Host=sql01 --from-literal DB_User=root --from-literal DB_Password=password123
```
### ENV
```
envFrom:
    - secretRef:
        name: db-secret
```