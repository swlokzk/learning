# Assignment Overview: Create an Architectural Diagram and Cloud Setup

Estimated time: 2 minutes
Introduction

In this module, you will design a container-based architecture to support Retail Bank's modernization initiative. You'll learn to create deployment diagrams, build and manage Docker containers for key banking microservices, and apply security best practices using cloud container registries.
Tasks
Task 1: Design container-based deployment architecture

Create a visual architecture diagram that illustrates modular, containerized banking services, such as authentication, loan servicing, and onboarding, highlighting service interactions and deployment topology using tools such as Lucidchart or Microsoft PowerPoint.
Task 2: Build Docker containers for microservices

Develop Docker containers for core banking services, ensuring modularity and scalability, and prepare container images for deployment in a cloud environment.
Task 3: Push and manage container images in the cloud registry

Use IBM Cloud Container Registry or AWS Elastic Container Registry to push and manage container images, demonstrating cloud-native deployment workflows.
Task 4: Implement container security best practices

Apply security controls, such as image scanning, role-based access control (RBAC), and image signing, to safeguard container deployments in accordance with industry standards.
Task 5: Validate container configurations

Ensure each microservice is modular, runs independently, exposes only necessary ports, and complies with security and compliance standards. Complete the validation checklist to confirm readiness and adherence to governance.
Deliverables

In this module, you will work on the following deliverables:

    Deployment topology diagram (.pptx or .png)
    Dockerfiles for at least three microservices (authentication, loan servicing, onboarding)
    CLI screenshots or logs verifying successful image pushes to a cloud container registry
    A brief description of the implemented security controls in the container setup
    Completed validation checklist (optional XLS) confirming modularity, security, and compliance of containerized services

---

Lab: Container, Docker, and IBM Cloud Container Registry
Estimated time: 30 minutes
Learning objectives

After completing this lab, you will be able to:

    Create a deployment-level architecture diagram showing microservices and container topology
    Build and run Docker containers for key banking modules, including authentication, loan servicing, and onboarding
    Push Docker images to IBM Cloud Container Registry or AWS ECR securely
    Define and document security best practices such as image signing, role-based access, and vulnerability scanning
    Validate container configurations against modularity, resilience, and regulatory compliance standards

Requirements for lab

    Install Docker locally
    IBM Cloud CLI or AWS CLI configured with credentials
    Internet access to a cloud container registry for IBM Cloud Container Registry or AWS ECR
    VS Code or terminal for scripting
    Account on IBM Cloud or AWS (free tier acceptable)

Note: You are advised to use the free version of the above tools. If you plan to upgrade these tools, you are responsible for any applicable charges.
Introduction

In this lab, as part of the core digital transformation, banking services, including customer onboarding, loan servicing, and user authentication, are rearchitected into a centralized microservice. You can package and register these microservices securely, ensure modularity, compliance, and resilience. Using Docker and cloud container registries, you'll learn to re-architect traditional banking services into independent, deployable microservices.
Required tools

    Lucidchart
    Draw.io
    Microsoft PowerPoint

Scenario overview

A retail bank is transitioning its legacy monolithic system to a cloud-native architecture. Microservices will be deployed in isolated containers, allowing rapid scaling, secure access control, and CI/CD-based rollout.

As a solution and system architect, you are tasked with containerizing the three banking services below:

    Authentication service: Handles customer login and token issuance
    Loan Servicing service: Processes EMI, payments, and the loan lifecycle
    Customer onboarding service: Validates KYC, opens an account, and sends welcome messages

Task 1: Design initial container topology

Create a diagram that visually represents how your banking microservices, such as Auth, Loan, and Onboarding, are deployed and interact within a cloud-native, containerized infrastructure.
Step 1: Open a design tool

Select any of the design tool and open it in the browser.

    Lucidchart: Provides clean, professional, and UML-friendly designs
    Draw.io: Free and easy-to-use design tool
    Microsoft PowerPoint: Accessible, with shape and connector design tools

Step 2: Add microservices (Containers)

    Draw three rectangular boxes for containers labeled as:
        Auth-service
        Loan-service
        Onboarding-service

Step 3: Segment the network

You need to show which services are:

    Exposed to the public (for example, API Gateway)
    Kept internal (for example, loan and onboarding)
    Example segmentation layout:

Public network:
└── [API Gateway]
↓
Internal network:
├── [auth-service]
├── [loan-service]
└── [onboarding-service]

    Use color coding or boundary boxes:
    Blue dashed box for "Public network"
    Green solid box for "Internal network"

Step 4: Container registry

Add a shape, like such as a cloud icon or rectangle, labeled:

    IBM Cloud Container Registry
    AWS ECR (Elastic Container Registry)

Then connect arrows from the registry to the containers, showing that images are pulled from there.

    Example:
    [ IBM Cloud Container Registry ]
    ↓
    [ auth-service ]

Step 5: Save your work

Save your designed of the initial container topology as a PNG or PDF with the name container_topology_diagram.pdf and keep it handy for the final project.
Task 2: Build Dockerfiles for three microservices

Each microservice will have its own Dockerfile, which defines the process for building the container.
Step 1: Create auth_service_Dockerfile

Example content:

    #Base image
    FROM node:18-alpine
    #Set working directory
    WORKDIR /app
    #Copy source code
    COPY . .
    #Install dependencies
    RUN npm install
    #Expose required port
    EXPOSE 3000
    #Start service
    CMD [“node”, “auth-server.js”]

Step 2: Create Dockerfiles for the loan service and onboarding

Simply adjust for port and entry file:

loan_service_Dockerfile

    FROM node:18-alpine
    WORKDIR /loan
    COPY . .
    RUN npm install
    EXPOSE 3001
    CMD [“node”, “loan-server.js”]

onboarding_service_Dockerfile

    FROM node:18-alpine
    WORKDIR /onboarding
    COPY . .
    RUN npm install
    EXPOSE 3002
    CMD [“node”, “onboarding-server.js”]

Step 3: Save your work

Save the created Dockerfiles with the names below and keep them handy for the final project.

    auth_service_Dockerfile
    loan_service_Dockerfile
    onboarding_service_Dockerfile

Task 3: Push Docker images to IBM Cloud Container Registry (ICR)

In this task, you will authenticate into IBM Cloud CLI, tag Docker images with the appropriate IBM Container Registry path, push Docker images for each microservice (auth, loan, onboarding) to a secure IBM Cloud Container Registry (ICR), and prepare your services for cloud deployment and future CI/CD pipelines.
Task requirements

    Docker installed and local images built
    IBM Cloud CLI installed
    IBM Cloud account (Free tier is fine)
    Internet access

Steps to be followed
Step 1: Log in to IBM Cloud

    Open your terminal or command prompt and enter ibmcloud login. This will prompt you to enter your IBM Cloud email address and password.
    Set the container registry region ibmcloud cr region-set us-south.
    You should see a message, The container registry region is now set to 'us-south'.

Step 2: Tag and push Docker images to ICR

Let's assume your IBM Cloud registry namespace is abc-banking.

    For the auth-service
        Tag the image for IBM Container Registry
        docker tag abc/auth-service:latest us.icr.io/abc-banking/auth-service:latest
        Push the image to IBM Cloud
        docker push us.icr.io/abc-banking/auth-service:latest
    For the loan service, use the command below to tag the image for IBM Container Registry and push it to IBM Cloud
        docker tag abc/loan-service:latest us.icr.io/abc-banking/loan-service:latest
        docker push us.icr.io/abc-banking/loan-service:latest
    For onboarding service, use the command below to tag the image for IBM Container Registry and push it to IBM Cloud
        docker tag abc/onboarding-service:latest us.icr.io/abc-banking/onboarding-service:latest
        docker push us.icr.io/abc-banking/onboarding-service:latest
    Follow the checklist once you push the Dockerfiles
        Images are tagged correctly (with us.icr.io/abc-banking/…)
        All 3 services pushed without errors
        You can verify the pushed images via:
        ibmcloud cr images

Task 4: Define security best practices

To ensure that container deployments are secure, document industry best practices in a Markdown file named security_practices.md.
Step 1: Create a Markdown file

    In your editor, such as VS Code, create a Markdown file and name it security_practices.md.
    Add the content below

    #Security Best Practices for Containerization
    ##1. Enable Image Signing

        Use Docker Content Trust or IBM Cloud CR signing
        Ensure all images are signed before push

    ##2. IAM Role-Based Access

        Use namespace separation: dev, staging, prod
        Assign IAM roles for fine-grained access to containers

    ##3. Vulnerability Scanning

        Integrate Trivy or IBM Cloud Image Scan
        Scan all images before deployment
        Fail builds if critical CVEs are found

    ##4. Private Registry Enforcement

        Do not expose your registry publicly
        Enable access logging and monitor unusual activity

Task 5: Validation checklist

Review the created container, Docker, and IBM Cloud container registry to ensure that the following items are incorporated:

    Each service is modular and runs independently
    Containers expose only necessary ports
    Images are stored securely in IBM Cloud CR or AWS ECR
    Topology supports isolation and compliance segmentation
    Security features (scan, RBAC, signed images) are documented

Summary

Congratulations on completing the Lab: Containerization of Banking Microservices Using Docker and IBM Cloud Container Registry! You've learned to design a containerized architecture for key banking services, build and push Docker images to a secure cloud registry, and implement security best practices such as image signing, access control, and vulnerability scanning to ensure modularity, compliance, and resilience.
Author

Parikshit Jain
