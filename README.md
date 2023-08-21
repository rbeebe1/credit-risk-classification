# Module 12 Report Template

## Overview of the Analysis
This analysis uses data from a peer-to-peer lending company to build a model that can identify the creditworthiness of its borrowers. 
* Each row within the dataset contains metadata per borrower, including information regarding their loan size, income, number of accounts, total debt, and has even been pre-labeled as healthy or high-risk for the sake of modeling. 
* Within the data, there are 75036 healthy loans labeled, and 2500 high-risk loans labeled.
* The stages of the machine learning process were:
  * Split the dataset into X and y, with X containing all the borrowers' data and y containing their healthy or high-risk labels.
  * Separate the labels and data into training and testing sets
  * Fit the training data to a Logistic Regression model.
  * Predict the labels for the testing data
  * Evaluate the model's performance using the accuracy score, confusion matrix, and classification report.
  * Repeat using oversampled data. 

## Results
* Machine Learning Model 1:
  * <img width="460" alt="image" src="https://github.com/rbeebe1/credit-risk-classification/assets/126029780/49549cba-79da-44e4-8f55-df62264c1772">

* Machine Learning Model 2:
  * <img width="455" alt="image" src="https://github.com/rbeebe1/credit-risk-classification/assets/126029780/695642f9-c30d-4d3e-be40-1ff8004d1e75">


## Summary
* **Machine Learning Model 2** utilizing the random oversampling seems to perform slightly better than Machine Learning Model 1 as we saw the second model has a slightly higher macro average accuracy and recall scores.
* It should be noted though, that the data was heavily skewed toward healthy loans and had a substantial number of them in the data compared to high-risk loans, resulting in the poor performance by the model. Of the two models, I would recommend the second, however, I would strongly suggest that any companies who wish to utilize this model to predict high-risk borrowers first train the model further on high-risk loan data. 
