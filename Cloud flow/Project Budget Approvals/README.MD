# Project Budget Approval Workflow

## Overview
This project implements an automated approval workflow in SharePoint, designed to streamline the process of budget requests and approvals within an organization. The workflow is triggered when a requester submits a budget request, and it facilitates the management of approvals through SharePoint list updates and notifications.

## Workflow Stages
1. **Request Submission**: Users submit budget requests via a SharePoint list, including details like Project Name, Department, Budget Requested, Purpose, Start Date, and End Date.
2. **Approval Process**: The workflow, upon submission, identifies the manager of the requester and sends a notification for approval.
3. **Decision Handling**:
   - If **approved**, the workflow updates the SharePoint list with the approval status, approver's name, and comments. The requester is then notified.
   - If **rejected**, the workflow updates the list item accordingly and notifies the requester.

## Workflow Versions
### Version 1
- Utilizes two distinct actions: "Create an Approval" and "Wait for Approval".
- Focuses on a straightforward approval mechanism.

### Version 2
- Employs a single "Start and Wait for an Approval" action.
- Streamlines the approval process.

### Version 3
- Incorporates "Start and Wait for an Approval of Text".
- Allows approvers to modify the "Budget Requested" field during approval.
- Updates the SharePoint list item with the new budget if modified and approved.

## Key Features
- **Dynamic Manager Identification**: Automates the process of finding and notifying the requester's manager for approval.
- **Adaptive Approval Workflow**: Supports different workflow versions to cater to various approval scenarios.
- **Real-time Notifications**: Ensures timely communication to both approvers and requesters.
- **List Item Updates**: Maintains an accurate record of approval statuses and comments in SharePoint.

## Connector Involved
- Approvals
- SharePoint
- Office 365 Users
- Office 365 Outlook

