# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Mohamed Elwakel

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
At the beginning the model had many errors one of them was the negatiive values which prevented us from submitting it to kaggle so we needed to replace them with zeros

### What was the top ranked model that performed?
KNeighborsDist Model

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
First I changed the weather and the season to categorical features and added new features by getting the month, day, and hour from date time

### How much better did your model preform after adding additional features and why do you think that is?
TODO: Add your explanation

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
TODO: Add your explanation

### If you were given more time with this dataset, where do you think you would spend more time?
TODO: Add your explanation

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|default_vals|default_vals|default_vals|1.795|
|add_features|default_vals|default_vals|default_vals|0.688|
|hpo|GBM: num_leaves: lower=26, upper=66|NN: dropout_prob: 0.0, 0.5|GBM: num_boost_round: 100|0.678|

### Create a line plot showing the top model score for the three (or more) training runs during the project.


![model_train_score.png](img/model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.


![model_test_score.png](img/model_test_score.png)

## Summary
I was able to use a new framework at the end called AutoGluon to solve a machine learning model using linear regression and automate it successfully which gave me a good experience and some fun.  