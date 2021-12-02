# Crop-Recommendation-Dataset
This case we use dataset taken from kaggle: Crop Recommendation Dataset, dataset can be found here. On dataset consist 22 type of crops growth in various condition and the end goal is to predict which crop could be planted (as labelled on Target Column) based on various condition that provided on features columns.

# Dataset Understanding
Dataset was used have 8 total columns where 7 columns are feature columns and 1 column is target variable. Description each columns will be explanation below :
- N : Ratio of Nitrogent content in soil
- P : Ratio of Phosporous content in soil
- K : Ratio of Potassium content in soil
- temperature : Temperature ambient in degree Celcius
- rainfall : Rainfall in mm
- humidity : Relative Humidity in %
- ph : pH value or acidity level in soil
- Label : Crop types

Based on Dataset, there are 2.200 data rows, have 6 numerical values and 1 categorical values. Then dataset have 0 missing values.

# Exploratory Data Analysis
As explained before there are numerical values and categorical value so we will explore data distribution each columns below.

## Numerical Distribution
![alt](https://github.com/Fachruds1/Crop-Recommendation-Dataset/blob/main/Numeric%20Distribution.jpg)
![alt](https://github.com/Fachruds1/Crop-Recommendation-Dataset/blob/main/numer%20distribution.jpg)

## Categorical Distribution
![alt](https://github.com/Fachruds1/Crop-Recommendation-Dataset/blob/main/categricl%20columns.jpg)

## Correlaton Features
N and K have highly correlation (0.74) but its not included in multicollinearity case because correlation < 0.8 so, we can use all features for modelling.

![alt](https://github.com/Fachruds1/Crop-Recommendation-Dataset/blob/main/corr%20analysis.png)

# Machine Learning Models
Our data has ready to do modelling so in this case we will do machine learning models using 3 models they are KNN Classification, Random Forest and Logistic Regression.

## KNN Classification
![alt](https://github.com/Fachruds1/Crop-Recommendation-Dataset/blob/main/knn%20test.png)
![alt](https://github.com/Fachruds1/Crop-Recommendation-Dataset/blob/main/knn%20rep.png)

## Random Forest
![alt](https://github.com/Fachruds1/Crop-Recommendation-Dataset/blob/main/rf%20test.png)
![alt](https://github.com/Fachruds1/Crop-Recommendation-Dataset/blob/main/rf%20rep.png)

## Logistic Regression
![alt](https://github.com/Fachruds1/Crop-Recommendation-Dataset/blob/main/lrg%20test.png)
![alt](https://github.com/Fachruds1/Crop-Recommendation-Dataset/blob/main/lrg%20rep.png)

# Summary
KNN Classification model obtain good and highest result but it’s not proper result because dataset was used included in survivorship bias. So, We must change dataset will be used by changing the data used with the data obtained with the right sampling technique. Or we can do in next project use this dataset by changing the target variable because we can see from the dataset that there are independent variables (rainfall, ph, temperature and humidity) and dependent variables (N, P, K) so that we can make the dependent variables as target variables.

