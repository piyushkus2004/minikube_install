# Managing Kubernetes with Minikube #
## Common Minikube Commands ## 
**To see the kubectl configuration use the command**
```
kubectl config view
```
**To show the cluster information**
```
kubectl cluster-info
```
**To check running nodes use the following command**
```
kubectl get nodes
```
**To see a list of all the Minikube pods run**
```
kubectl get pod
```
**To ssh into the Minikube VM**
```
minikube ssh
```
**To exit out of the shell run**
```
exit
```
**To stop running the single node cluster type**
```
minikube stop
```
**To check its status use**
```
minikube status
```
**To delete the single node cluster**
```
minikube delete
```
**To see a list of installed Minikube add-ons**
```
minikube addons list
```
# Access Minikube Dashboard #
```
minikube dashboard
```
**FOR ACCESSING DASHBOARD USING BROWSER USE THIS COMMAND**
```
minikube dashboard --url
```
