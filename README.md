## Outlier Removal in Dataset

### Overview
This repository contains code for removing outliers from a dataset using various statistical methods. 
Outliers are data points that significantly differ from other observations in the dataset and can distort statistical analyses.
This code aims to identify and remove outliers to ensure more accurate analysis and modeling.

 Outlier removal techniques are used to identify and eliminate data points that deviate significantly from the rest of the data in a dataset. These outliers can skew statistical analyses and machine learning models, leading to inaccurate results. Here are some common techniques for outlier detection and removal:
###  1.Mean 
   
The mean function can be used to remove outliers by calculating the mean of the data and then removing data points that lie too far from the mean, indicating they are potential outliers. One common approach is to define a threshold, such as a certain number of standard deviations away from the mean, and remove any data points that fall outside of this threshold.

###  2.Percentile 

The percentile method is a technique used to treat outliers by identifying and capping extreme values based on a specified percentage threshold. It involves calculating the threshold values based on percentiles and replacing any data points that exceed these thresholds with the corresponding threshold values.

###  3.Inter Quartile Method (IQR)

IQR is used to measure variability by dividing a data set into quartiles. The data is sorted in ascending order and split into 4 equal parts. Q1, Q2, Q3 called first, second and third quartiles are the values which separate the 4 equal parts.

Q1 represents the 25th percentile of the data.
Q2 represents the 50th percentile of the data.
Q3 represents the 75th percentile of the data.

###  4.Normal Distribution Method

Even in a normal distribution, there can be outliers. Depending on their nature and the sensitivity of your model to outliers, you might want to address them. Common strategies include truncation, or using statistical methods to cap or adjust these values.

The following first three methods help us identify them, while the fourth one will both identify and address them (which should actually be considered within the data cleaning stage instead of within the EDA one).


### 5.Z-Score

Z score, also called as standard score, is used to scale the features in a dataset for machine learning model training.
It can also be used to detect outliers. In this one, we will first see how to compute Z-scores and then use it to detect outliers.




