# Crowdfunding ETL Project 
## Introduction
A collaborative project to build an ETL pipeline using Python, Pandas, and PostgreSQL for extracting, transforming, and loading crowdfunding data from Excel files into a regional database.

#### Group Members: 
* Madison Mihle 
* Kat Hardy 
* Lauralee Callahan 

### Methods Used
* Machine Learning
* Exploratory Data Analysis 
* Data Integration and Aggregation 
* Data Extraction 
* Data Transformation and Loading
* Entity Relationship Diagram (ERD) Creation 

### Technologies 
* Visual Code Studio 
    * Pandas 
    * Python 
    * JSON 
* PgAdmin 
    * Postgres SQL 
    * ERD

### Installation 
Required Packages: 
* 'pandas'
* 'numpy'
* 'pprint'
* 'openpyxl'
* 'psycopg2' 

## Background
In this project, we practiced building an ETL pipeline to process crowdfunding data from the Excel files given. The data was extracted and transformed to create four CSV files, and then used to create an Entity Relationship Diagram (ERD) and table schema. The CSV files were loaded into a PostgreSQL database. All data was provided by _edX Boot Camps LLC_, and is intended for educational purposes only.

## Challenge 
### Part 1: Create the Category and Subcategory DataFrames
Data was extracted and transformed from the 'crowdfunding.xlsx' to create a category Dataframe with the following columns: "category_id" and "category". Next, this was exported as the 'category.csv' and saved. Still using the 'crowdfunding.xlsx' data, a subcategory DataFrame was created with the columns: "subcategory_id" and "subcategory". This was also saved as 'subcategory.csv'

### Part 2: Create the Campaign DataFrame
Next, data from the 'crowdfunding.xlsx' to create a campaign DataFrame that has the following columns: 
* "cf_id"
* "contact_id"
* "company_name" 
* "blurb" 
* "goal"
* "pledged" 
* "outcome" 
* "backers_count"
* "country" 
* "currency"
* "launched_at" 
* "deadline" 
* "category_id" 
* "subcategory_id"

This was then exported into the 'campaign.csv' file and saved. 

### Part 3: Create the Contacts DataFrame
Next, using option 1 (Python dictionary method), we extracted and transformed the data from 'contacts.xlsx' data. This was imported into a DataFrame and then iterated by converting each row to a dictionary. The dictionary values were extracted from the keys busing a Python list comprehension. Each of the values from the row was inserted into a new list. A new DataFrame was created from the extracted data. Columns were then split into the appropriate titles. This data was then cleaned and exported as 'contacts.csv' file. 

### Part 4: Create the Crowdfunding Database 
After inspecting the four CSV files, sketch an ERD of the tables. Using the information from the ERD to create a table schema for each CSV file, making sure to add specific data types, primary keys, foreign keys, and other constraints. 

The ERD of the crowdfunding schema is below: 

![alt text](https://github.com/maddieemihle/Crowdfunding_ETL/blob/main/Resources/ERD.png?raw=true) 

## References 
Data for this dataset was generated and provided by _edX Boot Camps LLC_, and is intended for educational purposes only.
