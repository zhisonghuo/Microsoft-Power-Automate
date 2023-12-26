# Power Automate Workflow for Upwork Summary Extraction

## Overview
This Power Automate workflow is designed to automate the extraction of key information from the Upwork weekly summaries. It utilizes AI Builder's custom document extraction model to accurately identify and retrieve critical data.

### Key Features:
- **Automatic Data Extraction**: Extracts key fields such as Start Date, End Date, Hours Worked, and Total Amount from Upwork weekly summaries.
- **Seamless Integration with OneDrive**: Activates when a PDF file is saved to a specified folder in OneDrive for Business.
- **Efficient Data Processing**: Uses a custom-trained document model to process the information.
- **SharePoint List Creation**: Automatically creates a SharePoint list item with the extracted data.
- **File Management**: Renames the processed file in the format `[Start Date]-[End Date].pdf`.
- **Instant Notifications**: Sends a mobile notification upon the completion of the workflow.

## Getting Started
To implement this workflow in your environment, follow these steps:

1. **SharePoint List Setup**:
   - Use the provided SharePoint list template to create a list in SharePoint Online.

2. **Workflow Import**:
   - Import the solution into your Power Automate environment.

3. **Customization**:
   - Modify the workflow as needed to fit your specific requirements.

## Prerequisites
- Microsoft Power Automate account.
- Access to SharePoint Online and OneDrive for Business.
- AI Builder access for custom document extraction model.

## Additional Information
For more detailed instructions and troubleshooting, please refer to the specific sections in this documentation.

---

Feel free to contribute or suggest improvements to this workflow. Your feedback is highly valued!
