# CI-CD-Automation-Pipeline

Welcome to the CI-CD-Automation-Pipeline! This project aims to establish a robust Continuous Integration and Continuous Deployment (CI/CD) pipeline using a variety of tools and technologies. Below is an overview of the project architecture, workflow & topics covered as part of this Project.

## Project Architecture Overview

![Screenshot (318)](https://github.com/Bathalapalli-SaiRangaPavan/CI-CD-Automation-Pipeline/assets/121741348/eb0fbaf2-17ed-43f5-b67f-8b2631557131)


### Version Control System (VCS)

- **GitHub**: Used for hosting the source code repositories.

### Continuous Integration (CI) and Continuous Deployment (CD) Tools

- **Jenkins**: Orchestrates the CI/CD pipeline.
- **Maven**: Handles the building of source code.
- **Sonarqube**: Conducts code analysis to ensure code quality.
- **JFrog Artifactory**: Acts as a repository for storing artifacts.
- **Docker**: Utilized for containerization of microservices.
- **Kubernetes**: Manages containerized applications.
- **Helm Charts**: Simplifies the deployment of applications on Kubernetes.
- **Prometheus & Grafana**: Used for monitoring the Kubernetes environment.

### Infrastructure Provisioning and Configuration Management

- **Terraform**: Used for provisioning infrastructure resources on AWS.
- **Ansible**: Handles configuration management tasks such as setting up Jenkins and Kubernetes deployment.

### Cloud Provider

- **AWS (Amazon Web Services)**: Infrastructure is provisioned and hosted on AWS.

## Project Workflow

### Source Code Management

- Developers push code changes to GitHub repositories.

### Continuous Integration

- Jenkins retrieves the source code from GitHub.
- Jenkins utilizes Maven to build the source code.
- Sonarqube conducts code analysis to ensure code quality.

### Artifact Management

- Upon successful code analysis, artifacts are stored in JFrog Artifactory.

### Containerization

- Docker is employed to create Docker images of microservices.
- Docker images are stored in JFrog Artifactory.

### Continuous Deployment

- Kubernetes orchestrates the deployment of containerized applications.
- Helm Charts streamline the deployment process on Kubernetes.

### Monitoring and Observability

- Prometheus collects metrics from Kubernetes pods.
- Grafana visualizes the collected metrics, providing insights into the Kubernetes environment's performance.

### Infrastructure Provisioning and Configuration

- Terraform provisions the necessary infrastructure resources on AWS.
- Ansible handles configuration tasks such as setting up Jenkins and deploying applications on Kubernetes.



## Topics Covered as part of this Project

1. **Terraform Setup**
   - Provision Terraform and configure infrastructure on AWS.

2. **Jenkins Setup**
   - Provision Jenkins master, build node, and Ansible using Terraform.
   - Set up Ansible server.
   - Configure Jenkins master and build node using Ansible.
   - Create a Jenkins pipeline job.
   - Create a Jenkins file from scratch.
   - Create a Multi-branch pipeline.
   - Enable webhook on GitHub.

3. **SonarQube Integration**
   - Configure SonarQube and Sonar Scanner.
   - Execute SonarQube analysis.
   - Define rules and gates on SonarQube.
   - Configure Sonar callback rules.

4. **JFrog Artifactory Setup**
   - Set up JFrog Artifactory.
   - Create a Dockerfile store.
   - Store Docker images on JFrog Artifactory.

5. **Kubernetes Setup**
   - Provision Kubernetes cluster using Terraform.
   - Create Kubernetes objects.
   - Deploy Kubernetes objects using Helm.

6. **Monitoring and Observability**
   - Set up Prometheus and Grafana using Helm Charts.
   - Monitor Kubernetes Cluster Using Prometheus.

## Prerequisites
- Familiarity with AWS services for infrastructure provisioning using Terraform.
- Basic understanding of Docker, Kubernetes, Jenkins, and Ansible.
- Knowledge of Git and version control workflows.

## Getting Started
To get started with the project, please follow the setup and installation instructions provided in the respective tool documentation.


