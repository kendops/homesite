


### Verify that everything is working

Use: swilliamx/homesite:v1 image 

### deploy your website on kube cluster 

Run command 
```shell 
kubectl apply -k ./
kubectl get ns 
kubectl get pod -n homesite
kubectl get pv -n homesite
kubectl get pvc -n homesite
kubectl get deployments -n homesite
kubectl get ing -n homesite
kubectl get svc -n homesite
```

### Cleanup

Run command 
```shell 
kubectl delete -k ./      
kubectl get ns 
```

############################

```sh
### Deploy your first application on Kubernetes
kubectl apply -f namespace.yaml — create namespace 
kubectl apply -f deployment.yaml — create deployment 
kubectl apply -f service.yaml — create service
kubectl apply -f ingress.yaml — create ingress

Verify application health and behavior 
kubectl get deploy -n homesite — check deployment
kubectl get po -n homesite — create pod
kubectl get svc -n homesite — creates service 
kubectl get ing -n homesite — creates ingress
kubectl describe -n homesite — check app detail
```