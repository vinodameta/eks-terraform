# eks-terraform

# Please apply below command after terraform install
1. terraform init
2. terraform plan
3. terraform apply

This will crate a EKS cluster in AWS Infra.

# get Kubeconfig locally with below command.
1. aws eks update-kubeconfig --name <eks_cluster_name>

# After kube config set up , deploy application as below.
1. kubectl apply -f redis-deployment.yml
2. kubectl apply -f redis-service.yml
3. kubectl apply -f web-deployment.yml
4. kubectl apply -f web-service.yml

Verify an app on ALB endpoint.
