# Basic-Machine-Learning-with-Python
### Machine Learning Tutorial:
   1. [Machine Learning Tutorial (Bangla) | Bangla Machine Learning (ML) Tutorial for Beginners(study mart)](https://www.youtube.com/playlist?list=PLKdU0fuY4OFfWY36nDJDlI26jXwInSm8f)
   2. Course Outline: ([Machine Learning For All With Python.pdf](https://github.com/hamidhosen42/Basic-Machine-Learning-Algorithm-with-Python/files/7080875/Machine.Learning.For.All.With.Python.pdf)

## [Difference Between Supervised and Unsupervised Learning](https://medium.com/@hamid42/difference-between-supervised-and-unsupervised-learning-f51643aeb647):
   ### Supervised Learning:
   <img width="887" alt="Supervised Learning" src="https://user-images.githubusercontent.com/68488154/131554881-51ee1661-4625-4983-9798-fd4be5f919a9.png">

   In Supervised learning, you train the machine using data that is well “labeled.” It means some data is already tagged with the correct answer. It can be compared to learning which takes place in the presence of a supervisor or a teacher.
     
   A supervised learning algorithm learns from labeled training data, helps you to predict outcomes for unforeseen data. Successfully building, scaling, and deploying accurate supervised machine learning Data science models takes time and technical expertise from a team of highly skilled data scientists. Moreover, Data scientist must rebuild models to make sure the insights given remains true until its data changes.
    
   ### Unsupervised Learning:
   <img width="739" alt="Unsupervised Learning" src="https://user-images.githubusercontent.com/68488154/131554911-987a80a2-76d8-4ae0-a58d-c27f296ec918.png">

   Unsupervised learning is a machine learning technique, where you do not need to supervise the model. Instead, you need to allow the model to work on its own to discover information. It mainly deals with the unlabelled data. Unsupervised learning algorithms allow you to perform more complex processing tasks compared to supervised learning. Although, unsupervised learning can be more unpredictable compared with other natural learning deep learning and reinforcement learning methods.
   
   ### Supervised and Unsupervised Learning Algorithm:
   <img width="771" alt="Supervised and Unsupervised Learning Algorithm" src="https://user-images.githubusercontent.com/68488154/131554785-d0055847-4788-4357-8745-0a89152f08b2.png">

## Performance Metrics:
  <img width="417" alt="Performance Metrics" src="https://user-images.githubusercontent.com/68488154/132079458-2ec5d7b4-d131-4e08-9190-d25d70dfa625.png">

## R-Squared Value:
   R-squared is a goodness-of-fit measure for linear regression models. This statistic indicates the percentage of the variance in the dependent variable that the independent variables explain collectively. R-squared measures the strength of the relationship between your model and the dependent variable on a convenient 0 – 100% scale. Image of a large R-squared. After fitting a linear regression model, you need to determine how well the model fits the data. Does it do a good job of explaining changes in the dependent variable? There are several key goodness-of-fit statistics for regression analysis.
   
  <img width="632" alt="R-Squared Value" src="https://user-images.githubusercontent.com/68488154/132080071-c47681a6-eae1-4793-9d00-aeabe6e5330f.png">
  
## Feature Engineering in ML:
   
   ### Encoding Technique Types:
   #### 1. Without Use any encoding:
   #### 2. lavel encoding:
  <img width="616" alt="8-Level Encoding" src="https://user-images.githubusercontent.com/68488154/133471493-8d0024d3-915e-49c0-acb4-812cc589d516.png">
  <img width="639" alt="9-Level Encoding1" src="https://user-images.githubusercontent.com/68488154/133471538-2a2b5e58-a7fc-4b6a-adbd-96e308ac5a3c.png">
  
   #### 3. One Hot Encoding:
   <img width="601" alt="10-One-Hot Encoding" src="https://user-images.githubusercontent.com/68488154/133471900-e76017bb-b963-4fa0-acca-17e1c0783f3c.png">
   
   #### 4. Ordinal Encoding:
   <img width="628" alt="11-Ordinal Encoding" src="https://user-images.githubusercontent.com/68488154/133471958-73a26580-f85c-4627-a89c-3a6c2146d312.png">
   
   #### 5. Hash Encoding:
   <img width="648" alt="12-Hashing Encoding" src="https://user-images.githubusercontent.com/68488154/133471981-03a210ee-3f76-45cd-b5f0-b4cbd26bf2e5.png">

## ID3 Algorithm in Decision Tree :
   ID3 algorithm stands for Iterative Dichotomiser 3, which is a classification algorithm that follows a greedy approach of building a decision tree by selecting the best attribute that yields maximum Information Gain (IG) or minimum Entropy (H).

We will go through the basics of the decision tree, ID3 algorithm before applying it to our data. We will answer the following questions:

1. What is a decision tree?
2. What is the ID3 algorithm?
3. What is information gain and entropy?
4. What are the steps in the ID3 algorithm?
5. Using ID3 algorithm on a real data
6. What are the characteristics of the ID3 algorithm?

What is a Decision Tree?
A Supervised Machine Learning Algorithm, used to build classification and regression models in the form of a tree structure.

A decision tree is a tree where each -

Node - a feature(attribute)
Branch - a decision(rule)
Leaf - an outcome(categorical or continuous)
There are many algorithms to build decision trees, here we are going to discuss the ID3 algorithm with an example.

What is an ID3 Algorithm?
ID3 stands for Iterative Dichotomiser 3

It is a classification algorithm that follows a greedy approach by selecting the best attribute that yields maximum Information Gain(IG) or minimum Entropy(H).

What are Entropy and Information gain?
Entropy is a measure of the amount of uncertainty in the dataset S. Mathematical Representation of Entropy is shown here -

H ( S ) = ∑ c ∈ C − p ( c ) l o g 2 p ( c )
Where,

S - The current dataset for which entropy is being calculated(changes every iteration of the ID3 algorithm).
C - Set of classes in S {example - C ={yes, no}}
p(c) - The proportion of the number of elements in class c to the number of elements in set S.
In ID3, entropy is calculated for each remaining attribute. The attribute with the smallest entropy is used to split the set S on that particular iteration.
Entropy = 0 implies it is of pure class, which means all are of the same category.

Information Gain IG(A) tells us how much uncertainty in S was reduced after splitting set S on attribute A. Mathematical representation of Information gain is shown here -

I G ( A , S ) = H ( S ) − ∑ t ∈ T p ( t ) H ( t )
Where,

H(S) - Entropy of set S.
T - The subsets created from splitting set S by attributing A such that
S = ⋃ t ϵ T t
p(t) - The proportion of the number of elements int to the number of elements in set S.
H(t) - Entropy of subset t.
In ID3, information gain can be calculated (instead of entropy) for each remaining attribute. The attribute with the largest information gain is used to split the set S on that particular iteration.

What are the steps in the ID3 algorithm?

Calculate entropy for the dataset.
For each attribute/feature.
Calculate entropy for all its categorical values.
Calculate information gain for the feature.
Find the feature with maximum information gain.
Repeat it until we get the desired tree.

## [All About Confusion Matrix.pdf](https://github.com/hamidhosen42/Basic-Machine-Learning-with-Python/files/7272695/All.About.Confusion.Matrix.pdf)

## Types of Regression
   1. Linear Regression
   2. Polynomial Regression
   3. Logistic Regression
   4. Quantile Regression
   5. Ridge Regression
   6. Lasso Regression
   7. Elastic Net Regression
   8. Principal Components Regression (PCR)
   9. Partial Least Squares (PLS) Regression
   10. Support Vector Regression
   11. Ordinal Regression
   12. Poisson Regression
   13. Negative Binomial Regression
   14. Quasi Poisson Regression
   15. Cox Regression
   16. Tobit Regression

## Ensemble Learning

Ensemble methods is a machine learning technique that combines several base models in order to produce one optimal predictive model . To better understand this definition lets take a step back into ultimate goal of machine learning and model building.

## [Random Forest Classifier & Regressor](https://www.youtube.com/watch?v=4EOCQJgqAOY)
![image](https://user-images.githubusercontent.com/68488154/136642823-85231cce-6661-442d-a1a5-dd6165a73748.png)

link:[Random Forest](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html)

The random forest is a classification algorithm consisting of many decisions trees. It uses bagging and feature randomness when building each individual tree to try to create an uncorrelated forest of trees whose prediction by committee is more accurate than that of any individual tree.

Random forests or random decision forests are an ensemble learning method for classification, regression and other tasks that operates by constructing a multitude of decision trees at training time. ... For regression tasks, the mean or average prediction of the individual trees is returned.

Random Forest Regression is a supervised learning algorithm that uses ensemble learning method for regression. ... A Random Forest operates by constructing several decision trees during training time and outputting the mean of the classes as the prediction of all the trees


## Feature Selection Techniques in Machine Learning with Python
Feature Selection is one of the core concepts in machine learning which hugely impacts the performance of your model. The data features that you use to train your machine learning models have a huge influence on the performance you can achieve. How to select features and what are the Benefits of performing feature selection before modeling your data?
   1. Reduces Overfitting: Less redundant data means less opportunity to make decisions based on noise.
   2. Improves Accuracy: Less misleading data means modeling accuracy improves.
   3· Reduces Training Time: fewer data points reduce algorithm complexity and algorithms train faster.

## Feature Selection Methods:
   1. Univariate Selection
   2. Feature Importance ( https://youtu.be/VXv0-Hv9cT4 )
   3. Correlation Matrix with Heatmap
## Feature Selection Related Important Links:
   1. https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.chi2.html#sklearn.feature_selection.chi2
   2. https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.f_classif.html#sklearn.feature_selection.f_classif
   3. https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.mutual_info_classif.html#sklearn.feature_selection.mutual_info_classif
   4. https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.f_regression.html#sklearn.feature_selection.f_regression
## k-nearest neighbors (KNN)
The k-nearest neighbors (KNN) algorithm is a simple, supervised machine learning algorithm that can be used to solve both classification and regression problems. It's easy to implement and understand, but has a major drawback of becoming significantly slows as the size of that data in use grows.
   1. https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsRegressor.html
   2. https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html
   3. <img width="470" alt="2-" src="https://user-images.githubusercontent.com/68488154/140653966-7b3dc395-e67d-47e8-ac44-f2b899a49fac.png">
   4. <img width="569" alt="3-" src="https://user-images.githubusercontent.com/68488154/140654023-8ba459a1-493b-43ab-b236-0aa3e6d24cfc.png">

