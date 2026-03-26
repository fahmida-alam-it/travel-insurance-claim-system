# ER Diagrams – Travel Insurance Claim System

This folder contains the **Entity-Relationship (ER) diagrams** for the Travel Insurance Claim System. These diagrams provide a visual representation of the system's data model, including entities, attributes, and relationships between them.

---

## Purpose

The ER diagrams help:

- Understand the structure of the travel insurance claim database.
- Visualize relationships between key entities such as **Claims, Customers, Policies, Payments, and Documents**.
- Serve as a reference for developers, business analysts, and stakeholders during system design and implementation.

---

## Key Entities and Attributes

### 1. **Customer**
- **Description:** Represents an individual purchasing or holding an insurance policy.
- **Key Attributes:** 
  - Customer_ID (PK)
  - Name
  - Date_of_Birth
  - Contact_Info
  - Address
- **Relationships:** 
  - Can have multiple **Policies**.
  - Can submit multiple **Claims**.

### 2. **Policy**
- **Description:** Details of a travel insurance plan purchased by a customer.
- **Key Attributes:** 
  - Policy_ID (PK)
  - Policy_Type
  - Start_Date
  - End_Date
  - Premium_Amount
  - Customer_ID (FK)
- **Relationships:** 
  - Linked to a single **Customer**.
  - Can cover multiple **Claims**.

### 3. **Claim**
- **Description:** Represents a claim submitted by a customer under a policy.
- **Key Attributes:** 
  - Claim_ID (PK)
  - Claim_Date
  - Status (e.g., Submitted, Approved, Rejected)
  - Claim_Amount
  - Policy_ID (FK)
  - Customer_ID (FK)
- **Relationships:** 
  - Linked to a **Policy** and a **Customer**.
  - May have multiple **Documents** and **Payments** associated.

### 4. **Document**
- **Description:** Files or attachments supporting a claim, such as receipts or medical reports.
- **Key Attributes:** 
  - Document_ID (PK)
  - Document_Type
  - File_Name
  - Upload_Date
  - Claim_ID (FK)
- **Relationships:** 
  - Associated with a single **Claim**.

### 5. **Payment**
- **Description:** Tracks payment transactions related to claims.
- **Key Attributes:** 
  - Payment_ID (PK)
  - Payment_Date
  - Amount
  - Payment_Method
  - Claim_ID (FK)
- **Relationships:** 
  - Linked to a single **Claim**.

### 6. **Agent (Optional)**
- **Description:** Represents insurance agents who process claims.
- **Key Attributes:** 
  - Agent_ID (PK)
  - Name
  - Contact_Info
- **Relationships:** 
  - Can be assigned to multiple **Claims** for processing.

---

## Contents

| File Name | Description |
|-----------|-------------|
| `Claim_ER_Diagram.png` | Main ER diagram showing all entities, their attributes, and relationships. |
| `Claim_ER_Diagram.png.png` *(if exists)* | Duplicate file – consider removing. |

---

## Notes

- The ER diagrams are part of the **system design documentation** and complement the BRD and SRD.
- Use these diagrams and descriptions as a reference when creating database schemas or integrating with other modules.
- Keep diagrams and entity descriptions updated whenever business rules or data models change.
