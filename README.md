


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