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
# Decision Trees

1. Purpose:

Decision Trees are versatile algorithms that can be used for both regression and classification tasks.

2. How It Works:

. The model creates a tree-like structure where each node represents a feature, each branch represents a decision, and each leaf node represents an outcome (class label or continuous value).
. The tree splits the dataset into subsets based on feature values to maximize homogeneity (for classification) or minimize variance (for regression).

3. Key Concepts:

. Splitting: Partitioning the dataset based on feature values.
. Impurity: Measures the "mixing" of classes in a subset. Common measures include:
 . Gini Index: Used for classification.
 . Entropy (Information Gain): Used for classification.
 . Mean Squared Error (MSE): Used for regression.
. Pruning: Reducing the size of the tree to prevent overfitting.

4. Advantages:

. Easy to interpret and visualize.
. Handles both numerical and categorical data.
. Non-linear decision boundaries.

5. Disadvantages:

. Prone to overfitting if the tree grows too deep.
. Sensitive to small variations in the data.

Example Use Case:
Classification: Predict whether a customer will buy a product based on features like income, age, and browsing behavior.
Regression: Predict house prices based on features like size, location, and number of rooms.

# Random Forest

1. What It Is:

. Random Forest is an ensemble learning method that builds multiple decision trees and combines their predictions (by majority vote for classification or averaging for regression) to improve performance and reduce overfitting.

2. Why Learn It After Decision Trees?

. It builds upon Decision Trees and introduces the concept of ensemble learning, teaching you how combining multiple models can improve accuracy and generalization.

### Key Advantages:

More robust and less prone to overfitting compared to individual Decision Trees.
Handles missing data and is less sensitive to outliers.
 
