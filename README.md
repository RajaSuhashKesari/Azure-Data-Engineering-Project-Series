# Azure-Data-Engineering-Project-Series
## 📌 Projects List --
    |  -> Project #1 :- Handle Error Rows in Data Factory Mapping Data Flows
    |  -> Project #2 :- Copy Multiple CSV Files of Employees using Wildcard File Path Method
    |  -> Project #3 :- Delete Files Older Than 30 Days
    |  -> Project #4 :- Incremental File Copy Based on Last_Modified_Date.
    |  -> Project #5 :- Process Fixed Length Text to CSV using ADF Mapping Dataflows
    |  -> Project #6 :- Log Pipeline Executions to SQL Table using Azure Data Factory
    |  -> Project #7 :- Remove Duplicate Rows using Mapping Data Flows in Azure Data Factory
    |  -> Project #8 :- Add new Employees to File By Incrementing Key using Mapping Data Flow in ADF
    |  -> Project #9 :- Calculate Running Total of Purchase for Each Customer
    |  -> Project #10 :- Log Pipeline Executions to CSV File Using Azure Data Factory
    |  -> Project #11 :- Implement SCD Type - 1 When Source is CSV and Sink is SQL
    |  -> Project #12 :- Implement SCD Type - 1 When Source is CSV and Sink is CSV
# Project #1 :- Handle Error Rows in Data Factory Mapping Data Flows
In this project i have built an pipeline in Azure Data Factory which is going to extract multiple employee csv files from the ADLS Gen2 and used Data flow transformations to seperate good and bad data from the each csv file.
Finally i stored the good and bad rows seperatley in the seperate table in the Azure SQL Database.
## 1.1 pipeline
![image](https://github.com/user-attachments/assets/0c04ea37-b158-4a02-8da6-2995fb90df94)
## 1.2 Dataflow
![image](https://github.com/user-attachments/assets/abe78c2b-bd1e-4904-8038-4762713177ad)
## 1.3 pipeline execution
![image](https://github.com/user-attachments/assets/61f80cdc-5291-44c4-bb3d-d7395a54d00f)
## 1.4 Input datasets
![image](https://github.com/user-attachments/assets/0cc8bbe9-7af4-4d45-8853-7384b3b42991)
## 1.5 Output filtered rows
### 1.5.1 Good rows
![image](https://github.com/user-attachments/assets/8e6331d5-da86-4fc4-8ff9-c4cbdcf81bde)
### 1.5.2 Bad rows
![image](https://github.com/user-attachments/assets/4502825f-c74f-48db-854c-48494139153b)

---

# Project #2 :- Copy Multiple Files CSV Files of Employees using Wildcard file path Method
## 2.1 pipeline image
![image](https://github.com/user-attachments/assets/933ae6e6-c18d-44eb-a4e9-41c01174dd41)
## 2.2 Exection of pipeline
![image](https://github.com/user-attachments/assets/1a5e3192-015c-4c9f-9ea7-b07e88289060)
## 2.3 Dataset - input folder
![image](https://github.com/user-attachments/assets/6d2749f7-9e19-46b2-a9b2-8ce3bbff04fa)
![image](https://github.com/user-attachments/assets/a22f3060-d56d-4e05-90b3-a62effd44bde)
## 2.4 Dataset - output folder
![image](https://github.com/user-attachments/assets/3fe1be1a-b058-4fc7-8482-c809ae91c2ab)
![image](https://github.com/user-attachments/assets/d0024c3a-66ce-4c5e-bcaa-9c628c7ce904)

---

# Project #3 :- Delete files older than 30 days
## 3.1 pipeline image
![image](https://github.com/user-attachments/assets/084a3fb5-fb80-4408-9c54-f05343cf5bdd)
## 3.2 Dataset
![image](https://github.com/user-attachments/assets/035b47c8-210b-4147-bdb8-1eb2c7974cba)
## 3.3 Files Present before execution of pipeline
![image](https://github.com/user-attachments/assets/4c6e8e1f-d2fc-467d-a954-11aa22f7c0a2)
## 3.4 Execution of pipeline
![image](https://github.com/user-attachments/assets/884e424d-e006-45cd-b3c7-3553a084deb8)
## 3.5 Files Deleted After Execution of the pipeline
![image](https://github.com/user-attachments/assets/a0d3290c-2b1b-4f12-be57-03bbfe3b230e)
## 3.6 Log file to track which files are deleted.
![image](https://github.com/user-attachments/assets/567b4f85-ea96-4258-8ffe-e34412f45ef1)

---

# Project #4: Incremental File Copy Based on Last_Modified_Date
This project demonstrates how to incrementally copy newly added or modified files from one ADLS Gen2 folder to another using Azure Data Factory. The pipeline intelligently filters files based on their last modified timestamp.
## 4.1 Pipeline & Copy Data Activity Configuration
![image](https://github.com/user-attachments/assets/c3c9aaee-3fa0-4638-8bc1-e3b032f59420)
## 4.2 Trigger Setup
A Scheduled Trigger is configured to automatically execute the pipeline once daily at 13:00 IST.
![image](https://github.com/user-attachments/assets/1caa98b8-733e-4a0a-a90a-7381588a39a8)
## 4.3 Datasets
### 4.3.1 Input Folder: DS_Folder_Contains_Files
![image](https://github.com/user-attachments/assets/dc9cff05-ed12-46ab-ad6c-603f45050812)
### 4.3.2 Output Folder: DS_Folder_Load_Files_Incrementally_Destination
![image](https://github.com/user-attachments/assets/5b554fad-4df7-4ac0-aa19-4591f9c89a05)
## 4.4 Pipeline Trigger Execution
![image](https://github.com/user-attachments/assets/df761dd7-ca53-4755-b059-0067790f2e25)
## 4.5 Input Files (Sample)
![image](https://github.com/user-attachments/assets/756fe0c1-d323-4659-ac9e-990ede75b8f7)
## 4.6 Output After Incremental Load
### 4.6.1 Before Execution
![image](https://github.com/user-attachments/assets/b45b8ea3-09a9-425c-bc2d-1906222309b5)
### 4.6.2 After Execution
![image](https://github.com/user-attachments/assets/61df00a7-4e57-4f8b-9ded-90c99c733157)

---

# Project #5 :- Process Fixed Length Text to CSV using ADF Mapping Dataflows
## 5.1 pipeline : Dataflow Activity
![image](https://github.com/user-attachments/assets/8d7dd342-c4d8-48c9-ad2f-3f9d48d1915c)
## 5.2 Dataflow: DF Parse Fixed Length employee
![image](https://github.com/user-attachments/assets/82c00388-e1a1-4b03-9177-fe73ae9abe31)
## 5.3 Pipeline Execution 
![image](https://github.com/user-attachments/assets/ad00ca2d-2401-4599-91df-ca2d07fe6742)
## 5.4 Datasets
### 5.4.1 Input Dataset :ds_input_fixedlength_txt
![image](https://github.com/user-attachments/assets/c96cb2f5-85e3-459f-ac46-8cdba1752c2b)
### 5.4.2 Output Dataset :ds_output_employee_csv
![image](https://github.com/user-attachments/assets/c6e6a780-015c-4d53-9870-cc208c85990d)
## 5.5 Final Outcomes
### 5.5.1 fixed length text file
![image](https://github.com/user-attachments/assets/48fb7024-eaca-46db-8ffb-d815ba5e3593)
### 5.5.2 Parsed fixed length text file to CSV
![image](https://github.com/user-attachments/assets/8e52208c-8cee-4a49-9ffc-abaa8d2de0f4)
![image](https://github.com/user-attachments/assets/2ca00d53-9238-4e81-a584-5fd1cd0bfa1f)

---

# Project #6 :- Log Pipeline Executions to SQL Table using Azure Data Factory
I created an Azure Data Factory (ADF) pipeline to log pipeline execution details into an Azure SQL Database. First, I designed a table and a stored procedure in Azure SQL DB. Then, in ADF, I built a pipeline that uses the Stored Procedure activity. Whenever this activity executes, the stored procedure inserts execution log data into the SQL table. The pipeline passes metadata such as pipeline name, run ID, trigger name, and execution time dynamically to the stored procedure through the activity’s parameter settings.

## 6.1 pipeline 
<img width="917" height="227" alt="image" src="https://github.com/user-attachments/assets/7bac76df-6613-4212-a34d-6c063403e8a6" />

## 6.2 Stored Procedure Activity Settings
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/01d95b5b-56c2-451a-b374-961fa84fc6f1" />

## 6.3 Pipeline Execution 
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/315f0a40-6e1b-488a-b70f-cfe41bf2e4f5" />

## 6.4 Azure SQL Table and Stored Procedure Setup
```sql
/* Create table */
CREATE TABLE [pipeline_logs].[pipeline_executions](
    data_factory_name varchar(50),
    pipeline_name varchar(50),
    trigger_name varchar(50),
    run_id varchar(50),
    trigger_time DateTime
);

/* Create stored procedure */
CREATE PROCEDURE [pipeline_logs].[sp_insert_pipline_log](
    @data_factory_name varchar(50),
    @pipeline_name varchar(50),
    @trigger_name varchar(50),
    @run_id varchar(50),
    @trigger_time DateTime
)
AS
BEGIN
    INSERT INTO [pipeline_logs].[pipeline_executions] VALUES(
        @data_factory_name,
        @pipeline_name,
        @trigger_name,
        @run_id,
        @trigger_time
    );
END;
```
## 6.5 SQL table before pipeline execution
<img width="1165" height="600" alt="image" src="https://github.com/user-attachments/assets/01b67736-41e5-4972-be9a-59d591ede9c8" />

## 6.6 SQL table after pipeline execution
<img width="1167" height="591" alt="image" src="https://github.com/user-attachments/assets/d6d20cf2-6699-46c2-b1bf-5cd0d60c6b74" />

# Project #7 :- Remove Duplicate Rows using Mapping Data Flows in Azure Data Factory

This project demonstrates how to remove duplicate employee records stored in **Azure Data Lake Storage Gen2** using **Azure Data Factory (ADF) Mapping Data Flow**, while retaining only the **first occurrence** of each record.

---

## 🚀 Pipeline Overview

### **1. Data Flow Activity**
- The ADF pipeline uses a **Data Flow Activity** to invoke a Mapping Data Flow that performs the deduplication process.

### **2. Data Sources**
- Two separate source datasets from **ADLS Gen2**.
- Both datasets share the same schema but contain some duplicate `employee_id` values.

### **3. Union Transformation**
- Combines data from both sources into a single unified dataset.

### **4. Aggregate Transformation**
- **Group By:** `employee_id`
- **Aggregation:**
  - Utilized **Column Pattern** to dynamically select all columns.
  - **Condition in Column Pattern:** Matches all columns in the dataset.
  - **Aggregation Expression:** `first($$)` — ensures only the first occurrence of each duplicate record is kept.

### **5. Sort Transformation**
- Sorts the resulting data by `employee_id` for cleaner, ordered output.

### **6. Sink**
- Writes the final **deduplicated and sorted dataset** into a CSV file in **ADLS Gen2**.

---

## 🛠 Key Features
- **Schema Drift Support:** Automatically adapts to schema changes without manual column mapping.
- **Efficient Deduplication:** Keeps only the first occurrence of duplicates using a dynamic aggregation pattern.
- **Organized Output:** Sorted results for better readability.

---

## 7.1 Pipeline Diagram
<img width="1157" height="762" alt="image" src="https://github.com/user-attachments/assets/e393f5d8-8c7d-48ed-bb95-745786c3263b" />

## 7.2 Dataflow Diagram
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/8cb7ffc9-5479-4b4a-bf8b-7150381b5d8c" />

## 7.3 Input Data
### 7.3.1 employees_file1.csv
<img width="432" height="308" alt="image" src="https://github.com/user-attachments/assets/cb12e484-357b-4796-8076-dc6230ebfbb9" />

### 7.3.1 employees_file2.csv
<img width="422" height="317" alt="image" src="https://github.com/user-attachments/assets/dfb21d4e-6a31-4515-a9d4-77bbc6cddb7e" />

## 7.3 Output Data
<img width="416" height="382" alt="image" src="https://github.com/user-attachments/assets/8805fb20-c519-4b02-a158-a95db7a4afa5" />

# Project #8 :- Add new Employees to File By Incrementing Key using Mapping Data Flow in ADF
## **Overview**
This project demonstrates how to incrementally load new employee data into an existing employee dataset stored in **Azure Data Lake Storage Gen2** using **Azure Data Factory Mapping Data Flow**.

### **The Challenge**
- **Final Employees dataset** already contains `employee_id` values.
- **New Employees dataset** does **not** contain `employee_id`.
- Requirement: Append new employees with **incremental IDs** without overwriting or duplicating existing IDs.

---

## **Pipeline Flow**

### **Data Flow Activity**
- The pipeline calls a **Mapping Data Flow** to handle **ID assignment** and **data merging**.

---

## **Mapping Data Flow Steps**

### **1. Sources**
- **Source 1**: Final Employees CSV (**with** `employee_id`)
- **Source 2**: New Employees CSV (**without** `employee_id`)

---

### **2. Find Maximum Existing ID**
- **Aggregate Transformation** on Final Employees dataset:
  - **Group By**: *(none)* → to get a single aggregated result.
  - **Aggregate Column**: `max(employee_id)` → renamed as `max_id`.

---

### **3. Generate Dummy IDs for New Employees**
- **Surrogate Key Transformation** on New Employees dataset:
  - Creates a new column `dummy_emp_id` with sequential values: `1, 2, 3, ...`

---

### **4. Cross Join for ID Increment**
- **Cross Join** between:
  - `max_id` (from aggregate)
  - `dummy_emp_id` (from new employee data)
- Purpose: Allows each new employee to know the maximum existing ID.

---

### **5. Create Incremental Employee ID**
- **Derived Column Transformation**:
  - New column:  
    ```
    employee_id = max_id + dummy_emp_id
    ```
  - Assigns unique incremental IDs to new employees.

---

### **6. Remove Unwanted Columns**
- **Select Transformation**:
  - Drop: `max_id`, `dummy_emp_id`
  - Keep: `employee_id`, `name`, `department`, `salary`

---

### **7. Merge Old and New Data**
- **Union Transformation**:
  - Combine Final Employees dataset with New Employees dataset (now with IDs).

---

### **8. Sort Data**
- **Sort Transformation**:
  - Sort by `employee_id` for a clean, ordered output.

---

### **9. Write Back to ADLS Gen2**
- **Sink**:
  - Write the merged dataset back to the **same file** containing the original Final Employees data (**overwrite with updated data**).

---

## 8.1 Pipeline :
<img width="1226" height="897" alt="image" src="https://github.com/user-attachments/assets/511bd535-ca1a-4803-8c90-9ad8f25f683c" />

## 8.2 Mapping DataFlow
<img width="1867" height="337" alt="image" src="https://github.com/user-attachments/assets/1a9c1300-07de-461e-b052-cc50ca988cb1" />

## 8.3 Input
### 8.3.1 New Employees
<img width="320" height="213" alt="image" src="https://github.com/user-attachments/assets/565b3cbf-f28b-4789-aa9a-205c2ffda335" />

### 8.3.2 Final_Employees
<img width="471" height="260" alt="image" src="https://github.com/user-attachments/assets/4d78c759-20c2-46b3-8fdf-4fd0a1a777a5" />

## 8.4  Final Output
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/2b3ec29e-9ef0-4213-80ae-9351ea06c1e9" />

---
# Project #9 :- Calculate Running Total of Purchase for Each Customer
## 9.1 Overview
This pipeline calculates the running total of purchases for each customer using Azure Data Factory's Mapping Data Flow. The solution:
1. Processed Purchase data from source systems
2. Applies window transformation for cumulative sums3
3. Stores processed results in ADLS Gen2
## 9.2 Implementation Details
### 9.2.1 Data Flow Image
<img width="1832" height="388" alt="image" src="https://github.com/user-attachments/assets/81831d71-f9ea-488d-a3ff-026ada0c18b9" />

### 9.2.2 Window Transformation Configuration
Key Settings:
#### Over Clause: CustomerID (Partitioning)
<img width="1762" height="775" alt="image" src="https://github.com/user-attachments/assets/4ecddb4a-95fe-48b4-9fd9-aa713875cf85" />

#### Sort Clause: Date ASC (Ordering)
<img width="1185" height="229" alt="image" src="https://github.com/user-attachments/assets/5a7e8751-d302-4184-8ac9-64460516d2d3" />

### Window Column:
<img width="1170" height="298" alt="image" src="https://github.com/user-attachments/assets/7ee3eba0-e154-47c4-8993-1dd34ec90c41" />

## 9.3 Input-Output of Dataflow
### 9.3.1 Source Data
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1a858f37-33bf-4a71-89d3-2a31c982b372" />

### 9.3.2 Processed Output
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d8451410-70f9-4e77-823c-0c8d0d7f254b" />

### 9.4 Final Conclusion
Based on the above output and below calculation all out produced by **Window Transformation** is correct
##### Customer C001:
```
2025-08-01: 120.50 (Running Total: 120.50)
2025-08-02: 80.00 (120.50 + 80.00 = 200.50)
2025-08-04: 45.25 (200.50 + 45.25 = 245.75)
2025-08-05: 150.00 (245.75 + 150.00 = 395.75)
2025-08-06: 50.00 (395.75 + 50.00 = 445.75)
2025-08-09: 200.00 (445.75 + 200.00 = 645.75)
```
C001 running totals are correct.

##### Customer C002:
```
2025-08-02: 75.00 (Running Total: 75.00)
2025-08-04: 150.75 (75.00 + 150.75 = 225.75)
2025-08-07: 95.00 (225.75 + 95.00 = 320.75)
2025-08-10: 250.00 (320.75 + 250.00 = 570.75)
```
C002 running totals are correct.

##### Customer C003:
```
2025-08-03: 220.00 (Running Total: 220.00)
2025-08-05: 180.50 (220.00 + 180.50 = 400.50)
2025-08-08: 120.00 (400.50 + 120.00 = 520.50)
2025-08-09: 75.50 (520.50 + 75.50 = 596.00)
```
C003 running totals are correct.

#### Final Verification:
My dataflow output correctly shows:
Each customer's purchases in chronological order,
The running totals accumulate properly within each customer group,
No mixing of totals between different customers.

---
# Project #10 :- Log Pipeline Executions to CSV File Using Azure Data Factory
📌 Project Overview

This project automates the logging of Azure Data Factory (ADF) pipeline runs into CSV files stored in Azure Data Lake Storage Gen2 (ADLS Gen2).

The pipeline is designed to capture all pipeline execution details from the previous day and store them in a structured format for auditing, monitoring, and analysis.

Each day, the pipeline produces a CSV file named with yesterday’s date, containing all the triggered pipelines within the defined time window.

## Requirments
1. Linked Services
   - Rest Linked Service
   - ADLS Gen2 Linked Service
2. Datasets
   - Rest Dataset
   - Delimited Text ADLS Gen2
3. Managed Identity
   - Enable Managed Identity of the same data factory that you are working with.
   - Go to role assignments and add "Data Factory Contributer" or "Data Factory Reader" role to the same Data Factory
4. Triggers
   - Create a schedule trigger which will trigger this pipliine daily at 12:00 AM
5. Pipeline to extract pipeline logs and put it in csv file
## 10.1 Pipeline image :
<img width="552" height="296" alt="image" src="https://github.com/user-attachments/assets/49a231be-5d23-4339-bdc4-0ed4ec6e3796" />

### 10.1.1 Copy Data Activty - Source :
<img width="1397" height="682" alt="image" src="https://github.com/user-attachments/assets/1d7ad00f-7d17-4467-a59a-ea4f41da4c87" />

**Request Body:-**
```
@concat(
  '{ "lastUpdatedAfter": "', formatDateTime(addDays(addMinutes(addHours(utcNow(), 5), 30), -1), 'yyyy-MM-ddT00:00:00Z'),
  '", "lastUpdatedBefore": "', formatDateTime(addDays(addMinutes(addHours(utcNow(), 5), 30), -1), 'yyyy-MM-ddT23:59:59'),
  '" }'
)
```
### 10.1.2 Copy Data Activty - Sink :
<img width="1392" height="682" alt="image" src="https://github.com/user-attachments/assets/68f65e8c-b6c6-47ff-8aaf-fee37a054b5b" />

Give file name directly or you can create paramter for CSV dataset and you can the file name dynamically at in **Copy Activity - Sink**
**File Name:-**
```
@concat(
    formatDateTime(
        addDays(
            addMinutes(addHours(utcNow(), 5), 30),
            -1
        ),
        'yyyy-MM-dd'
    ),
    '.csv'
)
```
### 10.1.3 Copy Data Activty - Mappings :
**Don't forget to use refernce Collection**
**Make sure all data type finally in string if not you will face error**
<img width="1141" height="958" alt="image" src="https://github.com/user-attachments/assets/dc51c2e8-9770-4eed-acc4-a38110d3b714" />

## 10.2 REST Linked Service - Configurations :-
<img width="712" height="1033" alt="image" src="https://github.com/user-attachments/assets/0b371f76-8e41-4419-83b3-90f9e029ecf9" />

**Base Url:**
```
https://management.azure.com/subscriptions/<PUT- YOUR-SUBSCRPTION-ID-HERE>/resourceGroups/<PUT-YOUR-RESOURCE-GROUP-NAME-HERE>/providers/Microsoft.DataFactory/factories/<PUT-DATA-FACTORY-NAME-HERE>
```
**Microsoft Entra ID resource:-**
```
https://management.azure.com/
```
## 10.3 Trigger - Configuration:-
<img width="710" height="1036" alt="image" src="https://github.com/user-attachments/assets/eb02ed25-fc33-41b7-827f-075ad1433999" />

## 10.4 Final Output:-
### CSV File generated in the ADLS Gen2 with yesterday date
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/a5b4335a-6ce0-4794-8d3a-97a780ce56bf" />

### CSV File Data
<img width="1405" height="902" alt="image" src="https://github.com/user-attachments/assets/2fce3541-5c89-4408-b7ad-5796e52cfd59" />

---

