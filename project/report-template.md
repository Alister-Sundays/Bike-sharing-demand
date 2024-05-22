# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### ALISTER WABUTI SUNDAYS

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
TODO: Add your explanation

### What was the top ranked model that performed? WeightedEnsemble_L3
The fact that WeightedEnsemble_L3 was the top-ranked model indicates that it outperformed other individual models and ensemble configurations in terms of predictive performance, possibly achieving a better balance between bias and variance, capturing complex patterns in the data, and generalizing well to unseen data.

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
• Season: We see highest number bike rentals in Summer Seasons and the lowest in Spring season.

• Weather: As one would expect, we see highest number of bike rentals on a clear day and the lowest on a snowy or rainy day.

• Humidity: With increasing humidity, we see decrease in the number of bike rental count.

High demand of bike at 8AM as the time of people for going to their work and 6PM time of returning to home.

Prefer more bikes in the morning

For additional features i extracted the hour from the datetime field and added it as a column on the train and test dataframe

### How much better did your model preform after adding additional features and why do you think that is?
Performace improvedthis is because the hour feature is quite important in the prediction . it carries more weight compared to other features
## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
It varied but the best performnce was realized when i optimzed the model with a hyperparameter

### If you were given more time with this dataset, where do you think you would spend more time?
EDA - To have a good understanding of the various features characteristics , correlations and importance 
Feature engineering - to reduce bias and variance on the model. perhaps do some normalization and encoding 

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
[Download model_scores.csv](model_scores.csv)

### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![model_train_score.png](img/model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png](img/model_test_score.png)

## Summary
TODO: Add your explanation
