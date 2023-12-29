# AI Builder GPT Prompt Workflow for Email Data Extraction

This repository outlines a workflow using AI Builder GPT Prompts to extract key information from shipment confirmation emails. The extracted data includes Sales Order Number, Tracking Number, Item Description, Order Quantity, and Shipped Quantity. The workflow involves testing AI responses, parsing data as JSON, and converting it to CSV format.

## Workflow Steps

### 1. Define AI Builder Prompts
Create targeted prompts for the AI Builder to extract:
- Sales Order Number
- Tracking Number
- Item Description
- Order Quantity
- Shipped Quantity

### 2. Test AI Responses
Utilize the `Create text with GPT using a prompt` action to test the AI's extraction accuracy.

### 3. Format Response as JSON
Structure the AI's response in a JSON format with key-value pairs for each data point.

### 4. Implement Approval Workflow
Incorporate the `Start and Wait for an Approval of Text` action, essential in the preview version for verifying the extracted data.

### 5. Parse JSON and Convert to CSV
After approval, parse the JSON to extract the information and convert it to a CSV format.

### 6. Error Handling
Ensure robust error handling for data format inconsistencies and extraction inaccuracies.

### 7. Optimization and Testing
Regularly test and refine the workflow to handle various email formats and enhance accuracy.

### 8. Documentation
Detailed documentation of each step is provided for clarity and ease of understanding.

## Conclusion

This workflow demonstrates the integration of AI Builder Prompts for practical business applications, specifically in processing shipment confirmation emails. It shows a structured approach to data extraction, approval, and conversion, suitable for presentation in a professional portfolio.

