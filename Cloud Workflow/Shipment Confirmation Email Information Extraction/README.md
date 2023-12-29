# Power Automate Workflow for Shipment Confirmation Email Data Extraction

## Overview
This workflow is specifically designed for Office 365 users to automate the process of extracting shipment information from emails. It is tailored to activate upon receiving emails from a specified vendor, filtered by the email's subject.

### Workflow Activation and Data Extraction:
- **Email Trigger**: Activates when a relevant email arrives in the Office 365 mailbox, identified by the vendor and subject filter.
- **Shipment Data Extraction**: Extracts key shipment details from the HTML body of the email, including:
  - Sales Order Number
  - Tracking Number (Track No)
  - Table Items (such as Item Description, Order Quantity, Ship Quantity)

### Data Processing and Output:
- **HTML Processing**: Transforms the email HTML content into a valid XML format suitable for data extraction.
- **XPath Utilization**: Employs XPath to accurately select the required fields from the processed HTML/XML content.
- **Data Composition**: Uses 'Select' and 'Compose' actions within Power Automate to compile the final shipment information.
- **CSV File Generation**: Saves the compiled data into a CSV format file for convenient use and storage.

## Implementation Guide
1. **Email Configuration**:
   - Define the criteria for the email trigger, focusing on vendor specifics and the email subject line.
2. **HTML to XML Conversion**:
   - Set up the workflow to convert email HTML content into a valid XML format.
3. **XPath Usage**:
   - Use xpath expression to extract the necessary fields.
4. **Workflow Customization**:
   - Tailor the 'Select' and 'Compose' actions to format and compile the shipment information.

## Prerequisites
- An active Office 365 mailbox.
- Understanding of HTML/XML conversion and XPath.
- Familiarity with Power Automate's 'Select' and 'Compose' actions.

## Connector Involved
- Office 365 Outlook
