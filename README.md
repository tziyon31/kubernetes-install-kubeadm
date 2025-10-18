# kubernetes install kubeadm

In this repository I documented how I built my own Kubernetes cluster from scratch using kubeadm  
I wanted to understand every layer from the container runtime to the network plugin and not just run a pre made installer  

I followed the official Kubernetes documentation step by step and made sure to use consistent versions across all nodes v1.33  
I installed kubeadm kubelet and kubectl configured the container runtime prepared the networking layer and initialized the control plane  

All of the commands I used can be found in the official documentation

[Install kubeadm kubelet and kubectl](https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/install-kubeadm/)  
[Create a cluster with kubeadm](https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/create-cluster-kubeadm/)  
[Container runtimes](https://v1-31.docs.kubernetes.io/docs/setup/production-environment/container-runtimes/)  
[Network plugins](https://kubernetes.io/docs/concepts/extend-kubernetes/compute-storage-net/network-plugins/)  

I used these guides as references but adjusted details like the Pod CIDR interface names and runtime configuration to match my environment  
I also tested the process multiple times until everything worked smoothly including the networking setup with Flannel  

This repository includes the Flannel YAML I applied and the notes I kept during the setup process  
The goal was to create a minimal stable Kubernetes cluster that follows the official best practices but is also easy to reproduce later  

Tziyon Bublil  
DevOps and AI Infrastructure  
