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

## 7) Formula  
Use Formula to create new columns, update columns, and use 1 or more expressions to perform a variety of calculations and operations. Go to Functions for a list of functions to use to create an expression. 
The  Formula tool can  update multiple fields  per tool instance.

## 8) Multi Row Formula  
Use Multi-Row Formula to take the concept of the Formula tool a step further. This tool allows you to use row data as part of the formula creation and is useful for doing  mathematical calculations. 
The Multi-Row Formula tool can only update one field per tool instance. If you would like to update multiple fields, you need to add a Multi-Row Formula tool for each field to be updated.  

## 9) Multi Field Formula  
It is quite similar to  formula tool but here we can update multiple fields of same type in a one go by using expressions.  

## 10) Imputation
Use Imputation to replace a specified value within one or more numeric data fields with another specified value.  

## 11) Select
Use Select to include, exclude, and reorder the columns of data that pass through your workflow. Excluding columns can limit the data that passes through a workflow and improve performance. You can also use the Select tool to modify the type and size of data, rename a column, add a description, and more.

## 12) Select Records
Use Select Records to return records and ranges of records that are specified, including discontinuous ranges of records. This tool is very useful for troubleshooting and sampling.

*Configure the Tool*
Ranges: Enter the records or range of records to return.
A single digit returns only the entered row. For example, "3" returns only row 3.

A minus sign before a number returns row 1 through the entered row. For example, "-2" returns rows 1 and 2.

A range of numbers returns the rows in the range, including the entered rows. For example, "17-20" returns rows 17, 18, 19, and 20.

A number followed by a plus sign returns the entered row through the last row. For example, "50+" returns row 50 through the last row.

Any combination can be used at the same time by entering the numbers on a new line.  


## 13) Generate Rows
Use Generate Rows to create new rows of data at the record level. Use this tool to create a sequence of numbers, transactions, or dates.  

## 14) Record ID
Use Record ID to create a new column in the data and assign a unique identifier, that increments sequentially, for each record in the data. The Record ID tool generates unique identifiers with numeric values or string values, based on the data type you select.  

## 15) Unique
Use Unique to distinguish whether a data record is unique or a duplicate by grouping on one or more specified fields, then sorting on those fields.  

## 16) Sort
is used to sort the fields(ascending/descending)

## 17) Tile
The Tile tool groups datasets by assigning a value (tile) based on ranges in the data. The Tile tool groups datasets using one of the following methods: Equal sum, Equal records, Smart tile, Unique value, and Manual tile
TILE: CONFIGURATION OPTIONS
Equal Records - each tile is assigned the same amount of rows
Equal Sum - tiles with equal total values
Smart Tile - tiles based on Standard Deviation of the values in the specified column
Manual - user assigns tile rules manually
Unique - creates tiles for unique values  

## 18) Multi-Field Binning
Use Multi-Field Binning to replicate some of the functionality of the Tile tool—additional features allow the data to be binned on multiple fields. 
You can bin fields on either equal records or equal intervals.


