# Report: Predict Bike Sharing Demand with AutoGluon Solution

#### M Yuktha

## Initial Training

### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?

Managing my end sems and project submission deadline was hard. It took me alot of time to setuo the environment and also felt sagemaker was abit difficult to use than kaggle for training. My training got me of 0.50215 as score.

### What was the top ranked model that performed?

The top performing model was WeightedEnsemble with the score value of -54.644837

## Exploratory data analysis and feature creation

### What did the exploratory analysis find and how did you add additional features?

I observed that the temperature categories followed a normal distribution based on the data. To enhance my model, I decided to divide the datetime feature into separate components, including year, month, day, and hour. This had a significant positive impact on the performance of the model. Regarding the season, I noticed distinct patterns representing the four seasons in the distribution. Similarly, the weather feature exhibited three distinct input categories. Workday and holiday are binary fields, while humidity and windspeed showed left and right skewness, respectively.

### How much better did your model preform after adding additional features and why do you think that is?

The model perfomance got better by adding new features to the initial model. the score improved from 1.88027 to 0.64925. This according to me happened due to splitting of data feilds and result.

## Hyper parameter tuning

### How much better did your model preform after trying different hyper parameters?

The best performing model was hpo model. The score increased from 0.64925 to 0.50215. I went through the guidelines and some online resources to have better tuning and working of the model.

### If you were given more time with this dataset, where do you think you would spend more time?

Would try to get more model knowledge and how ensembling right model could increase the score.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.

|model|score|
"initial"|1.88027
"add_features"|0.64925
"hpo"|0.50215

### Create a line plot showing the top model score for the three (or more) training runs during the project.

![image](https://github.com/Yuktha2708/Predict-Bike-Sharing-Demand-with-AutoGluon/assets/76445341/fef6458f-4cdd-4a4a-abea-6fdb6f4b23c4)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

![image](https://github.com/Yuktha2708/Predict-Bike-Sharing-Demand-with-AutoGluon/assets/76445341/44b33135-839b-4c60-a756-daee73be858f)

## Summary

Working with the features and conducting EDA provides significant benefits and valuable insights. My primary objective would be to enhance the model by incorporating the influence of working hours on bike demand and capturing the seasonal fluctuations in demand, characterized by spikes and lows. By considering these factors, aiming to improve the accuracy and effectiveness of the model in predicting bike usage.
