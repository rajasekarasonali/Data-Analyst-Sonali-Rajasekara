# Data-Analyst-Sonali-Rajasekara
## Project 1- Water Quality project


### 1. Exploratory Data Analysis (EDA)

#### •	Project Description
Exploring and understanding the underlying patterns in water quality data pertaining to Vancouver City collected from various sensors.

#### •	Project Title
Exploratory Analysis of Water Quality Data

#### •	Objective
To explore the data for general trends, patterns, and missing values, providing an initial understanding of key attributes like temperature and turbidity so that Vancouver City and health authorities can respond more effectively to incidents, mitigate health risks.

#### •	Dataset
This dataset contains all operating permits issued from the inception of the operating permit program to present, 2019-present. It also contains a full historical record of water quality reports. Water quality data with attributes like temperature, turbidity, and year was collected from https://opendata.vancouver.ca/explore/dataset/operating-permits-water-systems-water-quality-reports/information/.

#### •	Methodology
Summary statistics, relationship among variables were observed using the analysis tab of https://opendata.vancouver.ca/explore/dataset/operating-permits-water-systems-water-quality-reports/analyze/?dataChart=eyJxdWVyaWVzIjpbeyJjaGFydHMiOlt7InR5cGUiOiJiYXIiLCJmdW5jIjoiQ09VTlQiLCJ5QXhpcyI6InR1cmJpZGl0eSIsInNjaWVudGlmaWNEaXNwbGF5Ijp0cnVlLCJjb2xvciI6InJhbmdlLWN1c3RvbSJ9XSwieEF4aXMiOiJzeXN0ZW1fcmVwb3J0X2RhdGUiLCJtYXhwb2ludHMiOiIiLCJ0aW1lc2NhbGUiOiJ5ZWFyIiwic29ydCI6IiIsInNlcmllc0JyZWFrZG93biI6Im1lY2hhbmljYWxfc3lzdGVtX3R5cGUiLCJjb25maWciOnsiZGF0YXNldCI6Im9wZXJhdGluZy1wZXJtaXRzLXdhdGVyLXN5c3RlbXMtd2F0ZXItcXVhbGl0eS1yZXBvcnRzIiwib3B0aW9ucyI6e319fV0sImRpc3BsYXlMZWdlbmQiOnRydWUsImFsaWduTW9udGgiOnRydWV9. 

Step 1:Forming question /metric of interest,   and Data Preparation
The metric /question of interest is the Relationship between average turbidity with Temperature over the time.
Inspect the data: Review the dataset to ensure that turbidity and temperature values are recorded properly and no fields are missing.
Handle missing data: If there are any missing values for Turbidity or Temperature, decide on a method to handle them (e.g., removing rows, imputing with averages).
Convert units (if necessary): If temperature or turbidity is recorded in different units, make sure they are consistent across all entries.

Step 2: Calculate Average Turbidity for Each Temperature (Figure 4, Figure 4.1  )
Group data by temperature: Group the dataset based on the temperature column.
Calculate average turbidity: For each group (i.e., each temperature level), calculate the average turbidity.

Step 3: Visualize the Relationship (Figure 1, Figure 2) 
Create a scatter plot or line graph: Plot the average turbidity values on the Y-axis and the temperature values on the X-axis to visualize the relationship.

Step 4: Statistical Analysis (Figure 3) 
Calculate correlation coefficient: Use a statistical test like Pearson’s correlation to measure the strength and direction of the relationship between turbidity and temperature.

Step 5: Interpret Results
Review correlation and regression outcomes: Based on the analysis (correlation and regression), interpret whether temperature significantly impacts turbidity.
Discuss potential factors: Consider any external factors that might influence the relationship between turbidity and temperature (e.g., seasonal variations and system maintenance).

#### •	Tools and Technologies
Python Library -pandas, Numpy, Visualization libraries like matplotlib, seaborn, Correlation metrics using corre() ,  Statistical significance tests. AWS Glue 

#### •	Deliverables
Visual and statistical reports showing key patterns and correlations in the dataset over the time 

Figure 1
![F 1](https://github.com/user-attachments/assets/9f2d3761-5353-41ed-9e5f-2927aa445f2d)

Figure 2- 
![F 2](https://github.com/user-attachments/assets/a9916883-82ca-4ad3-85a2-e94006adf387)

Figure 3- 
![F 3](https://github.com/user-attachments/assets/b9007600-299e-499b-9772-1e401e52d33b)

Figure 4 
![F 4](https://github.com/user-attachments/assets/7d219bf5-847a-414f-8a42-6e649c50cf9d)

Figure 4.1
![F 4 1](https://github.com/user-attachments/assets/af1c2e00-f87b-4fe9-9aca-3be4e8f228f7)


### 2. Descriptive Analysis

#### •	Project Description
Exploring and understanding the underlying patterns in water quality data pertaining to Vancouver City collected from various sensors.

#### •	Project Title
Exploratory Analysis of Water Quality Data

#### •	Objective
To explore the data for general trends, patterns, and missing values, providing an initial understanding of key attributes like temperature and turbidity so that Vancouver City and health authorities can respond more effectively to incidents, mitigate health risks.

#### •	Dataset
This dataset contains all operating permits issued from the inception of the operating permit program to present, 2019-present. It also contains a full historical record of water quality reports. Water quality data with attributes like temperature, turbidity, and year was collected from https://opendata.vancouver.ca/explore/dataset/operating-permits-water-systems-water-quality-reports/information/.

#### •	Methodology: 

Step 1- Data Storage: 
The data was first stored in AWS S3 (Figure 5), providing a secure and scalable storage solution.

Step 2- Data Visualization:
AWS QuickSight was intended for data visualization, but due to access limitations, Excel was used for visualization (Figure 6).

Step 3- Internal Publishing: 
The data visualization was published on a general server for internal users (Figure 7,8 ), allowing restricted access to the organization using a Windows remote desktop

Step 4- Public Publishing:
 Finally, the visualization was made accessible to the public using a web server hosted on AWS EC2 (Figure 9, 10 ), ensuring broader accessibility.

#### •	Tools and Technologies
AES S3, AWS Glue, AWS QuickSight for visualizations, Excel,  AWS EC2, Windows remote desktop. (Figure 11) 

#### •	Deliverables
Summary tables, charts representing the average and range of water quality variables.

Figure 5
![F 5](https://github.com/user-attachments/assets/99e77062-9469-400c-aa38-41a8534fee48)

Figure 6
![F 6](https://github.com/user-attachments/assets/070dd595-8098-41b9-bf50-5735d88d0e2f)

Figure 7
![F 7](https://github.com/user-attachments/assets/131ee393-c9a7-46b5-94ed-704c129894de)

Figure 8
![F 8](https://github.com/user-attachments/assets/229cd6c9-793c-4cb9-adb3-112c9c5c974e)

Figure 9
![F 9](https://github.com/user-attachments/assets/a13e0abe-35a1-4eeb-954e-ba36dddf1e5e)

Figure 10
![F 10](https://github.com/user-attachments/assets/4e303733-2ee2-47bb-bc95-46ceacd05871)

Figure 11

![F 11](https://github.com/user-attachments/assets/226f8587-60a3-47f8-8822-4c4f9fe39086)

 
### 3. Diagnostic Analysis

#### • Project Description
Diagnostic analysis to identify the reasons for missing or incomplete data in the water quality dataset pertaining to Vancouver City collected from various sensors 

#### • Project Title
Diagnostic Analysis of Incomplete Water Quality Data

#### •	Objective
To investigate and identify the causes of missing values and inconsistencies in the water quality data.

#### •	Dataset
This dataset contains all operating permits issued from the inception of the operating permit program to present, 2019-present. It also contains a full historical record of water quality reports. Water quality data with attributes like temperature, turbidity, and year was collected from https://opendata.vancouver.ca/explore/dataset/operating-permits-water-systems-water-quality-reports/information/. 

#### •	Methodology
Anomaly detection methods, data validation, and rule engine checks.

Step 1- Data Ingestion: 
The data ingestion process for 2024 involves transferring data from an operational environment to an analytical environment by uploading it to landing folders within Amazon S3. The "Standard" storage class is chosen for its cost-effectiveness and ability to handle frequent daily access, ensuring both performance and reliability.(Figure 12) 

Step 2- Data Validation: 
Validate the ingested data to ensure its completeness and accuracy by Conducting rule engine checks to identify any missing values or incorrect data entries using AWS Databrew and AWS Glue to clean, transform, and prepare the data for further analysis. (Figure 13, 14, 15, 16,17)

Step 3 - Anomaly detection:
Detect anomalies or irregularities in the dataset that could indicate errors or issues by applying anomaly detection techniques to explore patterns, check for outliers, and identify inconsistencies in the water quality dataset.

Step 4 -Root Course Analysis:
Identify the underlying reasons for missing or incomplete data by Investigate data pipelines, sensor data collection processes, and external factors that may have led to missing or inconsistent data entries.

Step 5 -Reporting and Recommendations:
Document the findings and provide actionable insights by generating detailed reports summarizing the causes of data inconsistencies and offering recommendations to prevent future issues

#### •	Tools and Technologies
AWS Glue,AWS Glue Logs,  AWS S3, AWS CloudWatch AWS Cloudwatch Logs, Data Lineage tracing. 

#### •	Deliverables
Detailed reports on the cause of data inconsistencies and recommendations to address these issues.

#### •	Timeline
1 week to investigate, followed by a week for reporting.

Figure 12
![F 12](https://github.com/user-attachments/assets/98e627ee-94fb-4f7e-8607-d287a2a79fad)

Figure 13
![F 13](https://github.com/user-attachments/assets/38e81df4-1ad5-4832-92ae-61c626a26aba)

Figure 14
![F 14](https://github.com/user-attachments/assets/06a389ff-bf4b-4f3e-90f3-1a0df0f979a0)

Figure 15
![F 15](https://github.com/user-attachments/assets/f5e66234-ce92-4c94-9a6a-357d0e23e0a1)

Figure 16
![F 16](https://github.com/user-attachments/assets/eb050488-94b6-4b42-b658-d9e111d5f281)

Figure 17
![F 17](https://github.com/user-attachments/assets/5a90e7e6-a251-4584-b6d3-68fcbf978ba7)

 
### 4. Data Wrangling
   
#### •	Project Description
Data cleaning and preparation of water quality data for advanced analysis.

#### •	Project Title
Data Wrangling for Water Quality Data Analysis pertaining to Vancouver City collected from various sensors

#### •	Objective
To clean and prepare water quality data by handling missing values, reorganizing columns, and applying necessary transformations.

#### •	Dataset
This dataset contains all operating permits issued from the inception of the operating permit program to present, 2019-present. It also contains a full historical record of water quality reports. Water quality data with attributes like temperature, turbidity, and year was collected from https://opendata.vancouver.ca/explore/dataset/operating-permits-water-systems-water-quality-reports/information/. 

#### •	Methodology

Step 1- Data Ingestion: 
The data ingestion process for 2024 involves transferring data from an operational environment to an analytical environment by uploading it to landing folders within Amazon S3. The "Standard" storage class is chosen for its cost-effectiveness and ability to handle frequent daily access, ensuring both performance and reliability. (Figure 18) 

Step 2- Data Cleaning
Using AWS DataBrew, missing rows for "Temperature" and "Turbidity" were deleted to ensure data quality.(Figure 19, Figure 21)

Step 3- Data Structuring 
Additional structuring was performed with AWS DataBrew. Columns were renamed to match analysis objectives, and the "System report date" column was changed to a date format. The year was extracted from this column to focus on yearly metrics, optimizing the dataset for further analysis.(Figure 20, Figure 21) 

Step 4- Storing Cleaned data in Raw folders 
This refinement process resulted in a cleaner, more reliable dataset, properly organized and ready for further analysis or processing and this data was stored in Raw folder.

#### •	Tools and Technologies
AWS Glue, AWS DataBrew.

#### •	Deliverables
A cleaned and structured dataset ready for further analysis stored in the Raw folder

#### •	Timeline
2 weeks, including validation and final clean data delivery.

Figure 18
![F 18](https://github.com/user-attachments/assets/14892ecb-7c8a-4c18-aebe-b72281bc04a0)

Figure 19 
![F 19](https://github.com/user-attachments/assets/f49bac0d-d436-4a7f-84f5-cd75b3bd01b4)

Figure 20
![F 20](https://github.com/user-attachments/assets/6fc089ab-7859-4598-b7b3-037746d2ff6f)

Figure 21

![F 21](https://github.com/user-attachments/assets/2277a8be-5f90-4a48-b917-03e72cbde6af)

 
### 5. Data Quality Control

#### •	Project Description
Data Quality Control to ensure data consistency and completeness of water quality data pertaining to Vancouver City .

#### •	Project Title
Data Quality Control for Water Quality Data pertaining to Vancouver City

#### •	Objective
To apply data quality rules and ensure that water quality data meets completeness and consistency requirements.

#### •	Methodology: 

Step 1: Data Governance Setup
Establish a framework for managing data quality and privacy. AWS Glue Studio is used as the ETL service. A "Trusted Zone" is created in Amazon S3 after the "Curated Zone" to store data that meets data quality and privacy rules. Figure (22) 

Step 2: Data Quality Rule Definition
Set data quality standards by defining custom rules in the rule engine to check for completeness, freshness, and uniqueness in the data. In this case, only the completeness rule is applied for the following columns (Figure23) 
"year" > 0.95: Checks if more than 95% of values in the "year" column are non-null.
"temperature" > 0.95: Checks if more than 95% of values in the "temperature" column are non-null.
"avgturbidity" > 0.95: Ensures that more than 95% of values in the "avgturbidity" column are non-null.

Step 3: Data Quality Check
Evaluate the dataset for completeness using AWS Glue Studio which applies the rules defined in Step 2 to assess the completeness of key columns. Freshness and uniqueness checks are not performed for this dataset.

Step 4: Separating Data Based on Quality
Data that passes both the privacy and quality checks is saved in a Trusted Zone within an S3 bucket, while data that fails is saved separately for further review. (Figure 24) 

Step 5: ETL Job Execution and Scheduling
Run the data governance job using AWS Glue (Figure 25) 

#### •	Deliverables
A final dataset with 95% completeness in key attributes, ensuring quality for further analysis.

#### •	Timeline
1 week for rule application and validation.

Figure 22

![F 22](https://github.com/user-attachments/assets/e2ec680f-ec1a-49d1-9ef8-4704292402ae)

Figure 23
![F 23](https://github.com/user-attachments/assets/5cf83682-ec1c-4880-a6ef-f5134f25fa41)

Figure 24
![F 24](https://github.com/user-attachments/assets/26a48662-6096-4b51-afef-270dbfefd8ce)

Figure 25
![F 25](https://github.com/user-attachments/assets/560b4f60-fc20-48e2-a1c7-8fb328a665f1)



## Project 2- UCW project for HR departments (Professional development )


### 1. Exploratory Data Analysis
   
#### 	Project Description:
This analysis investigates the trends and characteristics of professional development approvals and reimbursements at University Canada West in 2024. 

#### •	Project Title:
Exploratory Analysis of Professional Development Approvals and Reimbursements for 2024 at UCW

#### •	Objective:
To explore the distribution and trends of professional development approvals and reimbursements and identify any significant patterns in the dataset.

#### •	Dataset:
Professional Development approvals and reimbursement data from the UCW HR office for the year 2024.(Figure a) 

#### •	Methodology:

Step 1:Forming question /metric of interest,   and Data Preparation
The metric /question of interest is the Percentage of Approvals done for 2024 in professional development domain
Inspect the data: Review the dataset to ensure that data are recorded properly and no fields are missing.
Handle missing data: If there are any missing values decide on a method to handle them (e.g., removing rows, imputing with averages).
Convert units (if necessary)

Step 2: Calculate Percentage of Approvals for Professional development data (Figure 4, Figure 4.1  )
Group data by year: Group the dataset based on the year column.
Calculate percentage of Approvals: For each year 

Step 3: Visualize the Metric (Figure 1, Figure 2) 
Create a line chart to investigate the trends in Approval rate over time. 

Step 4: Statistical Analysis 
Examining the statistical significance  of the trend of percentage Approvals. 

Step 5: Interpret Results
Review and interpret the yearly trends of Approval rates 
Discuss potential factors: Consider any external factors that might influence the identified behavior. 

#### •	Tools and Technologies:
Python Library -pandas, Numpy, Visualization libraries like matplotlib, seaborn, Line charts ,  Statistical significance tests. AWS Glue 

#### •	Deliverables:
Data visualizations showing trends in approvals and reimbursements
Summary report identifying key patterns in the data

Figure a
![Figure  a  ](https://github.com/user-attachments/assets/ea04bfe6-3b6d-4d95-97f6-a082c13f1add)

Figure 1

![F 1 ](https://github.com/user-attachments/assets/2ee16a3d-e763-48cd-8934-f93d7f568103)

Figure 2- 
![F 2 ](https://github.com/user-attachments/assets/d512d003-d567-466d-a908-0257c853a23f)

Figure 4 
![F 4](https://github.com/user-attachments/assets/1d8f4405-0082-446a-a86b-b484c2776a2d)

Figure 4.1
 ![F 4 1](https://github.com/user-attachments/assets/0d9e8d93-a779-4e23-9f0c-857ad962c9a3)


### 2. Descriptive Analysis

#### •	Project Description:
This analysis summarizes the approval and reimbursement data, focusing on central tendencies, variations, and frequency of professional development activities undertaken by staff members of UCW.

#### •	Project Title:
Descriptive Summary of UCW Professional Development Approvals and Reimbursements for UCW Staff

#### •	Objective:
To describe the total number of professional development activities approved, total reimbursements made, and their distribution across various staff roles and departments.

#### •	Dataset:
Professional Development approvals and reimbursement data from UCW HR for years 2023 and 2024 .

#### •	Methodology:

Step 1- Data Storage: 
The data was first stored in AWS S3 (Figure 5, Figure 5.1), providing a secure and scalable storage solution.

Step 2- Data Visualization:
AWS QuickSight was intended for data visualization, but due to access limitations, Excel was used for visualization 

Step 3- Internal Publishing: 
The data visualization was published on a general server for internal users (Figure 8 ), allowing restricted access to the organization using a Windows remote desktop

Step 4- Public Publishing:
 Finally, the visualization was made accessible to the public using a web server hosted on AWS EC2 (Figure 9, 10 ), ensuring broader accessibility.

#### •	Tools and Technologies: AES S3, AWS Glue, AWS QuickSight for visualizations, Excel,  AWS EC2, Windows remote desktop. (Figure 11) 

#### •	Deliverables:
A detailed report containing summary statistics
Visual dashboards showcasing the breakdown of reimbursements and approvals

Figure 5
![F 5 ](https://github.com/user-attachments/assets/dc213c56-4a2c-4c2e-a4f5-fd3882846209)

Figure 5.1
![F 5 1 ](https://github.com/user-attachments/assets/06e0b902-30dd-4ff8-8bd9-cf0d421b0213)

Figure 8
![F 8 ](https://github.com/user-attachments/assets/d31206f2-1e5e-47d2-8863-5ce046316cfc)

Figure 9
![F 9 ](https://github.com/user-attachments/assets/0ef21d05-6f00-4263-a966-ee10888480c4)

Figure 10
![F 10](https://github.com/user-attachments/assets/1e0d0968-e3c2-4846-87ab-9404bd166c9a)

Figure 11

![F 11](https://github.com/user-attachments/assets/736db6ed-8b07-43f0-b172-da2562f1fe9b)


### 3. Diagnostic Analysis

#### •	Project Description:
A diagnostic analysis was conducted to identify the reasons behind changes or anomalies in professional development approvals and reimbursements in 2024, focusing on identifying potential causes for the observed data trends.

#### •	Project Title:
Diagnostic Analysis of Reimbursement Variations for UCW Staff

#### •	Objective:
To investigate the factors contributing to significant increases or decreases in professional development reimbursements across departments.

#### •	Dataset:
Professional Development approvals and reimbursement data from UCW HR for for years 2023 and 2024 .

#### •	Methodology:

Step 1- Data Ingestion: 
The data ingestion process involves transferring data from an operational environment to an analytical environment by uploading it to landing folders within Amazon S3. The "Standard" storage class is chosen for its cost-effectiveness and ability to handle frequent daily access, ensuring both performance and reliability.(Figure 12) 

Step 2- Data Validation: 
Validate the ingested data to ensure its completeness and accuracy by Conducting rule engine checks to identify any missing values or incorrect data entries using AWS Databrew and AWS Glue to clean, transform, and prepare the data for further analysis. (Figure 13, 14, 17)

Step 3 - Anomaly detection:
Detect anomalies or irregularities in the dataset that could indicate errors or issues by applying anomaly detection techniques to explore patterns, check for outliers, and identify inconsistencies in the water quality dataset.

Step 4 -Root Course Analysis:
Identify the underlying reasons for missing or incomplete data by Investigating data pipelines, the operational environment’s data collection processes, and external factors that may have led to missing or inconsistent data entries.

Step 5 -Reporting and Recommendations:
Document the findings and provide actionable insights by generating detailed reports summarizing the causes of data inconsistencies and offering recommendations to prevent future issues

#### •	Tools and Technologies: AWS Glue,AWS Glue Logs,  AWS S3, AWS CloudWatch AWS Cloudwatch Logs, Data Lineage tracing. 

#### •	Deliverables:
Root cause analysis report on reimbursement rate variations
Recommendations for improving approval consistency

#### •	Timeline: 2 week to investigate, followed by a week for reporting.

Figure 12
![F 12 ](https://github.com/user-attachments/assets/112fa573-c5f2-4735-981d-e619aca8f074)

Figure 13
![F 13 ](https://github.com/user-attachments/assets/f1d3b3bc-3981-437b-9c90-65e9e6d6e768)

Figure 14
![F 14](https://github.com/user-attachments/assets/723407f0-7550-4ebe-a3d0-f447de6b25da)

Figure 17
![F 17](https://github.com/user-attachments/assets/07b4c166-955a-46e9-af64-8b62e08c4653)


### 4. Data Wrangling
   
#### •	Project Description:
The data wrangling phase focused on preparing and cleaning the professional development approval and reimbursement data, ensuring it was suitable for analysis.

#### •	Project Title:
Data Wrangling for UCW Professional Development Approvals and Reimbursements Analysis

#### •	Objective:
To clean and organize professional development data, ensuring completeness, accuracy, and proper formatting for further analysis.

#### •	Dataset:
Professional Development approval and reimbursement data for latest years, containing information on employee IDs, departments, activities, and financial reimbursements.

#### •	Methodology:

Step 1- Data Ingestion: 
The data ingestion process involves transferring data from an operational environment to an analytical environment by uploading it to landing folders within Amazon S3. The "Standard" storage class is chosen for its cost-effectiveness and ability to handle frequent daily access, ensuring both performance and reliability. (Figure 18) 

Step 2- Data Cleaning
Using AWS DataBrew, missing rows for "Year," “Total Applications received,”  and "Number of Applications Approved" was deleted to ensure data quality.(Figure 19, Figure 21)

Step 3- Data Structuring 
Additional structuring was performed with AWS DataBrew. Columns were renamed to match analysis objectives, and the "System report date" column was changed to a date format. The year was extracted from this column to focus on yearly metrics, optimizing the dataset for further analysis.( Figure 21) 

Step 4- Storing Cleaned data in Raw folders 
This refinement process resulted in a cleaner, more reliable dataset, properly organized and ready for further analysis or processing and this data was stored in Raw folder.

#### •	Tools and Technologies:
AWS Glue, AWS DataBrew.

#### •	Deliverables:
Cleaned dataset ready for analysis stored in Raw zone
Documentation of data wrangling steps and decisions

#### •	Timeline: 2 weeks, including validation and final clean data delivery.

Figure 18
![F 18 ](https://github.com/user-attachments/assets/e36c7f28-ac95-42ef-a378-b3de4328cd76)

Figure 19 
![F 19 ](https://github.com/user-attachments/assets/0cf60413-6947-44cc-9807-8ca4baf0373b)

Figure 21

![F 21](https://github.com/user-attachments/assets/64b13666-5ff1-4f75-9803-b20326e7128d)


### 5. Data Quality Control

#### •	Project Description:
This analysis ensures the data used for the project meets required quality standards, focusing on completeness, accuracy, and consistency.

#### •	Project Title:
Data Quality Control for UCW Professional Development Approvals and Reimbursements

#### •	Objective:
To ensure that the professional development approval and reimbursement data is complete, accurate, and consistent.

#### •	Dataset:
Professional Development approval and reimbursement data for latest years, containing information on employee IDs, departments, activities, and financial reimbursements.

#### •	Methodology:

Step 1: Data Governance Setup
Establish a framework for managing data quality and privacy. AWS Glue Studio is used as the ETL service. A "Trusted Zone" is created in Amazon S3 after the "Curated Zone" to store data that meets data quality and privacy rules. Figure (22) 

Step 2: Data Quality Rule Definition
Set data quality standards by defining custom rules in the rule engine to check for completeness, freshness, and uniqueness in the data. In this case, only the completeness rule is applied for the following columns (Figure23) 
"year" > 0.95: Checks if more than 95% of values in the "year" column are non-null.
"employee_Job title" > 0.95: Checks if more than 95% of values in the "temperature" column are non-null.

Step 3: Data Quality Check
Evaluate the dataset for completeness using AWS Glue Studio which applies the rules defined in Step 2 to assess the completeness of key columns. Freshness and uniqueness checks are not performed for this dataset.

Step 4: Separating Data Based on Quality
Data that passes both the privacy and quality checks is saved in a Trusted Zone within an S3 bucket, while data that fails is saved separately for further review. (Figure 23) 

Step 5: ETL Job Execution and Scheduling
Run the data governance job using AWS Glue 

#### •	Deliverables:
A final quality report, ensuring the data met the standards for completeness, accuracy, and consistency

#### •	Timeline:
The data quality process was completed over two weeks, ensuring minimal disruption to the overall analysis.

Figure 22

![F 22](https://github.com/user-attachments/assets/f23e30ee-3b4c-4bb5-b43c-fe853616fcc7)

Figure 23
![F 23 ](https://github.com/user-attachments/assets/cec4f9bc-e987-4fd4-ab2c-3b345aeda5a9)


 






