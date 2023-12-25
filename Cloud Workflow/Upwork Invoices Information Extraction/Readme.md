# Overview

This Power Automate workflow automates the extraction of key information from Upwork invoices using AI Builder's custom document extraction model. It streamlines the process of handling invoice data, improving efficiency and accuracy.

## Features

- **Automated Extraction:** Utilizes AI Builder's custom model to accurately extract invoice data.
- **Key Information Retrieval:** Extracts essential details such as 'Bill To', 'Attn', 'Bill to Address', 'Invoice Number', 'Invoice Date', 'Total Amount', and 'Memo'.
- **SharePoint Integration:** Automatically populates a SharePoint list with extracted data for easy management and access.

## How it Works

1. **Trigger:** The workflow is triggered when an invoice is uploaded to a specified folder in the Onedrive for Business.
2. **Data Extraction:** AI Builder's model extracts relevant invoice information.
3. **SharePoint List Creation:** The extracted data is used to create an item in a SharePoint list, containing the following columns:
    - Bill To
    - Attn
    - Bill to Address
    - Invoice Number
    - Invoice Date
    - Total Amount
    - Memo

- The uploaded invoice file is renamed to the format: `<Invoice Number>.pdf`

## Prerequisites

- Power Automate account.
- Access to AI Builder with a custom document extraction model.
- A SharePoint site with a designated list.

**Download the solution and import into your environment.**

The solution contains the customized document processing model that will be imported into your environment, but Microsoft said the model should be imported whthin 30 days afther the solution has been exported.

If you does not import with successfully, contact me.
