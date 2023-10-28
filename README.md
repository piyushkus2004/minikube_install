# minikube_install
# How to Install Minikube on Ubuntu ##
## Step 1: Update System and Install Required Packages

### Before installing any aplllication you need to update and upgrade your system ###
```
sudo apt-get update -y
```
```
sudo apt-get upgrade -y
```
### Also make sure to install (or check whether you already have) the following required packages: ###
```
sudo apt-get install curl
```
```
sudo apt-get install apt-transport-https
```
# Step 2: Install VirtualBox Hypervisor
**to install virtualbx on ubuntu run this commamd**
```
sudo apt install virtualbox virtualbox-ext-pack
```
# Step 3: Install Minikube #
### for latest minikube binary use wget command
```
wget https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
```
### copy downloaded file into /usr/local/bin/minikube directory 
```
sudo cp minikube-linux-amd64 /usr/local/bin/minikube
```
### give the file executive permission using the chmod command ###
```
sudo chmod 755 /usr/local/bin/minikube
```
### using this command verify minikube installed or not ###
```
minikube version
```
# Step 4: Install Kubectl #

```
curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl
```
```
chmod +x ./kubectl
```
```
sudo mv ./kubectl /usr/local/bin/kubectl
```
```
kubectl version -o json
```
# Step 5: Start Minikube #
```
minikube start
```
