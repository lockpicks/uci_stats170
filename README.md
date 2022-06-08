## STATS 170 2022: UC Irvine Capstone Project in Data Science 

### Project Title: Trends in Antibiotic Prescribing in COVID-19 & Upper Respiratory Infection Patients Over Time

### Team members: Ashmita Sawhney, Jeein Kim, Shreya Kini



## File Descriptions: 
1. URI_patients.sql: SQL script in order to extract the required sub-cohort (URI patients) from the raw data file
2. URI_outpatients.sql: SQL script in order to extract the required sub-cohort from URI patients, and filter it for outpatients only
3. Antibiotics.sql: SQL script that stores a culmination of prescription of 15 antibiotics to all URI & COVID outpatients 
4. Comorbidity.sql: SQL script to extract and store presence of all comorbidities for each patient 
5. Final_table.sql: SQL script that gathers final dataset used: including demographic data, comorbidity presence & antibiotic status 
6. assumptions.r: R code for checking assumptions that are needed for logistic regression
7. stats_model_1.r: Logistic regression model (LRM) using explanatory variables including only demographic data 
8. stats_model_2.r: LRM using explanatory variables including demographic data and all comorbidities 
9. stats_model_3.r: LRM using explanatory variables including demographic data and all comorbidities, plus time covariates 
10. visualizations.r: R code containing relevant visualizations for data analysis


## How to run our project:

Note: Since we used restricted data in our project that cannot be shared, we did not reproduce SQL code since there were >15 tables and billions of rows that were taken into account. All SQL script was run against N3C database that has strict rules on downloading data and/or duplicating tables from their database. As a result, we created a sample of the final dataset that was extracted after applying all exclusion criteria, and generated examples of the types of analyses and predictions our model can make. To run the R code:

  1. Download the file "Sample_Data.csv"
  2. Download the R markdown file "Stats 170 Final Project.Rmd" 
  3. Make sure both these files are in the same directory
  4. Run each codechunk sequentially to view modeling results and other visualizations
  5. To view output of all cells in the notebook, download the .html version of our notebook called "project.html" 



