Travel Insurance Claim System – Entity Documentation

This document details all the entities in the Travel Insurance Claim System, including their attributes, relationships, and purpose.

1. Customer

Description: Represents the individual purchasing travel insurance and submitting claims.

Attributes:

Attribute	Type	Notes
Customer_ID	UUID / Integer	Primary Key
First_Name	String	Required
Last_Name	String	Required
Email	String	Unique, Required
Phone_Number	String	Optional
Date_of_Birth	Date	Optional
Address	String	Optional
Policy_ID	UUID / Integer	Foreign Key to Policy

Relationships:

1 Customer → 1..N Policies (A customer can have multiple insurance policies.)
1 Customer → 0..N Claims (A customer can submit multiple claims.)
2. Policy

Description: Represents an insurance policy purchased by a customer.

Attributes:

Attribute	Type	Notes
Policy_ID	UUID / Integer	Primary Key
Customer_ID	UUID / Integer	Foreign Key to Customer
Policy_Number	String	Unique
Start_Date	Date	Required
End_Date	Date	Required
Coverage_Type	String	e.g., Basic, Premium
Status	String	Active / Expired / Cancelled

Relationships:

1 Policy → 1 Customer
1 Policy → 0..N Claims
3. Claim

Description: Represents a travel insurance claim submitted by a customer.

Attributes:

Attribute	Type	Notes
Claim_ID	UUID / Integer	Primary Key
Policy_ID	UUID / Integer	Foreign Key to Policy
Customer_ID	UUID / Integer	Foreign Key to Customer
Claim_Date	Date	Required
Status	String	e.g., Submitted, Under Review, Approved, Rejected
Amount_Claimed	Decimal	Optional
Amount_Approved	Decimal	Optional

Relationships:

1 Claim → 1 Policy
1 Claim → 1 Customer
1 Claim → 0..N Documents
1 Claim → 0..N Claim_Assignments
4. Document

Description: Represents any supporting documents submitted with a claim.

Attributes:

Attribute	Type	Notes
Document_ID	UUID / Integer	Primary Key
Claim_ID	UUID / Integer	Foreign Key to Claim
File_Name	String	Required
File_Type	String	e.g., PDF, JPG
Upload_Date	DateTime	Required
Status	String	Pending / Approved / Rejected

Relationships:

1 Document → 1 Claim
5. Adjuster

Description: Represents an insurance adjuster who reviews and processes claims.

Attributes:

Attribute	Type	Notes
Adjuster_ID	UUID / Integer	Primary Key
First_Name	String	Required
Last_Name	String	Required
Email	String	Unique
Phone_Number	String	Optional

Relationships:

1 Adjuster → 0..N Claim_Assignments
6. Claim_Assignment

Description: Links claims to adjusters assigned to process them.

Attributes:

Attribute	Type	Notes
Assignment_ID	UUID / Integer	Primary Key
Claim_ID	UUID / Integer	Foreign Key to Claim
Adjuster_ID	UUID / Integer	Foreign Key to Adjuster
Assigned_Date	DateTime	Required
Status	String	Pending / In Progress / Completed

Relationships:

1 Claim_Assignment → 1 Claim
1 Claim_Assignment → 1 Adjuster
Notes / Business Rules
A Customer can hold multiple Policies but a Policy belongs to only one Customer.
A Claim must belong to exactly one Policy and one Customer.
Documents are optional for a Claim but may be required depending on the claim type.
Adjusters can handle multiple Claims, and a Claim may be assigned to multiple Adjusters.


