# Supervised_Learning

In Supervised Learning, the model learns from past examples to predict future values.

Supervised learning is a type of machine learning where the values to be predicted are already known, 
and a model is built with the aim of accurately predicting values of previously unseen data. 
Supervised learning uses features to predict the value of a target variable, such as predicting a basketball player's position based on their points per game. 

There are two types of supervised learning. 

**Classification**
Classification is used to predict the label, or category, of an observation. 
For example, we can predict whether a bank transaction is fraudulent or not. 
As there are two outcomes here - a fraudulent transaction, or non-fraudulent transaction, this is known as binary classification. 

**Regression**
Regression is used to predict continuous values. 
For example, a model can use features such as number of bedrooms, and the size of a property, to predict the target variable, price of the property.

**Classification** 

Classifying labels of unseen data:
we build a classifier, 
Classifier learns from the labeled data we pass to it,
We then pass it unlabeled data as input, and 
it predict labels for this unseen data. 

As the classifier learns from the labeled data, we call this the training data.

**K- Nearest Neighbors (KNN) classifier:**

The idea of k-Nearest Neighbors, or KNN, is to predict the label of any data point by looking at the k closest labeled data points and getting them to vote on what label the unlabeled observation should have. KNN uses majority voting, which makes predictions based on what label the majority of nearest neighbors have.

## .values() --> is used to convert the data into numpy arrays 

Measuring model performance:

**Accuracy**  is the number of correct predictions divided by the total number of observations.

Train test split: 

x_train , x_test, y_train, y_test = train_test_split( x, y, test_size = 0.3, random_state = 21, stratify = y)

The random_state argument sets a seed for a random number generator that splits the data. 

stratify = y : Using the same number when repeating this step allows us to reproduce the exact split and our downstream results. It is best practice to ensure our split reflects the proportion of labels in our data. So if churn occurs in 10% of observations, we want 10% of labels in our training and test sets to represent churn. We achieve this by setting stratify equal to y.



