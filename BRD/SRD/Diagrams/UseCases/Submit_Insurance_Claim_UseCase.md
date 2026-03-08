# Use Case Name: Submit Travel Insurance Claim

**Actor:** Customer  

**Precondition:** Customer has a valid insurance policy and necessary documents (receipts, medical reports, etc.).  

**Trigger:** Customer experiences an event covered by the travel insurance policy and wants to submit a claim.  

---

## Main Flow (Basic Path)
1. **Log in** – Customer logs in to the travel insurance portal.  
2. **Navigate to Submit Claim** – Customer selects the “Submit Claim” section.  
3. **Select Claim Type** – Customer chooses the type of claim (e.g., medical, trip cancellation, lost luggage).  
4. **Fill Claim Form** – Customer provides required details:  
   - Policy number  
   - Date of incident  
   - Description of the incident  
   - Amount claimed  
5. **Upload Documents** – Customer attaches supporting documents (receipts, reports, proof of travel, etc.).  
6. **Review & Submit** – Customer reviews all information and submits the claim.  
7. **System Confirmation** – System generates a confirmation and a claim reference number.  
8. **Email Notification** – Customer receives an email confirmation with claim details and reference number.  

---

## Alternative Flows
**A1: Missing documents**  
- If required documents are missing, the system prompts the customer to upload them before submission.  

**A2: Invalid policy**  
- If the policy number is invalid or expired, the system notifies the customer and prevents submission.  

**A3: System error**  
- If the system encounters an error during submission, it displays an error message and advises the customer to try again later.  

---

## Postconditions
- Claim is recorded in the system.  
- Customer receives confirmation and claim reference.  
- Claim is ready for processing by the insurance team.  

---

## Notes
- The system should validate file formats and sizes for uploads.  
- The claim reference number should be unique and trackable.  

---

## Use Case Flow Diagram (Branching ASCII)

                 +------------------+
                 |      Customer     |
                 +------------------+
                          |
                          v
                 +------------------+
                 |      Log in       |
                 +------------------+
                          |
                          v
                 +---------------------------+
                 | Navigate to Submit Claim  |
                 +---------------------------+
                          |
                          v
                 +------------------+
                 | Select Claim Type |
                 +------------------+
                          |
                          v
                 +------------------+
                 | Fill Claim Form   |
                 +------------------+
                          |
                          v
                 +------------------+
                 | Upload Documents |
                 +------------------+
                     /       \
          Missing? /           \ OK
                 /               \
        +------------------+     v
        | Prompt to Upload |   +------------------+
        +------------------+   | Review & Submit  |
                 |             +------------------+
                 +--------> Fill Claim Form
                          |
                          v
                 +------------------------------+
                 | System Generates Claim Ref # |
                 +------------------------------+
                          |
                          v
                 +------------------+
                 | Email Confirmation |
                 +------------------+



















