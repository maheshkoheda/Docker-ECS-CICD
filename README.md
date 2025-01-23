# Docker-ECS-CICD
CICD to build, test, create docker image, push to ECR, Fetch from ECR and orchestrate in ECS
Overview
This project demonstrates a CI/CD pipeline for the vProfile application using Jenkins, Maven, SonarQube, Nexus, Docker, AWS ECR, and ECS. The pipeline automates the process of building, testing, analyzing, containerizing, and deploying the application.
Technologies Used
•	Jenkins: CI/CD automation
•	Maven: Build and dependency management
•	SonarQube: Code quality analysis
•	Checkstyle: Static code analysis
•	Nexus: Artifact repository
•	Docker: Containerization
•	AWS ECR: Docker image registry
•	AWS ECS: Container orchestration
CI/CD Pipeline Workflow
1.	Fetch Code: Clone the repository from GitHub.
2.	Build Application: Compile and package the application.
3.	Run Unit Tests: Execute automated tests.
4.	Code Analysis: 
o	Checkstyle for code formatting
o	SonarQube for code quality
5.	Quality Gate: Enforce quality standards.
6.	Build Docker Image: Create a container image.
7.	Push Image to AWS ECR: Upload the built image to AWS Elastic Container Registry.
8.	Deploy to AWS ECS: Update the ECS service with the new image.
Pipeline Script (Jenkinsfile)- Attached
Setup Instructions
1.	Install Jenkins and required plugins (Maven, SonarQube, Docker, AWS CLI, Pipeline, Git and many more).
2.	Configure AWS credentials in Jenkins for ECR and ECS.
3.	Set up SonarQube server and connect it with Jenkins.
4.	Push the Pipeline Script to Jenkins and trigger the build.

<img width="792" alt="jenkins2" src="https://github.com/user-attachments/assets/5f1bcb2a-ba87-4135-8828-11465ddf868b" />

