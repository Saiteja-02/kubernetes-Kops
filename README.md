# Kubernetes Cluster Deployment with kOps on AWS EC2

This repository contains configuration and automation scripts for deploying a Kubernetes cluster on **AWS EC2** using **kOps**. The goal is to provision a scalable, manageable Kubernetes cluster via declarative infrastructure.

---

## 🧰 Prerequisites

- `kubectl` installed  
- `kops` (Kubernetes Operations) binary compatible with your system  
- AWS IAM permissions:  
  - AmazonEC2FullAccess  
  - AmazonRoute53FullAccess  
  - AmazonS3FullAccess  
  - IAMFullAccess  
  - AmazonVPCFullAccess  
  - (and any other permissions required for VPC, DNS, etc.)

---

## 🚀 Deployment Steps (High-Level)

1. Create a state store (S3 bucket) for kOps configuration  
2. Define your cluster configuration (YAML)  
3. Use `kops create cluster` pointing to the state store  
4. `kops update cluster --yes` to apply changes  
5. Validate cluster with `kops validate cluster`  
6. (Optional) Make edits, update cluster, and reconciling changes  

---

## 🛠 Tools / Technologies Used

- **kOps** (Kubernetes Operations)  
- **AWS EC2 / VPC / IAM / S3 / Route53**  
- **Infrastructure as Code (IaC)**  
- YAML / JSON templating  
- Git / version control  

---

## 🧩 Concepts & Frameworks Applied

- Kubernetes cluster orchestration & lifecycle management  
- Infrastructure as Code (IaC) patterns  
- AWS cloud services and IAM security best practices  
- Declarative infrastructure and automation  

---

## 📂 Repository Structure

