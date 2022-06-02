


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
INGRESS
```
minikube addons enable ingress
```
Whe can check the last command with the next command
```
kubectl get pod -n kube-system
```
```
kubectl get ns
```
```
kubectl get all -n kubernetes-dashboard
```
```
kubectl get ingress
```
```
kubectl get ingress -n kubernetes-dashboard --watch
```
-------------------------
KUBENS
```
kubens
```
```
kubens my-namespace
```

-------------------------
### install hyperhit and minikube
`brew update`

`brew install hyperkit`

`brew install minikube`

`kubectl`

`minikube`

### create minikube cluster
`minikube start --vm-driver=hyperkit`

`kubectl get nodes`

`minikube status`

`kubectl version`

### delete cluster and restart in debug mode
`minikube delete`

`minikube start --vm-driver=hyperkit --v=7 --alsologtostderr`

`minikube status`

### kubectl commands
`kubectl get nodes`

`kubectl get pod`

`kubectl get services`

`kubectl create deployment nginx-depl --image=nginx`

`kubectl get deployment`

`kubectl get replicaset`

`kubectl edit deployment nginx-depl`

### debugging
`kubectl logs {pod-name}`

`kubectl exec -it {pod-name} -- bin/bash`

### create mongo deployment
`kubectl create deployment mongo-depl --image=mongo`

`kubectl logs mongo-depl-{pod-name}`

`kubectl describe pod mongo-depl-{pod-name}`

### delete deplyoment
`kubectl delete deployment mongo-depl`

`kubectl delete deployment nginx-depl`

### create or edit config file
`vim nginx-deployment.yaml`

`kubectl apply -f nginx-deployment.yaml`

`kubectl get pod`

`kubectl get deployment`

### delete with config
`kubectl delete -f nginx-deployment.yaml`

#Metrics

`kubectl top` The kubectl top command returns current CPU and memory usage for a cluster’s pods or nodes, or for a particular pod or node if specified.



