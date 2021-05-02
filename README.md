# Breast-Cancer-Prediction
## Data Source ##
The dataset used in this analysis is the 'Breast Cancer Wisconsin Dataset' which can be found at the [University of California Irvine Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)).

**Variables Description:**
 * ID number
 * Diagnosis (M = malignant, B = benign)
 * Ten real-valued features are computed for each cell nucleus:
     * radius (mean of distances from center to points on the perimeter)
     * texture (standard deviation of gray-scale values)
     * perimeter
     * Area
     * Smoothness (local variation in radius lengths)
     * Compactness (perimeter^2 / area - 1.0)
     * Concavity (severity of concave portions of the contour)
     * Concave points (number of concave portions of the contour)
     * Symmetry
     * Fractal dimension ("coastline approximation" - 1)

## Objective
Generate classification models such as Logistic Regression, Support Vector Machine, and K-Nearest Neighbors to classify whether the patient has a Malignant or Benign Tumor. 

## Method
  - Analyze columns (remove not needed columns).
  - Level the response variable (the count of 'yes' should match the count of 'no').
  - Split the dataset into train and test datasets. Use 70% on the train dataset and 30% to the test dataset.
  - Inspect the variables range, mean, and standard deviation to determine whether scaling is needed.
  - Generate Logistic Regression, make predictions, and assess model's accuracy.
  - Generate K-Nearest Neighbors, make predictions, and assess model's accuracy.
  - Generate Support Vector Machine, make predictions, and assess model's accuracy.
  
## Analysis
  - There are 2 columns in the dataframe that are needed - id and unnamed:32. They are removed on the dataframe.
  - There is a variance between the values of the response. There are 212 counts of benign/0 and 357 counts of malignant/1
  - Performed down scaling to match the counts of the responses.
  - There is a significant difference between the variables mean, range and standard deviation. Performed data set scaling.
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
