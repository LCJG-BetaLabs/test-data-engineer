# test-data-engineer

Welcome to the code test for the Data Engineer position!  
  This test aims to evaluate your skills in designing a cost-effective and secure data solution using Databricks, as well as your ability to perform data extraction, transformation, and loading tasks.

## Objectives

1. Define components for data storage, processing, and security, considering different data types.
1. Incorporate suitable tools and technologies aligned with Databricks.
1. Address cost-effectiveness, scalability, and resource utilization.

## Expected time

- < 8 hours

## Scenario

Please write a notebook in Databricks and set up a workflow to obtain data from a MySQL database with the sample table structure below, write the data to Parquet files using Databricks, and store the files in blob storage.
  Additionally, you need to create another workflow that reads the Parquet files and loads the data into tables in Databricks.
  
  Consider the following guidelines:

1. Connect to the MySQL database using appropriate libraries or connectors available in Databricks.
1. Write SQL queries to retrieve the required data from the MySQL database.
1. Transform the retrieved data, if necessary, to prepare it for storage in Parquet format.
1. Write the transformed data to Parquet files using Databricks, ensuring to partition the data appropriately.
1. Store the Parquet files in blob storage (e.g., Azure Blob Storage, AWS S3) for data persistence and scalability.
1. Create a workflow to automate the data extraction, transformation, and loading process, ensuring it runs at specified intervals or triggers.
1. For the second workflow, read the Parquet files from blob storage into Databricks.
1. Load the data from the Parquet files into the member table(s) in Databricks.

Table: Members

- member_id (string) - Unique identifier for each member
- first_name (string) - First name of the member
- last_name (string) - Last name of the member
- email (string) - Email address of the member
- phone_number (string) - Phone number of the member
- address (string) - Address of the member
- city (string) - City where the member resides
- country (string) - Country where the member resides
- registration_date (date) - Date when the member registered

Script to generate data in the member table can be found in the file `generate_member_data.py`.
  Please note that you'll need to install the faker library in your Databricks environment for this script to work.  
  You can install it using the command: `!pip install faker`

  Please provide the notebook code, along with an explanation of each step and function used, to extract the data from the MySQL database, write it to Parquet files, store the files in blob storage, and then read and load the data into tables in Databricks.  

  Please include your considerations for scalability and data security in the given scenario.  

## Submission

Please fork this repository as a private repository and invite __lcjg-betalabstech__ as a collaborator for submission.  
Good luck!

