## SharePoint to Azure SQL - Excel Integration Workflow

### Overview
This project demonstrates a robust workflow designed to seamlessly integrate Excel files uploaded to a SharePoint library into an Azure SQL table. Tailored for efficiency and accuracy, this workflow automates the data transfer process, ensuring data integrity and consistency across platforms.

### Key Features

- **Filtering Rows Based on Criteria**: The workflow includes a sophisticated filtering mechanism that selectively processes rows from the Excel file. This feature allows for the extraction of relevant data based on predefined criteria, ensuring that only pertinent information is transferred to the Azure SQL table.

- **Excel Date Processing**: A notable capability of this workflow is its adept handling of date formats from Excel files. The system is designed to accurately interpret and convert Excel date formats, ensuring that date-related data is correctly reflected in the Azure SQL database.

- **Robust Error Handling**: To maintain the integrity of the data transfer process, the workflow is equipped with comprehensive error handling strategies. These mechanisms detect and manage exceptions, preventing data corruption and ensuring the smooth operation of the workflow. Error logs and alerts are implemented for immediate issue identification and resolution.


The Power Automate expression used for date conversion is as follows:
```plaintext
if(
  equals(
    items('ApplyToEachExcelRow')?['Date'], 
    null
  ),
  null, 
  if(
    equals(
      int(items('ApplyToEachExcelRow')?['Date']), 
      1
    ),
    addDays('1899-12-31', 1, 'yyyy-MM-dd'),
    addDays('1899-12-30', 
      int(items('ApplyToEachExcelRow')?['Date']), 
      'yyyy-MM-dd'
    )
  )
)
```
This expression checks if the 'Date' field is null and processes it accordingly to ensure the date is correctly formatted for Azure SQL.
### Implementation Details

The workflow is triggered when a new Excel file is added to a specified SharePoint library. Upon activation, the workflow performs the following actions:

1. **Initial File Validation**: Checks the format and structure of the Excel file to ensure compatibility.
2. **Data Extraction**: Extracts data from the Excel file, applying row filters based on the defined criteria.
3. **Date Processing**: Converts Excel date formats to a compatible format for Azure SQL.
4. **Data Insertion**: Inserts the processed data into the Azure SQL table.
5. **Error Handling**: Monitors the process for any exceptions, handling them accordingly and logging details for review.

### Technologies Used

- Microsoft SharePoint
- Microsoft Excel
- Azure SQL Database

