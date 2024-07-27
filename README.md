## Steps to Set Up the Cluster

1. **Create Cluster**
   
2. **Install Components**
   - Nginx Ingress Controller
   - Metrics Server
   - Monitoring Stack

3. **Add Registry for the Cluster**

```
kubectl create namespace repl
kubectl config set-context --current --namespace=repl
kubectl apply -f Deploy.yaml
kubectl apply -f Service.yaml
kubectl apply -f Ingress.yaml
kubectl apply -f NetworkPolicy.yaml
kubectl apply -f Autoscaler.yaml
```
