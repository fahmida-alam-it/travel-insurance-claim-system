# Travel Insurance Claim System

## Project Overview
The Travel Insurance Claim System allows customers to submit insurance claims online and enables insurance agents to review, process, and approve or reject claims.

The system helps automate the claim process, reduce manual paperwork, and improve claim processing efficiency.

---

## System Objectives

- Allow customers to submit travel insurance claims online
- Upload supporting documents (receipts, medical reports)
- Enable agents to review and approve claims
- Track claim status throughout the process
- Maintain secure policy and claim records

---

## System Architecture

The system consists of the following components:

- Customer Web Portal
- Claim Management System
- Policy Database
- Claims Database
- Insurance Agent/Admin Interface

See the detailed diagram:

BRD/SRD/Diagrams/System_Overview.md

---

## Claim Process Overview

The claim process follows these steps:

1. Customer logs into the portal
2. Customer submits a travel insurance claim
3. Customer uploads required documents
4. System validates the claim information
5. Insurance agent reviews the claim
6. Claim is approved or rejected
7. Customer receives notification

Diagram available here:

BRD/SRD/Diagrams/Claim_Process_Overview.md

---

## Use Cases

The system supports several main use cases.

## Repository Structure

## Repository Structure – Travel Insurance Claim System

## Repository Structure – Travel Insurance Claim System

```
travel-insurance-claim-system
│
├── README.md
├── LICENSE.md
│
├── BRD
│   ├── Business_Requirements.md
│   │
│   └── SRD
│       ├── System_Requirements.md
│       │
│       └── Diagrams
│           ├── README.md
│           ├── System_Overview.md
│           ├── Claim_Process_Overview.md
│           ├── System_Architecture.md
│           ├── Claim_Data_Model.md
│           ├── Master_Index_Diagrams_2026-02-25.docx
│           ├── Process_Diagrams
│           │
│           ├── ER Diagrams/
│           ├── Flowcharts/
│           ├── UML Diagrams/
│           └── Wireframes_Mockups/
│
│           └── UseCases
│               ├── README.md
│               ├── Submit_Insurance_Claim_UseCase.md
│               ├── Register_Create_Account.md
│               ├── View_Policy_Details.md
│               ├── Upload_Claim_Documents.md
│               └── Approve_Process_Claims.md
│
├── Screenshots/
├── Tests/
└── docs/
```

## System Diagrams & Use Case Map
```
│
├── ER Diagrams
│   ├── Customer_ER_Diagram.md
│   ├── Claims_ER_Diagram.md
│   └── Policy_ER_Diagram.md
│
├── Flowcharts
│   ├── Claim_Submission_Flowchart.md
│   ├── Claim_Approval_Flowchart.md
│   └── Payment_Process_Flowchart.md
│
├── UML Diagrams
│   ├── UseCase_UML.md  ──► Linked to UseCases/UseCase_*.md
│   ├── Sequence_UML.md  ──► Shows step-by-step processes in Flowcharts
│   └── Class_UML.md     ──► Based on ER Diagrams
│
├── Wireframes_Mockups
│   ├── Dashboard_Wireframe.md  ──► Reflects key system functions
│   ├── Claim_Form_Wireframe.md ──► Linked to Claim Submission Flowchart
│   └── Mobile_View_Mockup.md   ──► For mobile interface of system
│
├── System_Overview.md       ──► Provides high-level summary of all components
├── Claim_Process_Overview.md ──► Connects Flowcharts + Use Cases
├── System_Architecture.md   ──► Shows technical architecture integrating all diagrams
├── Claim_Data_Model.md      ──► Detailed ER + Class Diagram mapping
│
├── Master_Index_Diagrams_2026-02-25.docx
└── Process_Diagrams/
```

| Use Case | Description |
|--------|-------------|
| Register / Create Account |
| Submit Insurance Claim | 
| Customer submits a travel insurance claim |
| Upload Claim Documents |
| View Policy Details | 
| Approve / Process Claims | 

Use cases are located in:

BRD/SRD/Diagrams/UseCases/


---

## Technologies (Example)

- Web Portal
- Database Management System
- Cloud Infrastructure
- Document Storage System

---

## Author

Project developed as part of a **System Analysis and Design documentation project**.

