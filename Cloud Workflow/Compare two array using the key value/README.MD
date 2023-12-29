# Power Automate Workflow for Array Comparison

## Overview
This workflow is designed to compare two arrays in Power Automate, focusing on matching key values within each array. The comparison process is governed by a specific JSON schema where `eenum` serves as the key identifier.

### Key Features:
- **Consistent JSON Schema**: Both arrays adhere to the same JSON structure, with `eenum` as the key field.
- **Array Comparison Logic**: 
  - Iterates through each item in the `wtArr` array.
  - Extracts the `eenum` key value from each item.
  - Compares this key value against each key in the `dvArr` array.

### Workflow Outcome:
- **Result Determination**: 
  - If a matching key is found, the workflow sets the `Result` value to "YES", indicating that the corresponding item in the destination array (`dvArr`) has been successfully identified.
  - The workflow efficiently identifies and marks items in the destination array that have a corresponding match in the source array.

## Implementation Steps
1. **Array Setup**:
   - Ensure both `wtArr` and `dvArr` arrays are initialized and populated according to the required JSON schema.
2. **Workflow Customization**:
   - Tailor the comparison logic to suit the specific structure and requirements of your arrays.

## Prerequisites
- Basic knowledge of JSON schema and array handling in Power Automate.
- Understanding of loop structures and conditional logic within Power Automate workflows.
