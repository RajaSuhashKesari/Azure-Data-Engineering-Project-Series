# Azure-Data-Engineering-Project-Series
## 📌 Projects List --
    |  -> Project #1 :- Handle Error Rows in Data Factory Mapping Data Flows
    |  -> Project #2 :- Copy Multiple CSV Files of Employees using Wildcard File Path Method
    |  -> Project #3 :- Delete Files Older Than 30 Days
    |  -> Project #4 :- Incremental File Copy Based on Last_Modified_Date.
    |  -> Project #5 :- Process Fixed Length Text to CSV using ADF Mapping Dataflows
    |  -> Project #6 :- Log Pipeline Executions to SQL Table using Azure Data Factory
## Project #1 :- Handle Error Rows in Data Factory Mapping Data Flows
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
## Project #2 :- Copy Multiple Files CSV Files of Employees using Wildcard file path Method
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
## Project #3 :- Delete files older than 30 days
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
## Project #4: Incremental File Copy Based on Last_Modified_Date
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
## Project #5 :- Process Fixed Length Text to CSV using ADF Mapping Dataflows
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


CREATE TABLE [pipeline_logs].[pipeline_executions](
    data_factory_name varchar(50),
	pipeline_name varchar(50),
	trigger_name varchar(50),
	run_id varchar(50),
	trigger_time DateTime
)

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
	)
END










