# User Stories and Acceptance Criteria

## Billing Employee

### User Story
As a billing employee, I want to create and submit an invoice so that it can be reviewed and approved for client billing.

### Acceptance Criteria
- Given that all required invoice information has been entered, when the billing employee submits the invoice, then the invoice status changes from Draft to Submitted.
- Given that required information is missing, when the billing employee attempts to submit the invoice, then the system prevents submission and identifies the missing information.

## Reviewer / Manager

### User Story
As a reviewer or manager, I want to review submitted invoices so that errors can be identified before final approval.

### Acceptance Criteria
- Given that an invoice has been submitted, when the reviewer begins the review, then the invoice status changes to Under Review.
- Given that an error is identified during review, when the reviewer rejects the invoice, then a rejection reason must be recorded and the invoice is returned for correction.

## Approver

### User Story
As an approver, I want to approve or reject reviewed invoices so that only accurate invoices complete the approval process.

### Acceptance Criteria
- Given that an invoice has completed review, when the approver approves it, then the invoice status changes to Approved.
- Given that the approver rejects an invoice, when the rejection is submitted, then the invoice status changes to Rejected and the rejection reason is recorded.
