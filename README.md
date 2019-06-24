# Titanic-Prediction

## Problem Statement
Predciting which passengers aboard the Titanic were most probable to survive the famous crash

## Data Wrangling and Feature Engineering
- Since this problem is a classificaiton problem, I decided to drop variables that would not contribute to the classification like Ticket and Cabin
- The titles were grouped into more holistic categories like Master, Miss etc to reduce entropy during classification
- The age was split into 5 range-based categories
- Created a new variable for family which included the sum of spouse, children and siblings
- Created a new binary variable for people who were aboard the ship alone, with no family
- Created a new variable by multiplying age and class 
- Empty values in the embarked variable were imputed with the mode
- All categorical variables were mapped to numeric categories (0,1,2...) so that they can be fit in the classification model
- Other missing values were imputed with either mean or mode

## The Model
I decided to fit the following classification models on the data:
- Support Vector Machines
- K-Nearest Neighbors
- Naive Bayes
- Decision Tree
- Random Forest

The Random Forest gave me the highest accuracy of 86%
