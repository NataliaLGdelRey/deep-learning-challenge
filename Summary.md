## Alphabet-Soup-Machine-Learning
------------------------------------


## Overview
--------------------
The aim of this project is to create a machine learning-based binary classifier tool for Alphabet Soup, a nonprofit foundation, to assist them in selecting the applicants for funding with the highest potential for success in their ventures. The dataset used for this analysis contains various measures on 34,000 organizations that have been funded by Alphabet Soup. The project includes three steps:

- Preprocessing the data for the neural network
- Compile, Train and Evaluate the Model
- Optimizing the model

## Results
--------------------

- Data Preprocessing
-----------------------

The 'EIN' and 'NAME' columns were dropped as they do not provide any useful information for the model.
The target variable was set as 'IS_SUCCESSFUL'.
Additional columns that could be noisy were dropped to optimize the model.
Compiling, Training, and Evaluating the Model:
The number of input features was set as the length of X_train[0].
The deep learning model was designed with 2 hidden layers consisting of 50 and 20 neurons, respectively, and one output layer.
The activation function used in the hidden layers is ReLU, which is ideal for looking at positive non-linear input data for classification or regression.
The activation function used in the output layer is sigmoid, which is ideal for binary classification.

- Summary
-------------------

Despite the various changes made in the model the model was unable to reach the target accuracy of 75%. The deep learning model that was implemented resulted in a loss of 0.5659 - and accuracy of 0.7251 (72%). The goal was to predict whether an applicant will be successful if funded by the organization or not. During our experiments, we rarely observed the training accuracy surpassing 73%, which is when the network has access to the answers. Thus, we are confident that obtaining a real-world result of 75% accuracy on test data using this method is not feasible.

## Recommendation
-------------------

The recommendation is to use a Random Forest Classifier algorithm for this classification problem. A random forest classifier is an ensemble learning method that operates by constructing a multitude of decision trees at training time and outputting the class that is the mode of the classes (classification) or mean prediction (regression) of the individual trees. By using Random Forest, the model can handle the imbalance in the dataset and predict with high accuracy. Moreover, it can provide feature importance that can help to identify which feature is essential in predicting whether the applicant will be successful or not.