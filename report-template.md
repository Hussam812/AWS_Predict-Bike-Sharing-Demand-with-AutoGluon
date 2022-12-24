# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### NAME HERE

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
TODO: Add your explanation
my prediction dosn't have any negative values

### What was the top ranked model that performed?
TODO: Add your explanation
my scend one was best with score value 1.80092

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
TODO: Add your explanation
* datatime column was odject data type i coverted it to datetime and split it to day, month, year
* season and weather were int dtype and i have converted them to category with as type data

### How much better did your model preform after adding additional features and why do you think that is?
TODO: Add your explanation
The model performance greatly improved from a score of 1.79343 prior to feature engineering to 1.80092 after

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
TODO: Add your explanation
i have used this {hyperparameters="multimodal",hyperparameter_tune_kwargs="bayesopt"},  and it didn't help it give my score 1.32535 
### If you were given more time with this dataset, where do you think you would spend more time?
TODO: Add your explanation
I would spend more time working on some_fature engineering and other hyperparaneter and i creating more features to fit into the training data.
### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|600|default|default|1.79343|
|add_features|800|default|default|1.80092|
|hpo|1000|multimodal|bayespot|1.32535|

### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![model_train_score.png](img/model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png](img/model_test_score.png)

## Summary
TODO: Add your explanation
I have fun with working with AutoGluon:

i need to enhance my models with adding othors features and need to knew why hyper prameter dosn't enhance my score