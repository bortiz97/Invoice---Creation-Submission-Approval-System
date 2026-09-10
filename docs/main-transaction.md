# Main Transaction

## Transaction Event
A billing employee creates and submits an invoice for review and approval.

## Trigger
A completed service or billable activity is ready to be invoiced to the client.

## Inputs
- Client information
- Invoice date
- Invoice number
- Service or charge details
- Amounts
- Supporting notes or documentation, when needed

## System Actions
The system:
- Validates that required invoice information is present
- Creates the invoice record
- Assigns the invoice status
- Routes the invoice through review and approval
- Records status changes and decisions

## Possible Outcomes
The invoice may:
- Remain in Draft
- Be Submitted
- Move to Under Review
- Be Approved
- Be Rejected and returned for correction

## Official Record
The system stores the invoice number, client, charges, status, timestamps, reviewer or approver actions, and final decision.
