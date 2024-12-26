# machine_learning_exam

1. [Objective] Write a Python program using numpy to perform specific image processing tasks
on a color image. The tasks include converting a color image to grayscale and performing
image flipping operations.

(1) Horizontal Flip Function: Write a function flip_horizontal that takes a numpy array of the
grayscale image and returns a horizontally flipped version.

(2) Vertical Flip Function: Write a function flip_vertical that takes the same numpy array and
returns a vertically flipped version.

2. Given a set of noisy data points generated from a polynomial function, your task is to write a
Python program that estimates the optimal degree of the polynomial that best fits the data.
You do not know the original polynomial degree used to generate the data.

[Tasks]
(1) Read the test2.csv file and split the data into a training set and a testing set.

(2) Implement a loop that tries polynomial models of different degrees (from 1 to 10).

(3) For each model, use polynomial features with a LinearRegression model to fit the training
data.

(4) Evaluate each model using the mean squared error (MSE) on the testing data.

(5) Identify the degree of the polynomial that gives the lowest MSE.
[Hints]
- Use PolynomialFeatures from sklearn.preprocessing to generate polynomial and interaction
features.
- Use mean_squared_error from sklearn.metrics to evaluate your models.
[Expected Output]
- Plot or print the MSE for each polynomial degree.
- Conclude which degree is optimal based on the lowest MSE.


3. The Wine dataset comprises 13 features related to the chemical composition of wine and a
target variable indicating the wine cultivar. This dataset is excellent for practicing classification
techniques in machine learning. Implement a k-Nearest Neighbors (k-NN) classifier to
identify the cultivar of a wine based on its chemical attributes. Determine the optimal
number of neighbors for the best classification performance.
[Tasks]
(1) Data Preparation:
⚫ Load the Wine dataset from the sklearn.datasets module.
⚫ Split the dataset into training and testing sets.
(2) k-NN Classifier Implementation:
⚫ Implement the k-NN classifier using scikit-learn.
⚫ Normalize the feature data since k-NN is sensitive to the magnitude of data points.
(3) Model Evaluation:
⚫ Evaluate the classifier performance using accuracy as the metric.
⚫ Experiment with different values of k (from 1 to 20) to find the optimal number of
neighbors.
⚫ Plot the relationship between k and testing accuracy.
(4) Discussion:
⚫ Discuss the effect of k on the classification performance.


4. The Wholesale Customers dataset contains data about customers of a wholesale distributor. It
includes various product spending categories such as Fresh, Milk, Grocery, Frozen,
Detergents_Paper, and Delicatessen. The dataset includes "Channel" and "Region" categories for
customers; however, please disregard these for the purposes of this assignment. This data is
suitable for understanding customer purchase behavior and segmenting customers based on
spending patterns using clustering techniques. You are tasked with analyzing the Wholesale
Customers dataset to identify distinct groups (clusters) of customers based on their annual
spending on different product categories. Use k-means clustering to achieve this
segmentation.
(data is available at https://archive.ics.uci.edu/dataset/292/wholesale+customers)

[Tasks]
(1) Data Preparation:
⚫ Load the Wholesale Customers dataset.
⚫ Conduct any necessary data preprocessing steps like normalization, handling missing
values, or removing irrelevant features.

(2) Exploratory Data Analysis:
⚫ Perform exploratory data analysis to understand the distribution of the key variables
and the relationship between different features.

(3) Clustering Implementation:
⚫ Implement k-means clustering to segment the wholesale customers.
⚫ Determine the optimal number of clusters using the Elbow Method
(Please refer https://www.analyticsvidhya.com/blog/2021/01/in-depth-intuition-of-k-
means-clustering-algorithm-in-machine-learning/.)

(4) Cluster Analysis:
⚫ For each cluster, calculate the mean spending in each product category (Fresh, Milk,
Grocery, etc.).
⚫ Compare these means across clusters to identify what distinguishes each cluster from
the others. For example, one cluster might have high spending in "Fresh" and low in
"Detergents_Paper," while another might show the opposite pattern.

(5) Reporting Results: Summarize the characteristics of each cluster


