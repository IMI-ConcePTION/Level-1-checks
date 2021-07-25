# Level 1 checks
## R scripts to check integrity of an ETL to the ConcePTION CDM

**Aims of Level 1 quality checks:**      
**1.**	To assess the integrity of the Extract-Transform-Load(ETL) process from the original data to the [ConcePTION CDM](https://docs.google.com/spreadsheets/d/1hc-TBOfEzRBthGP78ZWIa13C0RdhU7bK/edit#gid=413205035). for each Data Access Provider(DAP).        
**2.**	To provide feedback on the integrity of the ETL to the DAP iteratively for the refinement of the DAP???s ETL procedure.       


***Level 1 data checks review the completeness and content of each variable in each table of the D2 CDM to ensure that the required variables contain data and conform to the formats specified by the CDM specifications (e.g., data types, variable lengths, formats, acceptable values, etc.).*** 

**The level 1 checks are divided in 5 major steps:**   

***Step 1: Check the table formatting***     
Check if all rows of the .csv files in the working directory contain the correct number of fields.    
Check if all variables are present irrespective of their content.    
Check if variables are written in lowercase.     
Check for presence of mandatory variables as according to the CDM.    
Check for presence of non-mandatory variables by comparing between the table of interest and the information recorded in the METADATA table.    
Check presence of vocabularies for specific variables.    
Assess formats for all values and compare to a list of acceptable formats which have been filled out in the METADATA table.     

***Step 2: Missing data analysis***     
Tabulate missingness in all variables, overall and by calendar year (in the tables that contain a date variable).     
Missing data will be further stratified by meaning (in the tables that contain a meaning variable).    
Missing data overall will be displayed using bar charts for each CDM table and reported as counts and percentages.    
Missing data stratified by meaning or calendar year will be displayed using line charts for each CDM table and reported as counts and percentages.    
Missing data stratified by meaning and calendar year will be displayed using heat maps for each CDM table and reported as counts and percentages.     

***Step 3: Dates check***     
Check if dates are in the correct format (8 characters).      
Check if date variables contain allowable values:    
Year: 1995-present (exception for dates that represent end of follow up where years in the future will be allowed.)    
Month: 01-12    
Day: 01-31    

***Step 4: Check conventions and construct frequency tables of other and categorical variables.***    
Check if the table of interest contains any duplicate rows.    
Check that all conventions for the table of interest have been adhered to.     
Construct frequency tables of categorical variables, overall and by calendar year (when the table of interest contains a date variable).     
All frequency tables will be stratified by meaning when the table of interest contains a meaning variable.     
Results will be reported separately for variables with 2 or more categories.    
The results will be displayed graphically with bar charts or line charts.    

***Step 5: Distribution of continuous variables and date variables***    
For continuous variables mean, median, interquartile range, skewness and kurtosis will be reported.     
Distribution of date variables will be reported as counts of dates overall and by calendar year. All results will be stratified by the meaning variable if the table of interest contains one.    
Results will be displayed graphically with bar charts or line charts.    

***Subsection:***
Overview table with information on how counts in step 4 and 5 are being calculated.    

Current version: 5.2.