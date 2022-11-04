# kubernetes
All about Kubernetes from scratch

# I- MINIKUBE :-

MiniKube Installation

step 1 : 
Download Oracle Virtual Box : https://www.virtualbox.org/wiki/Downloads

Install and restart (*Restart is must*)

step 2 : 
Run the following commands to install and open Minikube in the Mac 
(Source : https://minikube.sigs.k8s.io/docs/start/ )

#minikube start
#minikube kubectl -- get po -A

step 3 :
Install Kubectl tool 
(Source : https://kubernetes.io/docs/tasks/tools/install-kubectl-macos/)
 
   #curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/darwin/amd64/kubectl"
   #curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/darwin/amd64/kubectl.sha256"
   #echo "$(cat kubectl.sha256)  kubectl" | shasum -a 256 --check
   #chmod +x ./kubectl
   #sudo mv ./kubectl /usr/local/bin/kubectl
   #sudo chown root: /usr/local/bin/kubectl
   
Step 4 : 
Verify 

#kubectl get po -A

#kubectl run web-server --image=nginx

#kubectl get pods

 Step 5 : 
 Sit back and enjoy K8 using Minikube.


# I- Multi node Cluster using "Kubeadm" tool :-

step 1 : Download Oracle virtual box (skip this if you already have it)
step 2 : Download centos:07 (http://isoredirect.centos.org/centos/7/isos/x86_64/CentOS-7-x86_64-DVD-2009.iso)
