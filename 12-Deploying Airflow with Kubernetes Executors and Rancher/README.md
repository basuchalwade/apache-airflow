# Deploying Airflow with K8S Executors and Rancher


# Deploying Airflow with K8S Executors & Rancher

<span style="color:#24292F">Quick overview of EKS</span>

<span style="color:#24292F">Set up an EC2 instance for Rancher</span>

<span style="color:#24292F">Create an IAM User with permissions</span>

<span style="color:#24292F">Create an ECR repository</span>

<span style="color:#24292F">Create an EKS cluster with Rancher</span>

<span style="color:#24292F">How to access applications from the outside?</span>

<span style="color:#24292F">Deploy Nginx Ingress with</span>  <span style="color:#24292F">Catalogs</span>  <span style="color:#24292F">\(Helm\)</span>

<span style="color:#24292F">Deploy and run Airflow with the Kubernetes Executor on EKS</span>

# Overview of AWS EKS

AWS EKS \(Elastic Kubernetes Service\)

Makes easy to deploy\, manage and scale containerized applications

Orchestrate your containers

Still need to configure subnets\, VPS\, IAM roles\, SSH keys\.\.\.

Integrated with AWS services \(ECR\, ELB\, IAM\, \.\.\.\)

![](img/12-Deploying%20Airflow%20with%20Kubernetes%20Executors%20and%20Rancher1.jpg)

# Overview

![](img/12-Deploying%20Airflow%20with%20Kubernetes%20Executors%20and%20Rancher2.png)

# Access applications from outside

Service\, Load Balancer\, Ingress

# The Issue

![](img/12-Deploying%20Airflow%20with%20Kubernetes%20Executors%20and%20Rancher3.png)

![](img/12-Deploying%20Airflow%20with%20Kubernetes%20Executors%20and%20Rancher4.png)

# ClusterIP

![](img/12-Deploying%20Airflow%20with%20Kubernetes%20Executors%20and%20Rancher5.png)

# NodePort

![](img/12-Deploying%20Airflow%20with%20Kubernetes%20Executors%20and%20Rancher6.png)

# Load Balancer

![](img/12-Deploying%20Airflow%20with%20Kubernetes%20Executors%20and%20Rancher7.png)

# Ingress

![](img/12-Deploying%20Airflow%20with%20Kubernetes%20Executors%20and%20Rancher8.png)
