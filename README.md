# Empowering Academic Excellence By Analyzing Student Performance Across Disciplines: Project Overview
* Support informed decision-making: Analyzing student performance data helps educators, administrators, and policymakers make informed decisions about curriculum development, resource allocation, and intervention strategies. Identifying the percentage of students meeting specific performance goals (such as an 80% goal) can be vital in targeting areas that need improvement or additional support.
* Identify trends and patterns: By examining summary statistics across multiple disciplines, I uncover patterns or trends in student performance. This information can be used to inform best practices, design targeted interventions, or guide future research on educational methods and strategies.
* Measure effectiveness of programs: This project serves as a benchmark for measuring the effectiveness of various educational programs, curricula, or teaching methods. By comparing the percentage of students meeting the 80% goal before and after implementing changes, stakeholders can assess the impact of their initiatives on student performance.


## Problem Description:
* Utilizing school data, perform a comprehensive analysis of summary statistics across six key disciplines (Math, Physics, Biology, Chemistry, Spanish, and Literature) to determine the percentage of students achieving an 80% or higher goal. 
* Each course has a distinct grading structure with assignments accounting for 20%, midterms contributing 30%, and finals representing 50% of the final grade. 
* Additionally, each discipline holds a specific credit weight (Math - 4, Physics - 4, Biology - 3, Chemistry - 2, Spanish - 2, Literature - 3), summing up to a total of 18 credits.






 ![Report Image](report_image.png)

## Data and packages
* Data: https://www.kaggle.com/datasets/austinreese/usa-housing-listings
* Packages: Pandas, Numpy, Matplotlib, Seaborn, Pickle

## Initial Features
       * 'id', 'url', 'region', 'region_url', 'price', 'type', 'sqfeet', 'beds',
       * 'baths', 'cats_allowed', 'dogs_allowed', 'smoking_allowed',
       * 'wheelchair_access', 'electric_vehicle_charge', 'comes_furnished',
       * 'laundry_options', 'parking_options', 'image_url', 'description', 'lat',
       * 'long', 'state'
       
 ## Data Cleaning
 * Check for missing values
 * Check for the data types
 * Drop features that don't impact the target variable
 * Dimensionality reduction
 * Outliers removal
 

## Feature understanding
### I looked at the distributions of the data for various features.

  ![Sqfeet Distribution](sqfeet_distribution.png)

  
  
## Feature relationship
# Power Bi
### Table data
* Table 1: https://www.kaggle.com/datasets/austinreese/usa-housing-listings
* Table 2: https://en.wikipedia.org/wiki/List_of_states_and_territories_of_the_United_
### Visualization
* Used the Power Query Editor to transform, analyze, and clean the data
* Used Model View to join two tables
* Used Report View to plot charts, tables, and maps and to implement filters, slicers, and drill-throughs 
  
 
 # Model Building
 ### Label Encoding with OneHotEncoding
 ### Split the data between features and target variable 'Price'
 ### Tuned hyperparameters and evaluated model performance using the R-squared as a metric:
 
 
 # Model performance: the Decision Tree regressor model outperformed the linear regression model models on the test and validation sets
 ### Linear Regression:  R^2 = 74%
 ### Decision Tree Regressor: R^2 = 82%
 
 
 # Saved the model with Pickle for future use
