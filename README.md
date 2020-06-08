
# Prediciton of Heart Disease using Cleveland Dataset

The objective of this project is to use techniques taught in class to study the data patterns or to predict heart disease for the Cleveland dataset. Refer to the Appendix for the reference and description of the data set.

# Dataset

The dataset can be found in the following link:
https://archive.ics.uci.edu/ml/machine-learning-databases/heart-disease/processed.cleveland.data

# Process

* Data Exploration: Conducting a deep exploratory analysis for the data
* Hypothesis Creation: : From the data exploration phase, what relationships are you planning to further clarify with modeling?
* Methodologies: The alogrithms being used to test the hypothesis
* COnclusions: The final findings from the analysis

# Data Exploration

Number of people with the heart disease: 137
Number of people without  the heart disease: 159
Number of Men in the dataset who have the disease: 112/200
Number of women in the dataset who have the disease: 25/96

More detailed exploration data is present in the Project_Report.pdf file

# Hypothesis:

* Different nums are affected by different parameters. Cholesterol, Age, Sex and Chest pain affect the NUM the most significantly.
* Older men, with High Cholesterol and High BP are more prone to heart disease.
* Trestbps and thalach can indicate if a patient has exang

# Methodologies
> * Hypothesis 1:
> Split “num” into 4 variables based on the level of severity of the heart disease: num1 - num4;
> Split data on training (70%) and testing (30%);
> Run Lasso on training data for each num to define min lambda;
> Run logistic regression on training data to identify the most significant factors and their coefficients;
> Assess the prediction accuracy using test data for predictions.

> * Hypothesis 2:

> Assign values of 0 & 1 on num
> Perform LASSO to determine the best subset of the dataset with response variable as num.
> Perform scaling on the predictors determined from LASSO
> Using Hierarchical  clustering with complete method on the dataset with predictors selected above

> * Hypothesis 3:
> Fit a logistic regression on trestbps and thalach regarding exang to test if the two predictors are of statistical significance.
> Drop the predictor that’s not significant until the predictors are all significant

# Results:

* Different factors influence heart disease prediction differently based on disease severity;
* Surprisingly as it can be seen from the table, neither age nor sex nor cholesterol turned out to be significant factors in prediction of all heart diseases’ severity levels;
* There is a significant increase in number of heart diseases cases when the age of person increases from 44 to 57 and also probability of heart disease can be more for men.
* The Cholesterol  levels in the cluster with more heart diseases are significantly more apart
* The Blood Pressure levels in both the clusters are appearing to be closer than expected
* Resting blood pressure(trestbps) is not an indicator of exang as tested in the logistic regression
* Maximum heart rate achieved (thalach) is a crucial indicator of exang.


# Credit:
The project was completed along with Achal Suresh, Sergey Postolosky, Yaosong Yu, Nida Kazi

