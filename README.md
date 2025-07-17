## 🎮 2048 Game on AWS EKS (Fargate)

A fun implementation of the 2048 game deployed using AWS EKS, ALB Ingress Controller, and Fargate.

![2048 Game Demo](./assets/2048-demo.gif)


##  Tech Stack

- AWS EKS (Fargate)
- Kubernetes
- ALB Ingress Controller
- HTML, CSS, JS (Game)
- kubectl, eksctl, IAM roles

---

##  Screenshots

| Game Interface | EKS Cluster | etc. | https://github.com/AshvinAN/2048-game-aws-eks/tree/c45679ef5d44ccdfe0af26c332839b927b10a609/screenshots
|----------------|-------------|
| ![](./screenshots/2048-Game-Console.png) | ![](./screenshots/EKS-cluster.png) | etc.

---

##  Project Structure

├── manifests/ # Kubernetes YAML files
├── game/ # Game source code
├── screenshots/ # Deployment screenshots
├── README.md
├── LICENSE
└── .gitignore

## 🚀 How I Deployed

1. Created an EKS Cluster with Fargate profile using `eksctl`
2. Applied all Kubernetes manifests  
   ```bash
   kubectl apply -f manifests/
3. Set up ALB Ingress Controller and IAM role
4. Verified service and ingress with:

bash:
kubectl get all -n game-2048
&
kubectl get ingress -n game-2048

5. Accessed game in browser via ALB Ingress URL

##  What I Learned
1. Hosting static apps with Kubernetes

2. Using AWS EKS with Fargate (no EC2 management)

3. Configuring ALB Ingress for web access

4. Working with IAM roles and service accounts

5. Using kubectl, eksctl, and manifest files efficiently

