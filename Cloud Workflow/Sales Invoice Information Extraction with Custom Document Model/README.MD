# Power Automate Workflow for Email Invoice Attachment Processing

## Overview
This workflow is designed for Office 365 users to automate the extraction of information from PDF attachments in emails. It is triggered by specific criteria in incoming emails from a designated vendor.

### Workflow Activation:
- **Email Trigger**: Activates when an email is received in the Office 365 mailbox.
- **Vendor and Subject Filter**: Checks if the email is from a specified vendor and meets the subject line criteria.

### Data Extraction and Processing:
- **Attachment Extraction**: Extracts PDF attachments from qualifying emails using a pre-trained document model.
- **Data Fields Extraction**: Focuses on extracting table-format information from invoices, including:
  - Order Number
  - Product Number
  - Shipped Count
  - Tracking Number
- **Data Aggregation**: Appends extracted information into an array-type variable within an 'Apply to Each' action.
- **CSV File Creation**: Compiles and saves the table information in a CSV format file.

## Implementation Steps
1. **Email Configuration**:
   - Set up email criteria for the workflow trigger, including vendor-specific details and subject line filters.
2. **Document Model Setup**:
   - Configure the pre-trained document model for PDF extraction.
3. **Workflow Customization**:
   - Adjust the workflow to suit your specific data extraction and aggregation needs.

## Prerequisites
- Access to an Office 365 mailbox.
- Setup of a pre-trained document model for PDF data extraction.
- Basic understanding of Power Automate workflows.

## Additional Information
For further details on setup, customization, and troubleshooting, refer to the subsequent sections of this documentation.

---

Feedback and suggestions for workflow enhancement are always welcome!
