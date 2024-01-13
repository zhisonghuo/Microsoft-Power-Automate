# Power Automate Workflow for Client-Specific File Routing

## Overview
This Power Automate workflow is designed for efficient file management, specifically routing files based on client IDs. It operates by organizing files from a root source folder to corresponding client folders.

### Key Workflow Functions:
- **Folder Path Specification**: 
  - **Source Folder**: Specify the root folder path for source files.
  - **Clients Root Folder**: Designate the root path where individual client folders are located.
- **Client Folder Identification**: Client folders are named following the format `[Client Name]_[Client ID]`.
- **Consistent Folder Structure**: Ensures that the folder structure under both the Source Folder and each client folder is identical.

### Workflow Process:
1. **File Addition Trigger**: The workflow initiates when a file is added to the Source Folder or its subfolders.
2. **Client ID Extraction**: Extracts the client ID from the file name in the Source Folder.
3. **Client Folder Matching**:
   - Checks the client folder list using the extracted client ID.
   - If a matching client folder is found, the file is routed to the corresponding folder, mirroring the structure in the Source Folder.
4. **Routing Verification**:
   - Ensures files are directed to either the exact folder or an equivalent subfolder within the client's directory.
5. **Non-Existent Client Handling**: Sends a notification if the target client folder is not found.

## Setting Up
To effectively implement this workflow in your environment, ensure the following steps are taken:
1. **Configure Source and Clients Root Folders**: Define the paths for the Source Folder and the Clients Root Folder.
2. **Standardize Folder Structures**: Verify that the folder structures in both areas are identical.
