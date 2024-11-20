# Stock Price Prediction with AWS and XGBoost

This project is a simple pipeline for predicting stock prices using an XGBoost model. The main idea is to train a machine learning model, deploy it using AWS SageMaker, and integrate it with other AWS services like Lambda, API Gateway, and SNS for real-time predictions and alerts.

## Basically it divides the pipeline in these stages:

- **Training the Model**: I used a Jupyter Notebook to train an XGBoost model on historical stock price data. The XGBoost model makes a prediction

- **Deploying the Model**: Once the model is trained, it’s deployed to AWS SageMaker as an endpoint. This means it’s ready to take in requests and return predictions.

- **Triggering Predictions**: An API Gateway and a Lambda function work together to let users send requests to the model. You can think of it like clicking a button and getting the predicted stock price.

- **Getting Alerts**: If something important happens (like the prediction crossing a threshold), an email alert is sent using Amazon SNS.

