# Use Case Name: Submit Travel Insurance Claim

**Actor:** Customer  

**Precondition:** Customer has a valid insurance policy and necessary documents (receipts, medical reports, etc.).  

**Trigger:** Customer experiences an event covered by the travel insurance policy and wants to submit a claim.  

---

## Main Flow (Basic Path)
1. Customer logs in to the travel insurance portal.  
2. Customer navigates to the “Submit Claim” section.  
3. Customer selects the type of claim (e.g., medical, trip cancellation, lost luggage).  
4. Customer fills out the claim form with required details:  
   - Policy number  
   - Date of incident  
   - Description of the incident  
   - Amount claimed  
5. Customer uploads supporting documents (receipts, reports, proof of travel, etc.).  
6. Customer reviews all information and submits the claim.  
7. System generates a confirmation and a claim reference number.  
8. Customer receives an email confirmation with the claim details and reference number.  

---

## Alternative Flows
**A1: Missing documents**  
- If the customer fails to upload required documents, the system prompts to upload them before submission.  

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

## Use Case Flow Diagram (ASCII)

Customer
   |
   v
[Log in to Portal]
   |
   v
[Navigate to Submit Claim]
   |
   v
[Select Claim Type]
   |
   v
[Fill Claim Form]
   |
   v
[Upload Documents] ---> (Missing Docs?) ---> [Prompt to Upload] ---> [Fill Claim Form]
   |
   v
[Review & Submit]
   |
   v
[System Generates Claim Reference]
   |
   v
[Email Confirmation to Customer]










