### Create configmap
```
kubectl create -f config-map.yaml
```

### ENV
```
envFrom:
  - configMapRef:
        name: app-config
```
### SINGLE ENV
```
env:
  - name: APP_COLOR
    valueFrom:
        configMapKeyRef:
            name: app-config
            key: APP_COLOR
```
### VOLUME
```
volumes:
- name: app-config-volume
  configMap:
    name: app-config
```