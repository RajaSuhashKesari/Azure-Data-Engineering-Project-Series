# Azure-Data-Engineering-Project-Series
## 📌 Projects List --
    |  -> Project #1 :- Handle Error Rows in Data Factory Mapping Data Flows
    |  -> Project #2 :- Copy Multiple CSV Files of Employees using Wildcard File Path Method
    |  -> Project #3 :- Delete Files Older Than 30 Days
    |  -> Project #4 :- Incremental File Copy Based on Last_Modified_Date.
## Project #1 :- Handle Error Rows in Data Factory Mapping Data Flows
In this project i have built an pipeline in Azure Data Factory which is going to extract multiple employee csv files from the ADLS Gen2 and used Data flow transformations to seperate good and bad data from the each csv file.
Finally i stored the good and bad rows seperatley in the seperate table in the Azure SQL Database.
## pipeline
![image](https://github.com/user-attachments/assets/0c04ea37-b158-4a02-8da6-2995fb90df94)
## Dataflow
![image](https://github.com/user-attachments/assets/abe78c2b-bd1e-4904-8038-4762713177ad)
## pipeline execution
![image](https://github.com/user-attachments/assets/61f80cdc-5291-44c4-bb3d-d7395a54d00f)
## Input datasets
![image](https://github.com/user-attachments/assets/0cc8bbe9-7af4-4d45-8853-7384b3b42991)
## Output filtered rows
### Good rows
![image](https://github.com/user-attachments/assets/8e6331d5-da86-4fc4-8ff9-c4cbdcf81bde)
### Bad rows
![image](https://github.com/user-attachments/assets/4502825f-c74f-48db-854c-48494139153b)
## Project #2 :- Copy Multiple Files CSV Files of Employees using Wildcard file path Method
## pipeline image
![image](https://github.com/user-attachments/assets/933ae6e6-c18d-44eb-a4e9-41c01174dd41)
## Exection of pipeline
![image](https://github.com/user-attachments/assets/1a5e3192-015c-4c9f-9ea7-b07e88289060)
## Dataset - input folder
![image](https://github.com/user-attachments/assets/6d2749f7-9e19-46b2-a9b2-8ce3bbff04fa)
![image](https://github.com/user-attachments/assets/a22f3060-d56d-4e05-90b3-a62effd44bde)
## Dataset - output folder
![image](https://github.com/user-attachments/assets/3fe1be1a-b058-4fc7-8482-c809ae91c2ab)
![image](https://github.com/user-attachments/assets/d0024c3a-66ce-4c5e-bcaa-9c628c7ce904)
## Project #3 :- Delete files older than 30 days
## pipeline image
![image](https://github.com/user-attachments/assets/084a3fb5-fb80-4408-9c54-f05343cf5bdd)
## Dataset
![image](https://github.com/user-attachments/assets/035b47c8-210b-4147-bdb8-1eb2c7974cba)
## Files Present before execution of pipeline
![image](https://github.com/user-attachments/assets/4c6e8e1f-d2fc-467d-a954-11aa22f7c0a2)
## Execution of pipeline
![image](https://github.com/user-attachments/assets/884e424d-e006-45cd-b3c7-3553a084deb8)
## Files Deleted After Execution of the pipeline
![image](https://github.com/user-attachments/assets/a0d3290c-2b1b-4f12-be57-03bbfe3b230e)
## Log file to track which files are deleted.
![image](https://github.com/user-attachments/assets/567b4f85-ea96-4258-8ffe-e34412f45ef1)
## Project #4: Incremental File Copy Based on Last_Modified_Date
This project demonstrates how to incrementally copy newly added or modified files from one ADLS Gen2 folder to another using Azure Data Factory. The pipeline intelligently filters files based on their last modified timestamp.
## Pipeline & Copy Data Activity Configuration
![image](https://github.com/user-attachments/assets/c3c9aaee-3fa0-4638-8bc1-e3b032f59420)
## Trigger Setup
A Scheduled Trigger is configured to automatically execute the pipeline once daily at 13:00 IST.
![image](https://github.com/user-attachments/assets/1caa98b8-733e-4a0a-a90a-7381588a39a8)
## Datasets
### Input Folder: DS_Folder_Contains_Files
![image](https://github.com/user-attachments/assets/dc9cff05-ed12-46ab-ad6c-603f45050812)
### Output Folder: DS_Folder_Load_Files_Incrementally_Destination
![image](https://github.com/user-attachments/assets/5b554fad-4df7-4ac0-aa19-4591f9c89a05)
## Pipeline Trigger Execution
![image](https://github.com/user-attachments/assets/df761dd7-ca53-4755-b059-0067790f2e25)
## Input Files (Sample)
![image](https://github.com/user-attachments/assets/756fe0c1-d323-4659-ac9e-990ede75b8f7)
## Output After Incremental Load
### Before Execution
![image](https://github.com/user-attachments/assets/b45b8ea3-09a9-425c-bc2d-1906222309b5)
### After Execution
![image](https://github.com/user-attachments/assets/61df00a7-4e57-4f8b-9ded-90c99c733157)






