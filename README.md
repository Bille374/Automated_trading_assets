# Machine Learning trading Bot

### As a financial advisor for top trading firm in world to keep competetion with other firms we have to manage and automatically trade assets by using a computer algorithms and machine learning.

### by enhancing the existing trading signals with machine learning algorithms that can adopt to new data

### problem:  people still need to specifically program their systems, which limits their ability to adopt to new data

### planning: to improve the existing algorithmic trading systems and maintain the firm competitive adavntage in the market

# Instructions

### The steps for this Challenge are divided into the following sections:

### Establish a Baseline Performance

### Tune the Baseline Trading Algorithm

### Evaluate a New Machine Learning Classifier

### Create an Evaluation Report

# Imports : make imports to model we do need in our analysis of dataset, then read ohlcv.csv file provided by the firm 
![Imports](https://user-images.githubusercontent.com/69637182/191531297-cc6e63a9-1863-4b73-af5e-296d0a08db74.png)
![Read_Data](https://user-images.githubusercontent.com/69637182/191531327-bf8b915f-055f-4b0a-8c94-6f58608a508e.png)

# Generate trading signals: which is the hardest part because it's assemption how the markert will react in that period chosen
wich was SMA_Fast= 2, SMA_slow=20

![signal](https://user-images.githubusercontent.com/69637182/191532051-9f647946-e3f2-46ca-99b1-87e3a0828807.png)
# Split y_train X_test dataset,fit model and scale it then balance y target 
![Spliting_Data_train_test](https://user-images.githubusercontent.com/69637182/191532764-c8c4d88d-a18a-4c50-8ff8-a8c9c48f2109.png)
![fit_model](https://user-images.githubusercontent.com/69637182/191532908-92de2e80-23d0-4651-8234-306edb7a4b07.png)
![Scaling_data](https://user-images.githubusercontent.com/69637182/191533313-739b6617-8940-4792-a3cf-b836d96888cb.png)

# apply DecisionTreeclassifier model from Sklearn:
![DecisionTreeclassifier](https://user-images.githubusercontent.com/69637182/191537527-fe22693d-5a11-4421-ad42-5e9e5e5c0e6a.png)

# Get classification report with  model predictions
![Classification report base Model](https://user-images.githubusercontent.com/69637182/191534094-40958bc2-4641-47ad-82ad-7a037abcbe48.png)
# Plot the actual returns versus the strategy returns: we can see that both graph supposed to get close to each other means our model did give good results
![Actual Returns vs Strategy Returns](https://user-images.githubusercontent.com/69637182/191534864-8c69db43-d130-4bc8-8ef0-cc87ba4679c6.png)


# Conclusion: 
By adding a new parameters to our base model and fix imbalances we have seen a bit impoving of accuracy of our trading algorithm returns
![algo_returns](https://user-images.githubusercontent.com/69637182/191539425-3561cf6a-0b44-4bf9-aca9-fee64505dd03.png)
