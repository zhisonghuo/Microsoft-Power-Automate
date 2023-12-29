# Power Automate Workflow for Certificate Data Extraction

## Overview
This Power Automate workflow is tailored for efficient extraction of key details from certificate files. It's designed to activate upon the addition of a certificate file in a specified OneDrive for Business folder.

### Key Features:
- **Triggered Execution**: Automatically initiates when a certificate file is added to the designated folder in OneDrive for Business.
- **Intelligent Data Extraction**: Utilizes a pre-trained document model to extract essential fields such as:
  - Certification Date
  - Name
  - Title
  - Profile URL
  - Active Since Date
  - Address
  - Four specific dates
  - Four corresponding earnings amounts
- **File Management**: Renames the uploaded PDF file for easy identification and organization.
- **SharePoint Integration**: Creates a new item in a SharePoint list with the extracted data.
- **Instant Notifications**: Sends a mobile notification upon successful completion of the workflow.

## Setting Up
To integrate this workflow into your system, follow these steps:

1. **Prepare OneDrive Folder**:
   - Designate or create a folder in OneDrive for Business where the certificate files will be uploaded.

2. **SharePoint List Configuration**:
   - Set up a SharePoint list to receive the extracted data.

3. **Workflow Customization**:
   - Customize the workflow as necessary to fit your specific needs and environment.

## Prerequisites
- A Microsoft Power Automate account (a premium license may be required for certain features).
- Access to OneDrive for Business and SharePoint Online.
- Pre-trained document model in AI Builder for data extraction.

## Useful Links
- **Certificate of Earnings PDF**: For downloading the certificate of earnings PDF, visit [Upwork Certificate of Earnings](https://www.upwork.com/ab/payments/reports/certificate-of-earnings.pdf).

## Additional Resources
For detailed instructions, customization tips, and troubleshooting, please refer to the further sections of this documentation.

---

Your contributions and suggestions for improvements to this workflow are always welcome!
