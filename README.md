# Prepation in Alteryx
tools used to prepare and clean the data before analysis
## 1) Auto Field
Use Auto Field to set the field type to the smallest possible size relative to the data contained within the column.  
The tool correctly assigns a numeric field to a string data type where any record starts with zero and not a number.  

## 2) Samples
Use Sample to limit the data stream to a specified number, percentage, or random set of rows. In addition, the Sample tool applies the selected configuration to the columns selected to group by.  
## 3) Oversampled Field
Without increasing the number of records it can over amplify one specif value.  
Example- You are working with a dataset of customer credit card transactions, and you want to detect fraudulent transactions. However, the dataset is highly imbalanced, with very few fraudulent transactions compared to legitimate ones. here we can use oversampled field to correct the imbalance.  

## 4) Create Samples
Use Create Samples to split the input records into 2 or 3 random samples. In the tool, you specify the percentage of records that are in the estimation and validation samples. If the total is less than 100%, the remaining records fall in the holdout sample.  

## 5) Random % Samples  
*Random N Records:* Select a value for Number of Records to specify the number of records to output.  
*Random N% of Records:* Select a value for Percent of Records to specify the percentage of incoming records to output.  
*Deterministic Output:* Select a value for Random Seed to ensure the same set of random results is returned each time you run the workflow (as long as the random seed is the same at runtime).  

## 6) Data Cleansing  
Use Data Cleansing to fix common data quality issues. You can replace/remove null values, remove unwanted characters, modify capitalization/case.  

