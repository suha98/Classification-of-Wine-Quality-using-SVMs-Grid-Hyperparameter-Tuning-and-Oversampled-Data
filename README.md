# Classification-of-Wine-Quality-using-SVMs-Grid-Hyperparameter-Tuning-and-Oversampled-Data

The wine quality dataset was collected from Kaggle: https://www.kaggle.com/yasserh/wine-quality-dataset 

About the dataset:

1.   The output variable is wine quality, rated on an integer scale of 0 (lowest) to 10 (highest)
2.   There are no missing values, that is, cells that are empty or had been filled with an irregular value like '-1' or 9999
3.   There are 11 columns of features and one output column that classifies the quality of the wine. One of the columns has the wine ID
4.   The dataset has a total of 1143 rows
5.   There is a major class imbalance in the data, with very few instances of the minority classes

After visualizing the data and using feature engineering techniques, I used Scikit Learn to implement an SVM in order to classify wine quality. I tuned the hypermarameters (C, gamma, and the kernel function) using the Grid Search algorithm; I also repeated the process on oversampled data (using SMOTE) to analyze the impact of class imbalance on performance.

The model was unable to classify even a single instance of the minority classes correctly before oversampling and had an overall accuracy of 66%. This increased to 86% on the oversampled data, with the majority of instances in all the classes being classified correctly.
