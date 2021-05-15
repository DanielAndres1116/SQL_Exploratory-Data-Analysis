# SQL_Exploratory-Data-Analysis

#### Note: If you can't see the notebook here, prove clicking this link: https://nbviewer.jupyter.org/github/DanielAndres1116/SQL_Exploratory-Data-Analysis/blob/main/SQL_ExploratoryDataAnalysis.ipynb

### Dataset Description
I used three datasets and are available on the on the city of Chicago's Portal. 

The first dataset contains a selection of six socioeconomic indicators of public health significance and a "hardship index" of each Chicago community area. The second dataset shows all school level performance data used to create School Report Cards. and The third dataser reflects reported incidents of crime that occurred in the City of Chicago. Due this last dataset is quite larger, for the purposes of this exercise I used a much smaller sample of this dataset, and it is a subset of the original dataset.

On the notebook are explained more details of the datasets and also are shown the links where we can download it. 

### Objectives
Understand the 3 datasets in question, load it into 3 tables in Watson Studio Platform in the section of Db2 database and execute SQL queries to the datasets. To communicate with SQL Databases from within a JupyterLab Notebook. I used the SQL "magic" provided by the ipython-sql extension.

Pd: In the lab environment provided for this exercise in the course, the ipython-sql extension is already installed and so is the ibm_db_sa driver. In a new environment, would be neccesary install this depending of the page where be the databases. 

To analyze the data using SQL, the datasets were stored in a database on Cloud of IBM Watson Studio Platform before. For this is necesary create an account on IBM Watson Studio and obtain an username and password and call my created Service Credentials for my Db2 instance. This process is better explained on the notebook. Depending on the web page where be the cloud and its databases, this part will change. 

I put in practice different types of queries to the data as:

- Count the number of crimes
- Count how many crimes involve an arrest
- Find out which unique types of crimes have been recorded at Gas Station locations
- Retrieve the Community Areas whose names start with certain letter
- Obtain which schools in certain Community Areas are healthy school certified
- Calculate the average school safety score
- Make a list of the top 5 Community Areas by average College Enrollment [number of students]
- Determine which Community Area has the least value for school Safety Score
- Find the Per Capita Income of the Community Area which has a School Safety Score of 1. 


### Conclusions

The SQL-queries are very useful to explore and understand whatever type of datasets. An it is possible make queries to datasets inside databases on cloud. Due the commands and functions that we can execute using SQL, we are able to make great Exploratory Analysis of the datasets. 




