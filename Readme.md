## Mastering 3-Tier Application Blue-Green Deployment on AWS EKS: A Step-by-Step Guide to Zero-Downtime Releases

### 🚀 Project Description
This project showcases how to achieve Blue-Green Deployment on AWS using Kubernetes (EKS) to enable zero-downtime deployments. Leveraging automation with Jenkins, the CI/CD pipeline handles seamless application updates, directing traffic between environments for smooth transitions.

---

### Overview

#### 🛠️ Tools Used:
- **AWS EKS**: Managed Kubernetes cluster on AWS, providing a scalable and highly available infrastructure.
- **Terraform**: Infrastructure as Code (IaC) tool for provisioning and managing AWS resources.
- **Jenkins**: CI/CD automation server to manage the deployment pipeline.
- **AWS Load Balancer Controller**: Manages traffic routing and load balancing between Blue and Green environments.

#### 🔑 Key Concepts:
- **Blue-Green Deployment**: A deployment strategy that involves two identical environments (Blue and Green) to transition from the current version to the new one with minimal downtime.
- **CI/CD Pipeline**: Automates the build, test, and deployment stages, reducing manual work and ensuring reliability.
- **Zero-Downtime Deployment**: Enables uninterrupted service availability during application updates.

---

### 📝 Pipeline Stages

1. **Build**:
   - Compiles the application and creates a Docker image.
   - Stores the image in a container registry (e.g., Amazon ECR).

2. **Test**:
   - Runs automated tests to ensure application reliability and correctness.

3. **Deploy**:
   - Deploys the Docker image to both Blue and Green environments within the Kubernetes cluster.
   - Uses Kubernetes manifests and Helm charts to configure each environment.

4. **Switch Traffic**:
   - Routes traffic between Blue and Green environments using AWS Load Balancer Controller.
   - Ensures traffic is directed to the new environment after successful deployment, without affecting users.

---

### 🎯 Outcome

- **Zero-Downtime Deployments**: Ensures seamless transitions for end-users with uninterrupted service availability.
- **Automated Release Management**: Speeds up deployment cycles and minimizes manual intervention.
- **Reliable Infrastructure**: Uses best practices for Blue-Green deployment and CI/CD to maintain a robust and scalable system.

---

🔗 Dive into this project to gain a deep understanding of Blue-Green Deployment strategies and CI/CD automation on AWS EKS!