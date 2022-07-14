# Docker login
```
docker login
ls /root/.docker/config.json
```

# Create a Secret in K8s for Docker Registry
```
kubectl create secret generic regcred --from-file=.dockerconfigjson=/root/.docker/config.json --type=kubernetes.io/dockerconfigjson -n kube-system

kubectl get secrets -n kube-system 
```

# Apply the calico Config: 
```
kubectl apply -f calico.yaml
```

# Check the POD Status 
```
kubectl get pods -n kube-system
```
