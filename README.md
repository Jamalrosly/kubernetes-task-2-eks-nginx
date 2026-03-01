# Kubernetes Task-2: AWS EKS Nginx Deployment

## Task Description
Created an AWS EKS cluster using eksctl.
Deployed Nginx application on Kubernetes and exposed it outside the cluster using LoadBalancer service.

## Tech Stack Used
- AWS EKS
- eksctl
- kubectl
- EC2 (Ubuntu)

## Steps Performed
1. Launched EC2 instance
2. Installed AWS CLI, eksctl and kubectl
3. Created EKS cluster
4. Deployed Nginx application
5. Exposed application using LoadBalancer
6. Accessed application from browser

## Commands Used
eksctl create cluster --name nginx-cluster --region ap-south-1 --nodes 2 --node-type t3.medium --managed
kubectl create deployment nginx --image=nginx
kubectl expose deployment nginx --type=LoadBalancer --port=80
kubectl get nodes
kubectl get pods
kubectl get svc

## Output
Nginx application successfully deployed and accessed via AWS LoadBalancer URL.
