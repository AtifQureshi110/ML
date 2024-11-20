# ML Algorithms.
All Models of ML
# Linear Regression
Linear Regression works on continuous data, aiming to find a relationship between independent (predictor) and dependent (target) variables by modeling their relationship with a linear equation. Its goal is to minimize the errors and fit a line (or hyperplane) that best represents the data.

1. Purpose:
   
Linear Regression is used to model the relationship between an independent variable (or variables) and a dependent variable.
It predicts continuous values based on this relationship.

2. How It Works:

It attempts to find the best-fitting straight line (in the case of simple linear regression) or a hyperplane (in the case of multiple linear regression) that minimizes the error between the predicted and actual values.
The relationship is expressed as a linear equation:
𝑦 = 𝛽0 + 𝛽1𝑥 + 𝜖
y: Dependent variable (target).
x: Independent variable (predictor).
𝛽0: Intercept.
β1: Slope of the line.
ϵ: Error term (residual).

3. Bringing Points Near the Line:

Linear Regression uses the least squares method to minimize the sum of the squared differences (errors) between the observed and predicted values. This process ensures that the predicted line is as close to the actual data points as possible.

# Logistic Regression

Logistic Regression is applied to datasets with a categorical target variable and is typically used for classification tasks, such as distinguishing between 0 and 1. The classification is achieved with the help of the sigmoid function, which maps inputs to probabilities and allows the model to predict class labels.

1. Purpose:

Logistic Regression is primarily used for classification problems where the target variable is categorical (e.g., binary classification like 0 and 1 or multi-class classification like A, B, and C).

2. How It Works:

It predicts the probability of a data point belonging to a particular class using the sigmoid function.
The sigmoid function maps any real-valued number to a value between 0 and 1, enabling it to model probabilities.
The sigmoid function:
σ(z)= 1/1+e−z


z is the linear combination of input features and weights: 
𝑧 = 𝛽0 +𝛽1x1 + ... +𝛽nxn

3. Classification:

For binary classification, logistic regression predicts probabilities and assigns a class based on a threshold (commonly 0.5):

​Predicted class={ 1, if σ(z)≥0.5 or 0 if σ(z)<0.5}

4. Datasets:

Logistic Regression can work with both numerical and categorical features, but the target column must be categorical. Features are often preprocessed (e.g., one-hot encoding for categorical features).
​





 
