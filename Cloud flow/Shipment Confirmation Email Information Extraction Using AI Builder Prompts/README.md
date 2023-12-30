# AI Builder GPT Prompt Workflow for Email Data Extraction

This workflow use "Create text with GPT using a prompt action (Preview)" action to extract key information from shipment confirmation emails. The extracted data includes Sales Order Number, Tracking NO, Item Description, Order Quantity, and Shipped Quantity. The workflow involves testing AI custom prompt responses, parsing the response data as JSON, and converting it to CSV format.

## Workflow Steps

### 1. Define AI Builder Prompts
Create AI custom prompt in Prompt Builder to extract:
- Sales Order Number
- Tracking NO
- Item Description (Product Number)
- Order Quantity
- Shipped Quantity

### 2. Test AI Responses
Utilize the Prompt Builder "test your prompt" to ensure AI response accuracy.

### 3. Implement Approval Workflow
Becuase the "Create text with GPT using a prompt action" still in preview in my environment, so it require the `Start and Wait for an Approval of Text` action following it to use human oversight for the AI output.

### 4. Parse JSON and Convert to CSV
After approval, parse the AI output text into JSON, re-format the information and convert it to a CSV format.


## Conclusion

This workflow demonstrates the integration of AI Builder Prompts for practical business applications, for example to process the shipment emails. It shows a structured approach to data extraction. The action allows for the creation of customized prompts, enabling tailored responses. This means you can guide the AI to generate outputs that are specifically aligned with your business requirements or project needs.

