# data-analytics-pyspark
Platform Used: Databricks and AWS SageMaker

Methods Used: PySpark (DataFrame, RDD, PySpark SQL) Results: Comprehensive analysis of academic publications including data cleaning, statistical analysis, and visualization.

Detailed Analysis of Academic Publications Using Databricks and AWS SageMaker

Setup Description 1.1 Databricks Setup
Created a new cluster in Databricks workspace.

Uploaded datasets (large_df and journal_df) to Databricks FileStore. Imported libraries (pyspark.sql.functions, matplotlib.pyplot, scipy.stats) for data manipulation and visualization. 1.2 AWS SageMaker Setup

Created an S3 bucket (courseworkassignment1) and uploaded datasets (large_df in JSON, journal_info in CSV). Launched a SageMaker notebook instance (assignment1) and created a new notebook using Conda python3 environment. Utilized boto3 for AWS service interaction and pyspark.sql for Spark session management.

Data Preparation 2.1 Data Cleaning Strategy Handled null values and empty strings in columns (author, journal, IF) to maintain data integrity.
3.1 Unique ID Verification and Dataset Integrity Ensured all papers have unique IDs (CorpusId). Implemented in DataFrame, RDD, and SQL (both Databricks and AWS SageMaker).

3.2 Average Number of Authors per Paper Analysis Calculated the average number of authors per paper (authors column) using DataFrame, RDD, and SQL.

3.3 Count of Different Journals Analysis Identified 33,196 different journals in the dataset using DataFrame, RDD, and SQL.

3.4 Top Authors by Publications Analysis Identified top authors based on publication count using DataFrame, RDD, and SQL.

3.5 Author Impact Analysis Calculated cumulative impact factors for authors based on publication counts using DataFrame, RDD, and SQL.

3.6 Publication Trends Analysis Analyzed publication trends from 2010 to 2020 based on impactful publications using DataFrame, RDD, and SQL.

3.7 Proportion of Impactful Publications Calculated the proportion of impactful publications relative to total publications each year (2010-2020).
