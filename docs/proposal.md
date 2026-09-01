# Invoice Creation, Submission & Approval System
## Capstone Project Proposal

### Project Overview
The Invoice Creation, Submission & Approval System is designed to provide a structured process for creating, reviewing, approving, and tracking invoices. The system will allow an invoice to move through a defined workflow from initial creation through final approval.

### Business Problem
Invoice processing can involve multiple steps and employees, making it difficult to track whether an invoice has been completed, submitted for review, approved, or requires corrections. Without a centralized process, invoice status and required actions may not always be clear. This system will provide a defined workflow that allows users to create invoices and track them throughout the approval process.

### Stakeholders
- **Billing Employee** – Creates invoices, enters charges, submits invoices, and makes corrections when necessary.
- **Reviewer/Manager** – Reviews submitted invoices for completeness and accuracy.
- **Approver** – Makes the final decision to approve or reject an invoice.

### Main Transaction
The main transaction is the creation and processing of an invoice from initial creation through approval.

The normal transaction flow is:

Draft → Submitted → Under Review → Approved

If corrections are required:

Under Review → Rejected → Draft → Submitted → Under Review → Approved

### Functional Requirements
1. The system shall allow a billing employee to create a new invoice.
2. The system shall allow the billing employee to enter invoice information, including the client, invoice date, services or charges, and amounts.
3. The system shall automatically calculate the total invoice amount based on the charges entered.
4. The system shall allow a completed invoice to be submitted for review and approval.
5. The system shall allow an authorized reviewer or approver to approve or reject a submitted invoice.
6. The system shall display and track the current status of each invoice.
7. The system shall allow a rejected invoice to be corrected and resubmitted.

### Nonfunctional Requirements
1. The system shall restrict invoice approval functions to authorized users.
2. The system shall maintain a record of important invoice actions and status changes for tracking and accountability.

### Business Rules
1. An invoice must include a client, invoice date, and at least one charge before it can be submitted.
2. All invoice charges must have an amount greater than $0.
3. The invoice total must equal the sum of all charges included on the invoice.
4. Only invoices with a Draft or Rejected status may be edited by the billing employee.
5. Only an authorized reviewer or approver may approve or reject a submitted invoice.
6. A rejected invoice must include a reason for rejection or correction before it is returned to the billing employee.
7. An approved invoice cannot be changed unless it is returned to an authorized user for correction.

### Invoice States
- **Draft** – The invoice is being created and may still be edited.
- **Submitted** – The billing employee has completed and submitted the invoice.
- **Under Review** – The invoice is being reviewed for accuracy.
- **Approved** – The invoice has passed review and has been approved.
- **Rejected** – The invoice requires corrections before it can be approved.

### Project Scope

#### Must Have
- Invoice creation
- Entry of invoice charges and amounts
- Automatic invoice total calculation
- Invoice submission
- Review and approval/rejection
- Invoice status tracking
- Correction and resubmission of rejected invoices

#### Should Have
- Invoice search
- Invoice history
- Reviewer comments or rejection reasons

#### Could Have
- Dashboard showing invoices by status
- Additional search and filtering options
- Status-change notifications

#### Won't Have This Semester
- Sending actual invoices to clients
- Processing real payments
- Integration with accounting or payment systems
- Use of real client or company financial data

### Project Goal
The goal of this project is to build a manageable transaction-processing system that demonstrates how an invoice can be created, validated, submitted, reviewed, approved or rejected, corrected when necessary, and tracked throughout its lifecycle.
