# Application-Deployment-on-AWS-EKS

Excited to share Hands-on Kubernetes End-to-End project on EKS with Fargate and Application Load Balancer Ingress Controller:
 
The Process is as follows:
1. As a pre-requisite installed kubectl, eksctl and awscli.
2. Created a EKS cluster using fargate using CLI command.
3  Updated the kubeconfig file to access the resources that have been created in the cluster through CLI.
4. Created a namespace “game-2048” attaching to fargate profile.
5.Deployed the 2048 application, service and set up an ingress resource to route the traffic.
6. Implemented a ingress controller to automate the Application load balancer creation.
7. Before the deployment of ALB controller we need to setup IAM OIDC provider to let the ALB controller access the application load balancer. 8. Setup a service account with appropriate IAM Role and Policy.
9. Used Helm charts to deploy the ALB controller
10. Access the deployed 2048 application running in EKS
