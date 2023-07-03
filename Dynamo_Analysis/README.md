# Dynamo Consult-Project

Prepation of the Data for Analysis
==================================
This project is a combination of database creation and data analysis.The database 
was created using MySQL and the script to build the database is
named Dynamo_Consult_DB.sql and it is available in this repository.
After the creation of the database,the 5 tables of the database were exported 
into microsoft excel and all duplicates were removed and other cleaning tasks were
performed to prepare the data for proper analysis. 

Prerequisite for Running the files
===================================

To run the Dynamo_Consult_DB.sql,you will need to have MySQL installed on your system
and the Dynamo_Consult_Report.pdf can be read with any PDF reader while every other file
can be read using any text editor like notepad.

Use of Power Pivot in Microsoft Excel
=====================================
Based on the fact that the dataset involves multiple tables and not just a single flat
file,the use of Power Pivot becomes very important in order to create relationships
between the tables and also for ease of building pivot table from the multiple tables.

Calculated Columns in the Power Pivot
=====================================

In the Students table, there are 2 columns used in the analysis that were not explicitly 
given in the original database but were calculated using analytics function:
The first one is IF function that was created to categorize students based on the completion 
time of their programs.                                                  
The IF formula used is as shown below:

=IF([enddate] >=TODAY(),"on-going","graduated")

The second one is the FORMAT function that was used to generate the abbreviated month name 
from the [startdate] column.The formula used is as shown below:

=FORMAT([startdate],"MMM")


The Dynamo Consult Data Analysis Report                                                                                      
=======================================
This is a compilation of different visuals that shows the relationship between the different fields 
used in the various parts of the analysis, the meaningful inferences that 
can be drawn from the visuals and likely suggestions to the decision-makers in the IT School(Dynamo Consult) 
so as to help the company maximize profit by increased sales, 
better customers’ experience and overall satisfaction of all the Dynamo Consult stakeholders.

