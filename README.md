# Data-Analyst-Sonali-Rajasekara
Water Quality project
1. Exploratory Data Analysis (EDA)

•	Project Description: Exploring and understanding the underlying patterns in water quality data pertaining to Vancouver City collected from various sensors.

•	Project Title: Exploratory Analysis of Water Quality Data

•	Objective: To explore the data for general trends, patterns, and missing values, providing an initial understanding of key attributes like temperature and turbidity so that Vancouver City and health authorities can respond more effectively to incidents, mitigate health risks.

•	Dataset: This dataset contains all operating permits issued from the inception of the operating permit program to present, 2019-present. It also contains a full historical record of water quality reports. Water quality data with attributes like temperature, turbidity, and year was collected from https://opendata.vancouver.ca/explore/dataset/operating-permits-water-systems-water-quality-reports/information/.

•	Methodology: Summary statistics, relationship among variables were observed using the analysis tab of https://opendata.vancouver.ca/explore/dataset/operating-permits-water-systems-water-quality-reports/analyze/?dataChart=eyJxdWVyaWVzIjpbeyJjaGFydHMiOlt7InR5cGUiOiJiYXIiLCJmdW5jIjoiQ09VTlQiLCJ5QXhpcyI6InR1cmJpZGl0eSIsInNjaWVudGlmaWNEaXNwbGF5Ijp0cnVlLCJjb2xvciI6InJhbmdlLWN1c3RvbSJ9XSwieEF4aXMiOiJzeXN0ZW1fcmVwb3J0X2RhdGUiLCJtYXhwb2ludHMiOiIiLCJ0aW1lc2NhbGUiOiJ5ZWFyIiwic29ydCI6IiIsInNlcmllc0JyZWFrZG93biI6Im1lY2hhbmljYWxfc3lzdGVtX3R5cGUiLCJjb25maWciOnsiZGF0YXNldCI6Im9wZXJhdGluZy1wZXJtaXRzLXdhdGVyLXN5c3RlbXMtd2F0ZXItcXVhbGl0eS1yZXBvcnRzIiwib3B0aW9ucyI6e319fV0sImRpc3BsYXlMZWdlbmQiOnRydWUsImFsaWduTW9udGgiOnRydWV9. 

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

•	Tools and Technologies: Python Library -pandas, Numpy, Visualization libraries like matplotlib, seaborn, Correlation metrics using corre() ,  Statistical significance tests. AWS Glue 

•	Deliverables: Visual and statistical reports showing key patterns and correlations in the dataset over the time 

Figure 1

Figure 2- 

Figure 3- 

Figure 4 

Figure 4.1
 
2. Descriptive Analysis

•	Project Description: Exploring and understanding the underlying patterns in water quality data pertaining to Vancouver City collected from various sensors.

•	Project Title: Exploratory Analysis of Water Quality Data

•	Objective: To explore the data for general trends, patterns, and missing values, providing an initial understanding of key attributes like temperature and turbidity so that Vancouver City and health authorities can respond more effectively to incidents, mitigate health risks.

•	Dataset: This dataset contains all operating permits issued from the inception of the operating permit program to present, 2019-present. It also contains a full historical record of water quality reports. Water quality data with attributes like temperature, turbidity, and year was collected from https://opendata.vancouver.ca/explore/dataset/operating-permits-water-systems-water-quality-reports/information/.

•	Methodology: 

Step 1- Data Storage: 
The data was first stored in AWS S3 (Figure 5), providing a secure and scalable storage solution.

Step 2- Data Visualization:
AWS QuickSight was intended for data visualization, but due to access limitations, Excel was used for visualization (Figure 6).

Step 3- Internal Publishing: 
The data visualization was published on a general server for internal users (Figure 7,8 ), allowing restricted access to the organization using a Windows remote desktop

Step 4- Public Publishing:
 Finally, the visualization was made accessible to the public using a web server hosted on AWS EC2 (Figure 9, 10 ), ensuring broader accessibility.

•	Tools and Technologies: AES S3, AWS Glue, AWS QuickSight for visualizations, Excel,  AWS EC2, Windows remote desktop. (Figure 11) 

•	Deliverables: Summary tables, charts representing the average and range of water quality variables.

Figure 5

Figure 6

Figure 7

Figure 8

Figure 9

Figure 10

Figure 11
 
3. Diagnostic Analysis

• Project Description: Diagnostic analysis to identify the reasons for missing or incomplete data in the water quality dataset pertaining to Vancouver City collected from various sensors 

• Project Title: Diagnostic Analysis of Incomplete Water Quality Data

•	Objective: To investigate and identify the causes of missing values and inconsistencies in the water quality data.

•	Dataset: This dataset contains all operating permits issued from the inception of the operating permit program to present, 2019-present. It also contains a full historical record of water quality reports. Water quality data with attributes like temperature, turbidity, and year was collected from https://opendata.vancouver.ca/explore/dataset/operating-permits-water-systems-water-quality-reports/information/. 

•	Methodology: Anomaly detection methods, data validation, and rule engine checks.

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

•	Tools and Technologies: AWS Glue,AWS Glue Logs,  AWS S3, AWS CloudWatch AWS Cloudwatch Logs, Data Lineage tracing. 

•	Deliverables: Detailed reports on the cause of data inconsistencies and recommendations to address these issues.

•	Timeline: 1 week to investigate, followed by a week for reporting.

Figure 12

Figure 13

Figure 14

Figure 15

Figure 16

Figure 17
 
4. Data Wrangling
   
•	Project Description: Data cleaning and preparation of water quality data for advanced analysis.

•	Project Title: Data Wrangling for Water Quality Data Analysis pertaining to Vancouver City collected from various sensors

•	Objective: To clean and prepare water quality data by handling missing values, reorganizing columns, and applying necessary transformations.

•	Dataset: This dataset contains all operating permits issued from the inception of the operating permit program to present, 2019-present. It also contains a full historical record of water quality reports. Water quality data with attributes like temperature, turbidity, and year was collected from https://opendata.vancouver.ca/explore/dataset/operating-permits-water-systems-water-quality-reports/information/. 

•	Methodology

Step 1- Data Ingestion: 
The data ingestion process for 2024 involves transferring data from an operational environment to an analytical environment by uploading it to landing folders within Amazon S3. The "Standard" storage class is chosen for its cost-effectiveness and ability to handle frequent daily access, ensuring both performance and reliability. (Figure 18) 

Step 2- Data Cleaning
Using AWS DataBrew, missing rows for "Temperature" and "Turbidity" were deleted to ensure data quality.(Figure 19, Figure 21)

Step 3- Data Structuring 
Additional structuring was performed with AWS DataBrew. Columns were renamed to match analysis objectives, and the "System report date" column was changed to a date format. The year was extracted from this column to focus on yearly metrics, optimizing the dataset for further analysis.(Figure 20, Figure 21) 

Step 4- Storing Cleaned data in Raw folders 
This refinement process resulted in a cleaner, more reliable dataset, properly organized and ready for further analysis or processing and this data was stored in Raw folder.

•	Tools and Technologies: AWS Glue, AWS DataBrew.

•	Deliverables: A cleaned and structured dataset ready for further analysis stored in the Raw folder

•	Timeline: 2 weeks, including validation and final clean data delivery.

Figure 18

Figure 19 

Figure 20

Figure 21
 
5. Data Quality Control

•	Project Description: Data Quality Control to ensure data consistency and completeness of water quality data pertaining to Vancouver City .

•	Project Title: Data Quality Control for Water Quality Data pertaining to Vancouver City

•	Objective: To apply data quality rules and ensure that water quality data meets completeness and consistency requirements.

•	Methodology: 

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

•	Deliverables: A final dataset with 95% completeness in key attributes, ensuring quality for further analysis.

•	Timeline: 1 week for rule application and validation.

Figure 22

Figure 23

Figure 24

Figure 25
 






