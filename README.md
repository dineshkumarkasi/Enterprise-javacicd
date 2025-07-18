# 🚀 Spring Boot CI/CD Pipeline with Jenkins, SonarQube, Docker, ECR, ArgoCD, and EKS

This project demonstrates a complete DevOps CI/CD pipeline to build, test, scan, and deploy a Spring Boot application to a Kubernetes cluster (EKS) on AWS using Jenkins, SonarQube, Docker, ECR, ArgoCD, Prometheus, and Grafana.

---

## 🎯 Objective

To automate the entire software delivery lifecycle of a Spring Boot application using a modern DevOps toolchain. The pipeline enables continuous integration, code quality analysis, containerization, security scanning, and continuous delivery into AWS EKS, while also providing observability with Prometheus and Grafana.

---

## 🛠️ Tools & Technologies

| Tool          | Purpose                                  |
|---------------|------------------------------------------|
| **Spring Boot**     | Java-based web application             |
| **Jenkins**         | CI/CD automation server                |
| **Maven**           | Build and dependency management        |
| **SonarQube**       | Static code analysis                   |
| **Docker**          | Containerization                       |
| **Amazon ECR**      | Docker image registry                  |
| **ArgoCD**          | GitOps-based Kubernetes deployment     |
| **Amazon EKS**      | Managed Kubernetes cluster             |
| **Prometheus**      | Metrics collection and monitoring      |
| **Grafana**         | Dashboards and visualization           |

---

## 📐 Architecture Diagram

 
![Architecture Diagram](architecture-planned.png)

> 💡 **Replace the above image link** with the correct path to your architecture diagram image in the GitHub repo. For example:
>
> - Upload your image (e.g. `cicd-architecture.png`) to the repo or as a GitHub issue asset
> - Right-click the uploaded image → “Copy image address”
> - Replace the placeholder URL above

---

## 🔄 CI/CD Pipeline Flow

1. Code pushed to GitHub triggers Jenkins pipeline
2. Jenkins builds the app using Maven
3. Code is analyzed by SonarQube for bugs, code smells, and security issues
4. Docker image is built and pushed to Amazon ECR
5. Image is optionally scanned (e.g., ArcocB, Trivy)
6. ArgoCD automatically syncs manifests and deploys to Amazon EKS
7. Prometheus scrapes app and system metrics
8. Grafana visualizes the metrics

---

## 📁 Project Structure

