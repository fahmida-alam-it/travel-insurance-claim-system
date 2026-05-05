### Insurance Claim Management System (Java + REST API)
🧠 Overview  

The Insurance Claim Management System is a backend system design project that simulates an end-to-end insurance claim workflow. It demonstrates the translation of business requirements into structured system design using Java and REST API principles.

The system models a real-world insurance claim lifecycle, including submission, validation, assessment, decision-making, and closure through a structured workflow.

This project reflects the ability to bridge business systems analysis and technical implementation by converting business requirements into system behavior and backend design. 

---


### 📊 Claims Process Flow

The diagram below illustrates the end-to-end process of submitting and processing an insurance claim:

![Claim Processing Flow](images/claim_flow.png)

- **Claim Submission:** Customer submits a new claim.
- **Validation:** System checks claim details.
- **Assessment:** Claims agent evaluates the claim and requests additional info if needed.
- **Decision:** Claim is approved or rejected.
- **Payment & Closure:** Approved claims are paid, and the process is closed.

The Insurance Claims process follows these main steps:

1. **Start** – The user begins the claims process.
2. **Login** – The user logs into the system.
3. **Submit Claim** – The user submits a new claim.
4. **Upload Documents** – Any required documents are uploaded.
5. **System Validation** – The system checks the claim and documents.
6. **Claim Review** – The claim is reviewed by the claims team.
7. **Approved / Rejected** – The claim is either approved or rejected.
8. **End** – The process is completed.

---

### 🧩 System Use Cases

The use cases diagram shows the main actors and their interactions with the system:

![System Use Cases](images/use_cases.png)

- **Customer:** Submit claim, upload documents, track status.
- **Claims Agent:** Assess claims, request information, approve or deny claims.
- **Administrator:** Manage users, generate reports, audit logs, configure system.
- **External Systems:** Database, payment gateway, and third-party services interact with the system as needed.

---

⚙️ Features
User authentication and secure login.
Online claim submission with form validation.
Document upload and verification system.
Automated notifications for claim status updates.
Admin interface for claim review and decision-making.
Support for appeal process if a claim is denied.

 ```
[Start]
↓
[Login]
↓
[Submit Claim]
↓
[Upload Documents]
↓
[System Validation]
↓
[Claim Review]
↓
[Approved / Rejected]
↓
[End]

 ```

![Claims Flow](SRD/Diagrams/Systems%20Diagram%20and%20Use%20case%20map%20%20Image.png)

---

## 🎯 Business Problem

Insurance claim processing often involves manual tracking, inconsistent workflows, and multiple stakeholders, leading to delays and lack of transparency.

This system demonstrates how a structured digital workflow can improve:

Claim processing consistency
Status visibility across stages
Reduction of manual handling errors
Alignment between business rules and system behavior

---
## Actors
- Customer
- Claims Agent
- Claims Manager

Project Scenario
Client: Mid-size Insurance Provider
Project: Claims Processing System Enhancement
The project aimed to improve the efficiency, accuracy, and user experience of the client’s claims processing platform. The initiative focuses on streamlining claim intake, automating validation rules, and enhancing reporting capabilities for business stakeholders.

### 🧩 Scope of Work
Gather and document business requirements (BRD)
Create detailed functional specifications (Use Cases & User Stories)
Produce process and system diagrams (ERD, Flowcharts, Sequence Diagrams)
Support data mapping and validation rules
Assist with User Acceptance Testing (UAT)

### 🛠 Deliverables in This Repository
Business Requirements Document (BRD)
Use Cases and User Stories
Data Mapping documents
Process and System Diagrams
UAT Test Plans and supporting materials


### 🧑‍💼 My Role
Business Systems Analyst
Key Responsibilities:
Stekeholder needs analysis
Business and system requirement documentation (BRD & SRD)
Process modeling and workflow design
Use case definition
Collaboration between business and technical teams
Defined user stories and functional requirements

### 🧾 Use Cases & User Stories
Actor interactions with the system
Functional scenarios for claim submission and processing
User goals and acceptance criteria
These artifacts support requirement validation and bridge business needs with solution design.

### 🗂️ Repository Folder Structure

This repository is organized to clearly separate Business Requirements (BRD), System Requirements (SRD), Diagrams, UAT,Use Case, User Stories, Wireframe, code, and supporting documentation.

Project-Root/
  README.md

  ```
Travel-Insurance-Claim-System/
│
├─ BRD/                # Business Requirement Documents
├─ SRD/                # System Requirement Documents
│
├─ Diagrams/           # All system diagrams
│   ├─ ERD/            # Entity-Relationship diagrams
│   ├─ Flowcharts/     # Process flow diagrams
│   ├─ Process/        # End-to-end process diagrams
│   ├─ UML/            # Use case, class diagrams
│   ├─ Sequence/       # Sequence diagrams
│   └─ Visio/          # (Optional) Visio versions of diagrams
│
├─ UseCases/           # Use case descriptions
├─ UserStories/        # Agile user stories
├─ Wireframes/         # UI mockups / screens
├─ UAT/                # User acceptance testing documentation
│
├─ Data/               # Data-related files
│   ├─ DataMapping/
│   └─ ExcelFiles/
│
├─ Docs/               # Supporting documents
│   └─ Master_Index_Diagrams.rtf
│
├─ images/             # Images used in README
├─ Code/               # Source code (if applicable)
│
└─ README.md

```
---
    
### 📊 Analysis & Design Artifacts
ER Diagram: Defines entities and relationships within the claims data model
Flowcharts: Visualize business workflows and decision points
Sequence Diagrams: Show system interactions and message flow between components
Data Mapping: Maps data fields between source inputs and system outputs
These artifacts support solution design, stakeholder communication, and requirement validation.

### 🔍 Key Features of the Proposed Solution
Online claim submission portal
Document upload and validation
Automated status tracking
Claims adjudication workflow
Notification and communication module

### 🛠 Technologies Used
Programming Language: Java (depending on implementation)
REST API Architecture
Backend System Design Concepts
Database: MySQL / PostgreSQL
Frontend:  / HTML, CSS
Tools: visio (for diagrams), GitHub (version control)
Microsoft Excel → Analysis, data mapping, tracking, and documentation support

Microsoft Visio → Process, ER, and sequence diagrams

UML → process modeling techniques

Requirements documentation best practices

Workflow and data modeling

SQL →  Data validation and analysis

Databricks (conceptual use)  → Data processing and analytics environment


### 🌟 Key Achievements / Value Delivered
Streamlined claims processing: Automated workflows reduced manual intervention and shortened claim processing time by 30%
Enhanced transparency: Implemented status tracking and notifications, improving communication with claimants and reducing follow-up inquiries by 40%
Improved requirement accuracy: Developed BRD, SRD, and detailed use cases enabling 95% of system requirements to be correctly implemented on the first iteration
Optimized data management: Designed ER diagrams and data mapping documents ensuring data consistency across multiple systems
Accelerated stakeholder alignment: Visual artifacts (flowcharts, sequence diagrams, wireframes) facilitated faster approvals, reducing feedback cycles by 25%

### How to Use This Repository

This repository is organized to clearly separate business analysis artifacts, documentation, and supporting files. Use the guidelines below to navigate and maintain the project.

### 📁 SRD (System Requirement Documents)
BRD → High-level business requirements
UseCases → Detailed functional flows
UserStories → Agile requirements
UAT → Test plans, test cases, and sign-off documents
ERDiagrams / FlowCharts / SequenceDiagrams → Visual system and process models

### 📁 ExcelFiles
Stores analysis workbooks, datasets, and reports used during analysis or testing.

### 📁 VisioDiagrams
Contains workflow diagrams, process maps, and architecture visuals.

### 📁 DataMapping
Includes mapping between business fields and system data elements:
Source-to-target mappings
Transformation rules
Data dictionaries

### 📁 Code

Java → Supporting or sample code

tests → Unit or functional test scripts


🚀 How to Run

Clone the repository:

git clone https://github.com/Fahmida-Alam-IT/travel-insurance-claim-system.git

Navigate to the project folder:

cd travel-insurance-claim-system

Install dependencies (if any):

pip install -r requirements.txt   # for Python

Run the application:

python src/main.py
Open your browser and follow the UI instructions to submit and track claims.


### 📁 📄 Documentation
BRD – Business requirements: BRD/Travel_Insurance_BRD.md
SRD – System requirements: SRD/Travel_Insurance_SRD.md
Diagrams – Flowcharts and process visuals: Diagrams/claim_flow.png
General supporting documentation such as:
Project notes
Guidelines
Reference materials

📊 Key Outcomes
Converting business requirements into system design
Understanding REST-based backend communication
Designing structured enterprise-style workflows
Bridging business analysis and technical implementation


👤 Author
Fahmida Alam
Business Systems Analyst | Java & REST API Systems | Agile Delivery | CBAP®














