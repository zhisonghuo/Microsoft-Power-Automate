# Employee of the Month Nomination System

## Project Overview

This repository contains the implementation of an automated system designed to streamline the 'Employee of the Month' nomination process within an IT department. The solution utilizes the Microsoft Power Automate workflow to efficiently manage nominations from submission to confirmation.

## Features

- **Microsoft Forms Integration**: Collects nomination data through a user-friendly interface.
- **Automated Document Population**: Auto-fills a Word template with the submitted data to ensure consistency.
- **PDF Conversion**: Transforms the populated Word document into a PDF for a professional appearance and ease of distribution.
- **Email Automation**: Automatically sends the generated PDF back to the nominator for review and confirmation.

## Technologies Used

- Microsoft Power Automate
- Microsoft Forms
- Microsoft Word
- PDF Conversion

## Setup and Usage

### Prerequisites

Before setting up the workflow, ensure you have access to the following Microsoft services:

- Microsoft Forms for creating nomination forms.
- Microsoft Power Automate to automate the workflow.
- Microsoft Word for template creation.
- An email service configured to work with Power Automate for sending notifications.

### Setting Up the Nomination Form

1. **Create a Nomination Form**:
   - Log in to Microsoft Forms.
   - Create a new form for 'Employee of the Month' nominations.
   - Add necessary fields such as the name of the nominee, nominator's details, reasons for nomination, etc.
   - Ensure the form is accessible to all potential nominators within your organization.

### Configuring Power Automate Workflow

2. **Set up a Power Automate Flow**:
   - Access Power Automate and create a new automated flow triggered by new form responses.
   - Configure the flow to capture response details and populate a Word template with the nomination data.
   - Add a step to convert the Word document into a PDF format.
   - Set up an action to email the PDF to the nominator for confirmation.

### Using the System

3. **Nomination Submission**:
   - Nominators fill out the form with the nominee's details and their contributions.
   - Upon submission, the Power Automate workflow is triggered automatically.

4. **Automated Document Generation**:
   - The flow captures the form data and populates the Word template.
   - The populated template is then converted to a PDF for a standardized look.

5. **Review and Confirmation**:
   - The nominator receives an email with the PDF attached.
   - They can review the nomination and provide any additional feedback if necessary.

### Final Steps

6. **Archiving and Record-Keeping**:
   - Store the final PDFs in a secure location for record-keeping.
   - Optionally, create a SharePoint site or a dedicated folder in OneDrive for easy access to all nominations.

This automated system simplifies the process of nominating employees for recognition, reduces manual effort, and ensures a consistent and professional presentation of nominations.
