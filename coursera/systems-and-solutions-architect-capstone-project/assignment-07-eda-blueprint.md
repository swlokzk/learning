# Assignment Overview: EDA Blueprint

Assignment Overview: EDA Blueprint

Estimated time: 2 minutes
Introduction

The retail bank is adopting an Event-Driven Architecture (EDA) to enable real-time transaction monitoring, fraud detection, and immediate customer notifications. This module guides you through designing a simplified EDA blueprint depicting event flow, security measures, and reliability features.
Tasks
Task 1: Identify EDA components

Recognize and describe event producers, brokers, and consumers involved in Retail Bank's real-time banking system, focusing on transaction sources, event routing, and alerting services.
Task 2: Design EDA architecture diagram

Create a clear diagram illustrating the event flow from producers through brokers to consumers, including retry mechanisms, dead-letter queues, and security checkpoints (such as TLS encryption).
Task 3: Develop an event mapping table

Map event types to corresponding producers, topics, and consumers in a concise table for easy reference and clarity in message routing within the system.
Task 4: Verify EDA architectural elements

Use a mini-checklist to confirm inclusion of key EDA features such as brokers, retry logic, dead-letter queues, multiple producers, and labeled security tags for data in transit.
Deliverables

In this module, you will work on the following deliverables:

    A simplified EDA architecture diagram (PowerPoint or PNG format) showing event flow and security elements
    An event mapping table (Word document) linking event types to producers, topics, and consumers
    An optional mini-checklist (Excel) verifying critical architectural components and security features

---

Lab: Design EDA Blueprint
Estimated time: 15 minutes
Learning objectives

After completing this lab, you will be able to:

    Identify the role of event producers, brokers, and consumers in real-time banking
    Classify key event types such as transaction completion, suspicious activity, or low balance alerts
    Sketch a simple event routing flow, including retry handling and dead-letter queues
    Identify the suitable place for security and reliability in the EDA model
    Produce a visual and a short table that explains each component

Required tools

To open the links below, right click on the link, and select Open in new tab.

    Lucidchart
    Draw.io
    Microsoft PowerPoint

Note: You are advised to use the free version of the above tools. If you plan to upgrade these tools, you are responsible for any applicable charges.
Introduction

An event-driven architecture (EDA) blueprint is a visual representation of how systems communicate through real-time event flows. It helps designers to understand relationships between producers, consumers, and brokers. In this lab, you'll create a simplified EDA blueprint to represent how key banking components interact through event channels for timely notifications, fraud detection, and other critical operations.
Scenario

A retail bank wants to enable real-time notifications and fraud monitoring for its digital banking customers. To achieve this, the bank plans to implement a basic event-driven architecture (EDA) that listens to events from transaction systems and routes them to various services, such as fraud detection or alerting systems.

In this lab, you'll create a simplified architecture diagram that maps out how events are produced, transferred, and consumed within the bank's systems.
Tasks to be performed
Task 1: Identify the components

In this task, you will identify and define the main components of the EDA model.
Step 1: Open diagramming tool

Open a preferred diagramming tool, such as Lucidchart, draw.io, PowerPoint, or Word SmartArt.
Step 2: Create labeled boxes for each category

    Event producers
        Core Banking System
        ATM or POS Systems

    Event broker (middle layer)
        Apache Kafka or IBM MQ (as a placeholder icon labeled "Broker")
        Handles topic-based routing and buffering

    Event consumers
        Fraud Detection System
        Notification Service (SMS, Email)

    Security and monitoring
        TLS (data in transit)
        Role-based Access
        Retry logic and DLQ (Dead Letter Queue)

Task 2: Create the EDA diagram

Begin by creating a simplified, clear EDA blueprint that shows the event flow between producers, brokers, and consumers to make the flow easy to follow.
Step 1: Arrange the diagram

    On the left side of your canvas, add a label box 'Event producer (Core banking system and ATM/POS systems)'
    At the center, add 'Event broker (Kafka or IBM MQ with topics labeled /alerts, /fraud, /balance)'
    At the right, add 'Event consumers (Fraud detection, notification, and SMS service)'

Step 2: Draw arrows

Show data flow from

    Each producer to the broker
    The broker to each relevant consumer

Step 3: Add visuals

    Label arrows with topic names (/alerts, /fraud)
    Add a retry path labeled with '3 attempts' note
    Add a small data letter queue (DLQ) box for failed messages
    Place a TLS tag near message arrows to show secure communication

Step 4: Save your work

Export the created EDA diagram and save it as SimplifiedEDAdiagram.pdf. Keep this diagram handy for the final project.
Task 3: Create event mapping table

In this task, you will document how events are produced, routed, and consumed.
Step 1: Download the template

Download the Template_Event Mapping (Word or PDF) and open it.

Note: To download the template, right click on the link, and select Open in new tab.
Step 2: Fill in the details

Review the EDA diagram and fill in the details for the events, such as transaction complete, high-risk activity, low-balance warning, and so on, in the template.
Step 3: Save your work

Save this template as Event mapping in Word or PDF format and keep it ready for the final project.
Task 4: Review EDA diagram

Ensure that your created design meets the following requirements:

    Uses a broker for message delivery
    Includes retry or DLQ concept
    Includes at least two producers
    Includes TLS or security tag
    Diagram is labeled and readable

Summary

Congratulations on completing the Lab: Design EDA Blueprint! In this lab, you've built a clear understanding of how events move through banking systems, from producers to consumers. You've created an EDA blueprint using DLQ and security layers, ensuring reliability and safety in event processing. The resulting EDA blueprint demonstrates how banks can achieve responsive, scalable, and fault-tolerant real-time operations.

---
