# Assignment Overview: Data Infrastructure

在本模組中，您將設計一個資料流程圖，展示如何將分散的銀行資料系統整合到一個統一的企業資料架構中。您將學習如何可視化關鍵資料來源與安全合規的 ETL 管道的端到端集成，以滿足審計和監管要求。
任務
任務 1：定義資料流元件

開啟 Lucidchart 或您常用的圖表繪製工具。使用標準資料流程圖符號來表示實體（CRM、核心銀行系統）、流程（ETL 作業）、資料儲存（暫存層、資料倉儲）以及帶有標籤的箭頭的資料流。
任務 2：建立資料整合的資料流程圖

先從核心外部資料來源（CRM、貸款管理系統、核心銀行系統、交易日誌）著手。建立 ETL 管道階段（提取、轉換、載入）模型。展示資料驗證點、稽核追蹤標記，並新增加密和資料脫敏的註釋，以確保符合隱私法規。
任務 3：檢查清單驗證

確保您的資料流程圖符合以下標準：包含所有核心系統、模組化 ETL 元件、精確的暫存和倉儲層、明確的資料安全措施（包括脫敏和加密）、透過稽核日誌實現可追溯性，以及支援監管報告和分析需求。 

---

Assignment Overview: Data Infrastructure

Estimated time: 4 minutes
Introduction

In this module, you will design a data flow diagram illustrating the consolidation of fragmented banking data systems into a unified enterprise data architecture. You'll learn to visualize the end-to-end integration of critical data sources with secure, compliant ETL pipelines that support auditability and regulatory needs.
Tasks
Task 1: Define the data flow components

Open Lucidchart or your preferred diagramming tool. Use standard data flow diagram symbols to represent entities (CRM, Core Banking), processes (ETL jobs), data stores (staging layer, warehouse), and data flows with labeled arrows.
Task 2: Create a data flow diagram of data integration

Start with core external data sources (CRM, Loan Management, Core Banking, Transaction Logs). Model the ETL pipeline stages (Extract, Transform, Load). Display data validation points, audit trail markers, and include annotations on encryption and data masking to ensure compliance with privacy regulations.
Task 3: Checklist validation

Ensure your data flow diagram meets criteria such as the inclusion of all core systems, modular ETL components, precise staging and warehouse layers, explicit data security measures (including masking and encryption), traceability through audit logs, and support for regulatory reporting and analytics needs.
Deliverables

In this module, you will work on the following deliverables:

    Retail_Data_Infrastructure_DataFlowDiagram.png or .pptx file illustrating the consolidated data architecture and ETL pipeline
    Data_Infra_Validation_Checklist.xlsx (optional), confirming that key validation criteria for data integration, security, and compliance are met
    Submission tip: include a legend and use color-coding to enhance readability and clarity

---

Lab: Data Flowchart for the Consolidation of Data Infrastructure
Estimated time: 15 minutes
Learning objectives:

After completing this lab, you will be able to:

    Create a data flow diagram (DFD) that shows end-to-end integration of banking systems
    Identify critical data sources and how they feed into the central enterprise data warehouse
    Model ETL stages, staging areas, and data validation checkpoints
    Illustrate data privacy, encryption, and regulatory compliance checkpoints
    Validate the created DFD diagram that supports auditability, data lineage, and retention policies

Required tools

    Lucidchart
    Draw.io
    Microsoft PowerPoint

Note: You are advised to use the free version of the above tools. If you plan to upgrade these tools, you are responsible for any applicable charges.
Introduction

In modern banking, a visual blueprint represents how a bank's scattered data systems can be unified into a single, well-governed data infrastructure. The diagramming tools will help you to map data movement through extraction, transformation, and loading (ETL) stages while maintaining security, compliance, and traceability.
Scenario overview

In a digital core transformation for a retail bank, one of the most critical goals is to consolidate fragmented data systems, including CRM, loan management, core banking, and transaction logs, into a unified enterprise data architecture.

This lab simulates a real-world deliverable that visualizes how multiple siloed data sources are integrated via a secure, traceable ETL pipeline and stored in a centralized, compliance-ready data layer.
Key data sources
Source system 	Description
CRM 	Customer profiles and contact history
Loan management 	Loan applications, repayments, and delinquencies
Core banking system 	Account balances and customer IDs
Transaction logs 	Card payments, transfers, and ATM usage
Tasks to be performed

For this lab, download the Template_Data Flowchart for the Consolidation for Data Infrastructure (Word or PDF) to insert your responses.
Task 1: Define the data flow components

In this task, you will identify and set up all the required building blocks to create a data flowchart.
Step 1: Open diagramming tool

Open a preferred diagramming tool, such as Lucidchart, draw.io, PowerPoint, or Word SmartArt.
Step 2: Review symbols

Validate the standard DFD symbols:

    Entities (External Systems): Represent data sources, for example, CRM and Core Banking
    Processes (ETL Jobs): Represent data movement and transformation, for example, Extract, Validate, and Load
    Data Stores: Represent storage layers, for example, the Staging Layer and the Data Warehouse
    Data Flows: Use labeled arrows to indicate the direction and nature of data movement

Examples of DFD symbols
Symbol type 	Symbol shape (as seen in Lucidchart/Draw.io/PowerPoint) 	Meaning/Use 	Example in banking context
Entity (External System) 	Rectangle 	Represents an external data source or system that provides or receives data. 	CRM system, loan management system, core banking, and transaction logs
Process (ETL Job/Transformation) 	Rounded Rectangle or Circle 	Represents data transformation, movement, or computation (ETL steps). 	Extract Data, Transform Data, Validate, and Load to Staging
Data Store (Database/Repository) 	Two Parallel Lines or Cylinder Shape 	Represents storage where data is held temporarily or permanently. 	Staging Area, Enterprise Data Warehouse, and Archive Store
Data Flow (Movement of Data) 	Arrow (Labeled) 	Indicates the direction of data flow between entities, processes, or stores. 	CRM → Extract → Transform → EDW (label arrows as “Customer Data”, “Loan Data”, etc.)
Validation/Audit Checkpoint (Optional) 	Diamond 	Represents decision or validation steps used in some extended DFDs. 	Data Validation Complete?, Audit Log Created?
Task 2: Create a data flowchart

In this task, you will design a complete flow of how data moves from source systems to the enterprise data warehouse.
Step 1: Add external data sources

Incorporate external data sources from the left side of the diagram.

    CRM
    Loan management system
    Core banking
    Transaction logs

Step 2: Create the ETL pipeline

Add process boxes labeled below to create the ETL pipeline, center in the diagram.

    Extract: Pull data from each source system
    Transform: Standardize formats, remove duplicates, and validate integrity
    Load: Move cleaned data to the staging layer and then to the enterprise data warehouse

Step 3: Include data validation and audit points

    Add symbols or notes showing validation checkpoints after each ETL stage
    Include audit trains, for example, Log ETL timestamp for each batch

Step 4: Annotate security and compliance controls

Add annotations such as:

    "Encrypted during transmission (TLS 1.3)"
    "ETL timestamp logs stored for audit compliance"
    "Personally Identifiable Information (PII) masked in staging"

Step 5: Show final output

End with a single enterprise data warehouse (EDW) output node from the right side of the diagram, including:

    Regulatory reporting
    Compliance dashboards
    Executive BI/Analytics systems

Step 6: Customize the diagram

    Use color coding. For example
        Blue color for sources
        Green color for ETL
        Orange color for storage
    Align elements from left (Source) to right (Output)

Step 7: Save your work

Export the file and save it as a retail_banking_data_infrastructure as an image or a PPT. Keep this diagram ready for the final project.
Task 3: Review data flowchart

Review the created data flowchart for completeness, accuracy, and alignment with relevant compliance requirements with the checklist below.

    All core data systems are represented (CRM, core banking, etc.)
    ETL components are modular and logically ordered
    Staging and warehouse layers are clearly identified
    Data security (masking, encryption) is explicitly mentioned
    Traceability elements like audit logs are included
    Outputs support regulatory, operational, and analytical needs

Summary

Congratulations on completing the Lab: Data Flowchart for Consolidation of Data Infrastructure! In this lab, you've created a data flow diagram that visualizes the considerations of a retail banking system into a centralized enterprise data warehouse. The completed data flowchart illustrates a structured and traceable data movement that supports analytics, reporting, and regulatory objectives in a modern banking environment.

---

