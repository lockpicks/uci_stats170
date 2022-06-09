The directory `code` contains all codes that were used to extract the de-identified dataset from [N3C platform](https://ncats.nih.gov/n3c), plus codes used for creating visualisations and modelling purposes. 

For demo usage with sample data, please refer to our [main repository](../../).

- `URI_patients.sql`: SQL script in order to extract the required sub-cohort (URI patients) from the raw data file
- `URI_outpatients.sql`: SQL script in order to extract the required sub-cohort from URI patients, and filter it for outpatients only
- `Antibiotics.sql`: SQL script that stores a culmination of prescription of 15 antibiotics to all URI & COVID outpatients
- `Comorbidity.sql`: SQL script to extract and store presence of all comorbidities for each patient
- `Final_table.sql`: SQL script that gathers final dataset used: including demographic data, comorbidity presence & antibiotic status
- `assumptions.r`: R code for checking assumptions that are needed for logistic regression
- `stats_model_1.r`: Logistic regression model (LRM) using explanatory variables including only demographic data
- `stats_model_2.r`: LRM using explanatory variables including demographic data and all comorbidities
- `stats_model_3.r`: LRM using explanatory variables including demographic data and all comorbidities, plus time covariates
- `visualizations.r`: R code containing relevant visualizations for data analysis
