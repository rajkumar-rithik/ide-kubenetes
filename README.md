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
kubectl apply -f deploy.yaml
kubectl apply -f service.yaml
kubectl apply -f ingress.yaml
kubectl apply -f network.yaml
kubectl apply -f autoscaler.yaml
```
