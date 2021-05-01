# Breast-Cancer-Prediction
## Data Source
Breast Cancer Wisconsin (Diagnostic)\
Data Set Link https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)


## Objective
Generate a classification model (Logistics Regression, K-Nearest Neighbor, and Support Vector Machine) and determine which model is the best for the problem. Make sure to perform the necessary data cleaning steps (scaling, splitting, correlation, etc.) before generating the model. 

## Method
  - Analyze columns (remove not needed columns)
  - Level the response variable (the count of 'yes' should match the count of 'no')
  - Split the dataset into train and test datasets. Use 70% on the train dataset and 30% to the test dataset
  - Inspect the variables range, mean, and standard deviation to determine whether scaling is needed
  - Generate Logistic Regression, make predictions, and assess model's accuracy
  - Generate K-Nearest Neighbors, make predictions, and assess model's accuracy
  - Generate Support Vector Machine, make predictions, and assess model's accuracy
  
## Analysis
  - There are 2 columns in the dataframe that are needed - id and unnamed:32. They are removed on the dataframe
  - There are 212 counts of benign which is labeled as 0 and 
  - There is a variance between the values of the response. There are 212 counts of benign/0 and 357 counts of malignant/1
  - Performed down scaling to match the counts of the responses
  - There is a significant difference between the variables mean, range and standard deviation. Performed data set scaling
  - Logisitcs Regression has an accuracy of 96%
    - True Positive - 62
    - True Negative - 61
    - False Positive - 2
    - False Negative - 3
  - K-Nearest Neighbors has an accuracy of 
    - True Positive - 62
    - True Negative - 60
    - False Positive - 3
    - False Negative - 3
  - Support Vector Machine has an accuracy of 
    - True Positive - 62
    - True Negative - 60
    - False Positive - 3
    - False Negative - 3

## Conclusion
There are 3 models generated on the analysis. The best model is Logistic Regression which has 96% accuracy. 
