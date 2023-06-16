# Data_Analysis-Project1
Prerequisite for Running the files
To view the downloaded Contoso Sales and the Contoso Sales – Original file which are .pbix files on your local device, you will need to install the Power BI software on your system and for the report file which is in PDF format, a PDF reader is needed.

Data Analysis Using Power BI
============================

In the Sales table, there are 2 measures used in the analysis that were not explicitly given in the original power BI file but were calculated using the formulae below:

Net Sales = SUM (Sales [SalesAmount]) - SUM (Sales [ReturnAmount]) - SUM(Sales[DiscountAmount])

Profit = SUM(Sales[SalesAmount]) - ( SUM(Sales[TotalCost])+ SUM(Sales[DiscountAmount]) + SUM(Sales[ReturnAmount]))

In addition to the above measures, in order to have a field that shows both the specific Years alongside their corresponding quarters available for analysis, a new field(column) was created. The new field is in the Calendar table and was named "YearQuarter ".                                           The formula for the new field is as shown below:

YearQuarter = Calendar[Year] & "-" & SWITCH(Calendar[QuarterOfYear],1,"Qtr1",2,"Qtr2",3,"Qtr3",4,"Qtr4")

The above formula concatenates the contents of the "Year " column and that of the "QuarterOfYear " column in the Calendar table. However, there was a small tweak to the final result using the "SWITCH " function which ensures the Quarter value in the "QuarterOfYear " column does not just appear as 1,2,3,4 but as "Qtr1","Qtr2","Qtr3" and "Qtr4" respectively for a better understanding of what the new field represents in the visuals where they were used.

The Contoso Data Analysis Report                                                                                      
================================
This is a compilation of different visuals that shows the relationship between the different fields used in the various parts of the analysis, the meaningful inferences that can be drawn from the visuals and likely suggestions to the decision-makers in the CONTOSO company so as to help the company maximize profits by increased sales, better customers’ experience and overall satisfaction of all the CONTOSO stakeholders.

