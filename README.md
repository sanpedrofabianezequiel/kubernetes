


```
minikube start
```
```
kubectl apply -f nginx-deployment.yaml
```
```
kubectl get pod -o wide
```
```
kubectl get service
```
```
Debug nginx-deployment-result.yaml
```
```
kubectl delete -f nginx-deployment.yaml
```
```
kubectl get deployment nginx-deployment -o yaml > nginx-deployment-result.yaml
```
```
kubectl get all
```
```
kubectl get secret
```
```
kubectl get pod --watch
```
```
kubectl describe pod mongodb-deployment-7bb6c6c4c7-r5mft 
```
```
kubectl get all || grep mongodb
```
```
kubectl get namespace
```
```
kubectl cluster-info
```
```
kubectl create namespace my-namespace
```
```
kubectl get configmap -n default
```
```
kubectl get configmap
```
```
kubectl get configmap -o wide
```
```
kubectl get configmap -o yaml
```
```
kubectl apply -f mysql-configmap.yaml --namespace=my-namespace
```
-------------------------
KUBENS
```
kubens
```
```
kubens my-namespace
```