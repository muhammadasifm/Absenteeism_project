# Data Analytics for  Address Absenteeism at a company during work: Project Overview 
* Created a tool that exolore whether a person  presenting certain characteristic is expected to be be away from work at some point in time or not to help to know f or howmany howmany working hours an employee could be away from work
* gather relevent employee data 
* Optimized Linear to reach the  model. 
* obtain the result that will clearly show whether or not each of these individual is expected to be absent for morethan 3 hours during a work day 

## Code and Resources Used 
**Python Version:** 3.10  
**Packages:** pandas, numpy, sklearn,tableau,sql  

## data set
use secondary dataset
*	ID
*	Reason for Absence
*	Date
*	Transportation Expense
*	Distance to Work
*	Age
*	Daily Work Load Average
*	Body Mass Index
*	Education
*	Children
*	Pets
*	Absenteeism Time in Hours

## Data preprocessing
After loading  the data, I needed to clean it up so that it was usable for our model. I made the following changes and created the following variables:

convert the row data into formate that easier to unserstand & usful for processing and analysis
fix the problem that can inevitable occure with data gathering
* mporting the Dataset in Python
* Eyeballing the Data
* Introduction to Terms with Multiple Meanings
* An Analytical Approach to Solving the Task
* Dropping the "ID" Column
* Analysis of the "Reason for Absence" Column
* Converting a Feature into Multiple Dummy Variables
* Working with Dummy Variables from a Statistical Perspective
* Grouping the Various Reasons for Absence
* Concatenating Column Values
* Creating Checkpoints in Jupyter
* Working on the "Date" Column
* Modifying "Education" and Discussing "Children" and "Pets"
* Final Remarks on the Data Preprocessing Part of the Exercise

## EDA
I looked at the distributions of the data and the value counts for the various categorical variables.
organise the information in suitable and practical way


## Model Building 

* Creating the Targets for the Logistic Regression
* Selecting the Inputs for the Regression
* Standardizing the Dataset for Better Results
* Train-test Split of the Data
* Training and Evaluating the Model
* Extracting the Intercept and Coefficients
* Interpreting the Coefficients
* Creating a Custom Scaler to Standardize Only Numerical Features
* Interpreting the Important Predictors
* Simplifying the Model (Backward Elimination)
* Testing the Machine Learning Model
* Saving theLogistic Regression Model
* Creating a Module for Later Use of the Model

First, I transformed the categorical variables into dummy variables. I also split the data into train and tests sets with a test size of 20%.   

I tried three different models and evaluated them using Mean Absolute Error. I chose MAE because it is relatively easy to interpret and outliers aren’t particularly bad in for this type of model.   

I tried linear reggression model models:
*	**Linear Regression** – Baseline for the model

## Model performance
The Random Forest model far outperformed the other approaches on the test and validation sets. 
*	**Linear Regression**:model learned to clasfy 73% observation correctly 

![alt text](https://github.com/muhammadasifm/Absenteeism_project/blob/main/image/Capture%20last.PNG "summary table")

## summary
![alt text](https://github.com/muhammadasifm/Absenteeism_project/blob/main/image/absense%20of%20reasons.jpg "varios reasons")
* reason 0= basline line model(no reason)
* person have poison poison 20 time likely to absent than person who have no reason
* Drop unwanted reasons using back war elimination(daily work load avg,distance to work, day of week... all are have less impact) and make simple model
* Transportation reason is standardized so get hight accuracy, optimization work is hight
* pet have negative coeffitiant, 24& lower than base model, less effective
* intercept grt accurate result, cant interpret anything
## Data vizualisation

* Moving Data from Python to SQL
* Tableau Analysis: Age vs Probability
* Tableau Analysis: Reasons vs Probability
* Tableau Analysis: Transportation Expense vs Probability

## visulaize the data using tableau
* Analyze
* visualize
* interpret
 
![alt text](https://github.com/muhammadasifm/Absenteeism_project/blob/main/image/tablue%20analysis.PNG "Tableau observation")
![alt text](https://github.com/muhammadasifm/Absenteeism_project/blob/main/image/tablue%20analysis%202.PNG "Tableau observation")
