# Invoice Data Dictionary

| Field | Meaning | Type | Required? | Source | Rule / Constraint | Example |
|---|---|---|---|---|---|---|
| Invoice ID | Unique system identifier for the invoice | Integer | Yes | System-assigned | Must be unique | 100245 |
| Invoice Number | Business invoice number | Text | Yes | System-assigned | Must be unique | INV-2026-00125 |
| Client Name | Name of the client being invoiced | Text | Yes | User-entered | Cannot be blank | ABC Mortgage |
| Invoice Date | Date of the invoice | Date | Yes | User-entered | Must be a valid date | 09/14/2026 |
| Service Description | Description of service or billable activity | Text | Yes | User-entered | Description required | Document Recording |
| Quantity | Number of billable units | Integer | Yes | User-entered | Must be greater than 0 | 2 |
| Unit Amount | Charge for each billable unit | Decimal | Yes | User-entered | Cannot be negative | 30.00 |
| Total Amount | Total invoice charge | Decimal | Yes | Derived/Calculated | Quantity × Unit Amount | 60.00 |
| Supporting Notes | Additional information about the invoice | Text | No | User-entered | Optional | Recording completed |
| Status | Current invoice state | Text | Yes | System-assigned | Draft, Submitted, Under Review, Approved, or Rejected | Under Review |
| Created At | Date/time invoice record was created | Date/Time | Yes | System-assigned | Recorded when invoice is created | 09/14/2026 9:15 AM |
| Submitted At | Date/time invoice was submitted | Date/Time | Conditional | System-assigned | Recorded when status changes to Submitted | 09/14/2026 10:30 AM |
| Reviewed At | Date/time invoice was reviewed | Date/Time | Conditional | System-assigned | Recorded when review occurs | 09/14/2026 1:15 PM |
| Reviewer ID | Identifies the reviewer or approver | Text | Conditional | System-assigned | Required when invoice is reviewed | EMP204 |
| Decision | Final review decision | Text | Conditional | System-assigned | Approved or Rejected | Approved |
| Decision Notes | Reviewer explanation or correction instructions | Text | No | User-entered | Used when additional explanation is needed | Approved as submitted |
