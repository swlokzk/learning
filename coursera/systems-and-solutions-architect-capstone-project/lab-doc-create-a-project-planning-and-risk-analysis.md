
# Lab: Create a Project Planning and Risk Analysis

Estimated time: 30 minutes
Learning objectives

After completing this lab, you will be able to:

    Analyze a retail bank's transformation scenario to develop a work breakdown structure (WBS) and network diagram
    Perform a SWOT analysis to evaluate internal strengths, weaknesses, and external opportunities and threats
    Develop a risk register to identify, prioritize, and plan responses to risks in a banking environment
    Create a risk matrix to map and rank threats and opportunities based on probability and impact

Introduction

Effective project planning and risk analysis form the foundation of any successful transformation initiatives, specifically in the finance industry. In this lab, you will explore how to structure a planning tools that help teams break down complex programs, visualize dependencies, and anticipate potential obstacles before the final deployment. You will also develop a WBS, conduct a SWOT analysis, and apply risk-management techniques to identify critical threats and opportunities.
Software requirements

Access to Microsoft Office or the free web version of Microsoft 365 (available at office.com) is required. Familiarity with alternative tools such as Google Docs and Google Sheets may also be sufficient.

Note: Please follow the steps given here to sign up for Microsoft 365.
Notes

    Templates follow PMI guidelines for architecture and risk planning
    Save all outputs to use as part of the Final Project

Scenario: Core digital transformation for a retail bank

A retail bank is undergoing a mission-critical digital transformation of its legacy systems to modernize services, including customer onboarding, loan servicing, transaction monitoring, and compliance reporting. The initiative is driven by the need for real-time data access, high system uptime, secure infrastructure, and adherence to KYC, AML, and PCI-DSS regulations. Stakeholders include CTO Rachel Singh, Architect Arjun Desai, Compliance Officer Nina Patel, and Product Owner Sameer Khan. The transformation must be completed within twelve months, adhering to strict budget and regulatory constraints.
Exercise 1: Build a work breakdown structure (WBS) and network diagram

In this exercise, you'll develop a WBS and network diagram to visualize project phases and the schedule.
Task 1: Build a work breakdown structure (WBS)

Based on the retail banking digital transformation scenario, you will use the Microsoft Excel WBS Template to create a work breakdown structure (WBS) for retail banking. This WBS will help you organize and structure the major phases and tasks involved in the project.

Let's look at the steps for building a WBS for retail banking.
Step 1: Download template

Download the WBS Template This template is structured to help you break down the Core digital transformation for a retail banking project into manageable components, including planning, executing, and closure.
Step 2: Enter project name

Enter the project name 'Core digital transformation for a retail banking' in Level 1 activity 1.0.
Step 3: Define high-level phases

Add the three major phases of the project under Level 2:

    1.1 Planning
    1.2 Execution
    1.3 Closure

Step 4: Add planning tasks

Under the planning phase, add the following tasks:

    1.1.1 Identify stakeholders
    1.1.2 Gather requirements
    1.1.3 Design cloud-native architecture

Step 5: Add execution tasks

Under the execution phase:

    1.2.1 Configure CI/CD Pipeline
    1.2.2 Integrate Core Banking & API Layers
    1.2.3 Test Compliance (KYC/AML/PCI-DSS)

Step 6: Add closure tasks

Under the closure phase, list:

    1.3.1 Deploy to Production
    1.3.2 Conduct User Training
    1.3.3 Perform Handover to Operations

Step 7: Save your work

Save your work breakdown structure as Name_WBS.pdf and keep it handy for the final project.
Task 2: Build a network diagram

Based on the scenario, you will develop a network diagram for this project, focusing on the phases of Planning, Executing, and Closure.
Step 1: Download template

Download the Network Diagram Template. This template supports visualizing task sequences and timelines.
Step 2: Sequence planning tasks

Complete the sequence planning for each task. Place activities from the planning tasks 1.1.1–1.1.3 in the order you believe should occur. If the tasks can occur concurrently, show them as happening simultaneously. If there are dependencies, place the activities accordingly. Calculate the total duration for this phase, which should be 2 weeks.
Step 3: Sequence execution tasks

Complete sequencing the execution tasks by placing activities from 1.2.1 to 1.2.3 in the order you believe should occur. If the activities can happen concurrently, show them occurring simultaneously. If there are dependencies, place the activities accordingly. Calculate the total duration for this phase, which should be 6 months.
Step 4: Sequence closure tasks

Complete sequencing of the closure activities by placing activities from 1.3.1 to 1.3.3 in the order you believe should occur. If the activities can happen concurrently, show them occurring simultaneously. If there are dependencies, place the activities accordingly. Calculate the total duration for this phase, which should be 1.5 months.
Step 5: Calculate total project duration

Add the planning, execution, and closure activities to calculate the total time required to complete this project. The estimated duration is 9.5 months.
Step 6: Save your work

Save your created Network Diagram as Name_NetworkDiagram.pdf and keep it handy for the final project.
Exercise 2: Perform SWOT analysis

In this task, you will assess both internal and external factors influencing the success of the core digital transformation for a retail bank project using a structured SWOT analysis. This will help you identify strengths to leverage, weaknesses to address, opportunities to explore, and threats to mitigate.
Step 1: Download template

Download the SWOT analysis template (Word or PDF) provided in Microsoft Word or PDF format. This template will guide you in organizing and documenting your findings across four SWOT categories.
Step 2: Identify SWOT factors

Using the information from the Core digital transformation for a retail bank scenario, list relevant internal and external factors in each section of the template:

    Strengths:
        Experienced DevOps team
        CTO sponsorship
        Secured cloud partnerships
    Weaknesses:
        Legacy integration risk
        Skill silos
        Compliance complexity
    Opportunities:
        Real-time banking
        Advanced fraud detection
        Regulatory technology (regtech)
    Threats:
        API dependencies
        Fintech competition
        Audit nonconformance

Step 3: Save your work

Save your SWOT Analysis as Name_SWOTAnalysis.pdf and keep it handy for the final project.
Exercise 3: Develop a Risk Register

In this exercise, you will identify and document potential risks associated with the Core digital transformation for retail banking. You will also analyze threats and opportunities, assign risk ratings, and outline appropriate response strategies. This proactive approach helps minimize project disruptions and maximize positive outcomes.
Step 1: Download template

Download the Risk Register Template. The template is structured to help you document risk-related details, including causes, events, and mitigation strategies.
Step 2: Document risks

Using the retail banking scenario, document each identified risk using the columns in the template. Include both negative threats and positive opportunities. Ensure that each risk entry is specific, realistic, and aligned with the scenario.

For example, review the following table:
Risk ID 	Risk Title 	Cause 	Event 	Impact 	Category
R1 	KYC API SLA Violation 	Third-party provider latency 	Delay in customer onboarding 	Compliance risk, reputational damage 	Threat
R2 	Legacy System Integration Failure 	Outdated APIs and schema mismatches 	Transactional errors or data loss 	Project delay, rollback, additional cost 	Threat
R3 	CI/CD Pipeline Breakdown 	Inadequate rollback automation 	Deployment failure 	Downtime, failed sprint releases 	Threat
R4 	Positive Stakeholder Adoption 	Intuitive workflows and dashboards 	Increased engagement 	Accelerated feedback loops, smoother rollout 	Opportunity
Step 3: Assign risk ratings

For each risk, assign a Probability (1–5) and an Impact (1–5). Then, calculate the Risk Score by multiplying the two values.

Example:

    R1: Probability = 4, Impact = 5 → Score = 20
    R2: Probability = 4, Impact = 4 → Score = 16
    R3: Probability = 3, Impact = 3 → Score = 9
    R4: Probability = 2, Impact = -4 → Score = -8 (Opportunity)

This score helps prioritize risks based on their potential impact on the project.
Step 4: Define triggers

List the early warning signs or triggers that may indicate that a risk is about to occur:

    R1: Missed onboarding logs or delayed provider response
    R2: Failed data validation between legacy and modern systems
    R3: Build errors or unresponsive test environments
    R4: Early user feedback praising UX design

Triggers help the team respond proactively before the risk escalates.
Step 5: Develop response strategies

For each risk, define clear response strategies to either mitigate threats or enhance opportunities:

    R1: Implement provider SLA monitoring with escalation matrix
    R2: Conduct sandbox integration tests and version control audits
    R3: Enhance rollback scripts, add pre-deployment quality checks
    R4: Highlight success stories internally and promote adoption features

These actions should be practical and tailored to each specific risk.
Step 6: Save your work

Save your developed risk register as Name_RiskRegister.xlsx and keep it handy for the final project.
Task 4: Develop a Risk Matrix

In this task, you will visualize and categorize project risks by mapping them onto a Risk Matrix, helping prioritize action based on impact and probability. This tool will support risk-aware decision-making for the Core digital transformation for a retail bank.
Step 1: Download template

Download the Risk Matrix Template. This template includes a standard threat matrix and opportunity matrix, allowing you to plot risks based on their likelihood and impact.
Step 2: Map risks on the matrix

Using the probability and impact scores from your Risk Register, place each risk on the matrix:

    R1: KYC API SLA violation → (4,5) on Threat Matrix
    R2: Legacy system integration failure → (4,4) on Threat Matrix
    R3: CI/CD pipeline breakdown → (3,5) on Threat Matrix
    R4: Positive stakeholder adoption → (2,-4) on Opportunity Matrix (negative impact indicates opportunity)

Plot each risk in the appropriate cell where the probability and impact intersect
Step 3: Apply color coding

Color-code each risk based on its risk level:

    Red: High risk (requires immediate attention)
    Yellow: Moderate risk (monitor closely)
    Green: Low risk or opportunity (monitor or enhance)

This visual cue enables stakeholders to quickly assess the most critical risks and identify where to focus mitigation efforts.
Step 4: Save your work

Save your created risk matrix as Name_RiskMatrix.xlsx and keep it handy for the final project.
Summary

Congratulations on completing this Lab: Project Planning and Risk Analysis! These artifacts reflect your ability to break down complex architecture programs, identify dependencies, and mitigate strategic and technical risks in high-stakes enterprise environments.
Author

Parikshit Jain

