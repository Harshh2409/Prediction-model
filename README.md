# Prediction-model

This project is a machine learning model that predicts whether a policy holder will churn. The model is trained on a dataset of historical data, and it can be used to predict the likelihood of churn for new and existing policy holders.

Installation
To install this project, you will need to have Python installed on your computer. Once you have Python installed, you can install the project by running the following command in your terminal:

pip install policy-holder-prediction-model

Usage
To use the model, you will need to import it into your Python code. Once you have imported the model, you can use it to predict the likelihood of churn for a policy holder by passing the policy holder's data to the predict() method.

The predict() method takes a dictionary of data as input. The keys of the dictionary should be the names of the features that you want to use to predict churn. The values of the dictionary should be the values of the features for the policy holder.

For example, to predict the likelihood of churn for a policy holder who is 35 years old, has been with the company for 5 years, and has a claim history of 2 claims, you would use the following code:

from policy_holder_prediction_model import PolicyHolderPredictionModel

model = PolicyHolderPredictionModel()

data = {
"age": 35,
"tenure": 5,
"claim_history": 2,
}

prediction = model.predict(data)

The prediction variable will contain the model's prediction for the likelihood of churn. The prediction will be a number between 0 and 1, where 0 indicates a low likelihood of churn and 1 indicates a high likelihood of churn.

