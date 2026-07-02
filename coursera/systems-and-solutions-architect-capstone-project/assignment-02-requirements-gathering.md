# Assignment Overview: Requirements Gathering

Estimated time: 4 minutes
Introduction

In this module, you'll master the requirements gathering lifecycle for Retail Bank's Digital Core Transformation. You will learn to conduct stakeholder engagement, elicit and document requirements, and establish traceability for complex banking systems using industry-accepted enterprise architecture frameworks.​
Tasks
Task 1: Draft the Business Requirements Document (BRD)

Define the project scope, objectives, and metrics for Retail Bank's transformation, which involves integrating legacy systems into a secure, scalable, cloud-native platform. Document assumptions and set measurable success criteria to support architectural planning and regulatory compliance.​
Task 2: Elicit requirements via stakeholder workshops and interviews

Interview product owners, compliance teams, DevOps engineers, and customers to collect functional and non-functional requirements. Record expectations for onboarding, audit, automation, uptime, and security, mapping feedback to business goals.​
Task 3: Create a use case diagram with flow descriptions

Model interactions between actors—such as internal teams, customers, and regulators—to visualize system boundaries and responsibilities. Diagram key use cases and document detailed flows for onboarding, compliance, deployment, and reporting using specialized tools.​
Task 4: Build the Requirements Traceability Matrix (RTM)

Construct an RTM in Excel linking requirements to objectives and test strategies. Include acceptance criteria, verification methods, and risk notes, and ensure traceability for business alignment, compliance, and performance validation.​
Deliverables

In this module, you will work on the following deliverables:

    Completed Business Requirements Document (BRD) summarizing scope, objectives, assumptions, and metrics
    Use Case Diagram and flow descriptions illustrating stakeholder-system interactions
    Requirements Traceability Matrix (RTM) connecting requirements to business objectives with test methods and criteria

Author(s)

Parikshit Jain

---

# Lab: Requirements Gathering

Estimated time: 30 minutes
Learning objectives

After completing this lab, you will be able to:

    Create a Business Requirements Document (BRD) outlining scope, objectives, assumptions, and success metrics for a retail bank's core digital transformation project
    Collect business and technical requirements through interviews and workshops with banking stakeholders, including product owners, compliance leads, DevOps, and customers
    Create the use case diagram and detailed flow descriptions to visualize stakeholder-system interactions
    Build a requirements traceability matrix (RTM) to link requirements to business objectives and ensure alignment

Required tools

    Google Docs
    Google Spreadsheet
    Lucidchart

Introduction

This lab integrates stakeholder engagement, requirements elicitation, and documentation tasks for a retail bank's core digital transformation project. By drafting a BRD, eliciting requirements, creating use case diagrams with flow descriptions, and building an RTM, you will ensure stakeholder alignment, clarify system functionality, and maintain traceability to business objectives, adhering to PMI standards for Business Analysts.
Task 1: Draft a Business Requirements Document (BRD)
Objective

Create a BRD for modernizing a retail bank's core systems using a secure, compliant, and cloud-native architecture
Step 1: Define key elements of the BRD

Start by outlining the key components of the Business Requirements Document (BRD) based on a retail bank's scenario. Include the following:

    Scope: Define the project as a digital transformation initiative to integrate fragmented systems, including customer onboarding, loan servicing, fraud detection, and compliance monitoring into a unified platform.

    Objectives:
        Migrate to a secure cloud-native infrastructure by the fourth quarter
        Improve onboarding and loan processing time by 40%
        Achieve 100% compliance with KYC, AML, PCI-DSS, and GDPR
        Maintain 99.99% uptime with scalable infrastructure

    Assumptions:
        Vendor contracts are in place
        Stakeholders are available for workshops and validations
        Cloud environment is provisioned and secure

    Success metrics:
        Zero regulatory violations post-launch
        Less than 2 seconds of average API response times
        Successful CI/CD implementation with rollback functionality
        Customer satisfaction improvement based on post-deployment survey

Step 2: Save your work

    Once your Business Requirements Document (BRD) is complete, including scope, objectives, assumptions, and success metrics, review for clarity and accuracy.

    Save the file with a clear name, such as Name_BRD.pdf, and save a copy for future reference or stakeholder review.

Task 2: Elicit requirements via interviews/workshops
Objective

Gather functional and non-functional requirements from key banking stakeholders
Step 1: Plan interviews and workshops

Begin by identifying key stakeholder groups and selecting the most suitable methods, such as interviews, surveys, or workshops, to gather insights into their needs and expectations. Use the following approach:

    Product owners: Understand business logic for onboarding, transaction flow, and fraud management
    Compliance teams: Capture requirements for audit trails, data governance, and reporting standards
    DevOps engineers: Clarify CI/CD needs, monitoring, security enforcement, and deployment frequency
    Customers: Collect expectations on service reliability, digital experience, and access control

Step 2: Document requirements

Translate stakeholder input into clearly written functional and non-functional requirements that can guide system design and development.

    Functional requirements (FR):
        FR1: Customers can securely onboard and manage accounts via web and mobile apps
        FR2: Compliance staff can access real-time audit logs and KYC reports
        FR3: Product owners can configure loan approval workflows and fraud detection rules
        FR4: DevOps can automate builds, tests, and deployment pipelines

    Non-functional requirements (NFR):
        NFR1: Less than 2 seconds of average response time for all public-facing APIs
        NFR2: System must achieve 99.99% uptime across core services
        NFR3: Encryption at rest and in transit must comply with bank-grade security policies

Step 3: Save your work

After documenting all functional and non-functional requirements gathered from interviews and workshops, review for completeness and traceability.

Save your file as Name_Requirements.pdf, and keep it handy for use in your project documentation.
Task 3: Create a use case diagram and detailed flow descriptions
Objective

Visualize system interactions and responsibilities of different actors in the banking ecosystem.
Step 1: Download template

Download the Template_Use Case Diagram (Word or PDF). This document includes structured tables for documenting actors, use cases, relationships, and reflections.

You may use any diagramming tool (Lucidchart, Draw.io, Visio, etc.) to visualize your diagram. Export and embed it in the template where indicated.
Step 2: Identify actors

List the key users or systems that interact with a retail bank's digital transformation. Specify internal or external actor

For example:

    Primary actors: Product owners, compliance officers, DevOps engineers, and so on
    Secondary actors: Customers, external regulators, credit bureau APIs, and so on

Fill in the actors' column in the template with:

    Actor name
    Primary/Secondary designation
    Their role in the system
    How they interact with the system

Step 3: Define the use case

Identify the major functionalities the system should support, based on the actors' goals

In the Use Case Table, enter for each use case:

    Name (for example, Manage Patient Account)
    Description of what the system does in response to that actor's action

Hint for sample use cases:

    Customers: Onboard new customers
    Compliance officers: Configure compliance rules
    DevOps: Manage deployment pipeline
    Product owner: Monitor fraud alerts
    Regulators: Access regulatory reports

Step 4: Create a use case diagram

Use Lucidchart, Visio, or Draw.io to visualize use cases and actors with system boundaries that represent how actors interact with a retail bank's digital transformation.

Follow the steps below:

    Enable UML shapes or symbols
    Add the system boundary
    Add use cases inside the system boundary, linked via associated lines to each actor
    Add actors outside the system boundary, including customers, regulators, and payment gateways
    Connect actors to their use cases

Step 5: Define relationships between actors and use cases

In this step, you will specify how each actor interacts with the system by mapping them to the relevant use cases. This helps illustrate whether the interaction is direct (the actor performs the task within the system) or indirect (the actor is affected or involved behind the scenes).

In the table given in the template, complete the following:

    Onboard new customer: Customer submits KYC info; system validates via API; compliance team approves; user gains access
    Configure compliance rules: Officer defines thresholds; system applies them across transactions; real-time updates push to audit logs
    Manage deployment pipeline: DevOps triggers build/test pipeline; system executes in staging; automated checks run before release
    Monitor fraud alerts: Product owner receives rule-triggered alerts; reviews logs; flags for investigation
    Access regulatory reports: System generates compliance reports; regulators access via secure portal

Step 6: Answer reflection questions (Optional)

Reflect on your experience by answering the questions in the template. Briefly describe any challenges faced, the benefits of your diagram, and possible strategies for improving system design or stakeholder engagement
Step 7: Save your work

    Save your completed Use Case Diagram with a clear filename (for example, Name_UseCaseDiagram.pdf) after updating all sections, including actors, use cases, and relationships

Task 4: Build requirements traceability matrix (RTM)
Objective

Map all requirements back to business objectives and define test strategies
Step 1: Download and review the RTM template

Download the Traceability Matrix template and Example.xlsx. This template includes a blank traceability matrix, step-by-step instructions, and an example to guide you through the process.
Step 2: List requirements

Refer to the requirements developed in your earlier analysis and document the following sample entries:

    Functional requirements (FRs):
        FR1: Customers can securely onboard and manage accounts via web and mobile apps
        FR2: Compliance staff can access real-time audit logs and KYC reports
        FR3: Product owners can configure loan approval workflows and fraud detection rules
        FR4: DevOps can automate builds, tests, and deployment pipelines

    Non-functional requirements (NFR):
        NFR1: Less than 2 seconds of average response time for all public-facing APIs
        NFR2: The system must achieve 99.99% uptime across core services
        NFR3: Encryption at rest and in transit must comply with bank-grade security policies

Requirement ID 	Requirement description 	Type
FR1 	Customers can securely onboard and manage accounts via web and mobile apps 	Functional
FR2 	Compliance staff can access real-time audit logs and KYC reports 	Functional
FR3 	Product owners can configure loan approval workflows and fraud detection rules 	Functional
FR4 	DevOps can automate builds, tests, and deployment pipelines 	Functional
NFR1 	Less than 2 seconds of average response time for all public-facing APIs 	Non-Functional
NFR2 	The system must achieve 99.99% uptime across core services 	Non-Functional
NFR3 	Encryption at rest and in transit must comply with bank-grade security policies 	Non-Functional
Step 3: Map to objectives and use cases

    Align each requirement with the relevant BRD objective. For example: compliance–> performance –> automation
    Complete each row using traceable IDs

Step 4: Define acceptance criteria

    Specify testable outcomes

Step 5: Include verification methods

    For example: API benchmarking, security testing, and audit log validation

Step 6: Review your matrix

    Review your created matrix for coverage and traceability

Step 7: Save your work

    Once your Requirements Traceability Matrix is complete and reviewed for accuracy, save the file as Name_RTM.pdf. Keep this file handy for future reference or inclusion in your professional portfolio.

Summary

Congratulations on completing Lab: Requirements Gathering!

In this lab, you gained hands-on experience in end-to-end requirements engineering within a regulated financial institution. By completing these tasks, you will strengthen your skills in elicitation, modeling, and validation—core competencies essential for becoming a job-ready systems architect or solution designer in the banking industry.
Author

Parikshit Jain

