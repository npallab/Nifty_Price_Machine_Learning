This project is designed to predict the Nifty closing price for the next trading day using a linear regression model. The model takes as input the Open, High, Low, and Close prices for a given day and predicts the closing price for the following day.

**Project Overview**
*Problem Statement*
Predicting stock market movements is a complex task, but linear regression provides a simple yet effective approach to estimate future prices based on historical data. This project focuses on predicting the Nifty index's closing price using a linear regression model trained on past data.

**Approach**
Data Collection: The project begins with gathering historical Nifty index data, including the Open, High, Low, and Close prices for each trading day. This data is stored in a CSV file (train_data.csv).

**Data Preprocessing:** The dataset is cleaned and preprocessed to ensure there are no missing values or outliers that could skew the model's predictions.

**Model Training:** A linear regression model is trained using the scikit-learn library in Python. The model is trained to learn the relationship between the input features (Open, High, Low, and Close prices) and the target variable (next day's Close price).

**Model Evaluation:** After training, the model is evaluated using appropriate metrics such as Mean Squared Error (MSE) to ensure it performs well on unseen data.

**Model Saving:** The trained model, along with the regression parameters, is saved into a model.pkl file using Python’s pickle module. This allows for easy reuse of the model without needing to retrain it each time.

**User Interface:** A simple Python script (predict.py) is created to provide a user interface for predicting the next day’s Nifty closing price. This script loads the model from the .pkl file and takes user inputs for Open, High, Low, and Close prices to make predictions.

**Project Structure**
train_data.csv: The dataset containing historical Nifty index data used for training the model.
model.pkl: The serialized linear regression model and regressor, stored using Python's pickle module.
predict.py: A Python script that serves as a user interface for predicting the next day's Nifty closing price.
How to Use

**1. Train the Model (Optional)**
If you want to retrain the model with new data:

Load the train_data.csv into your Python environment.
Use the scikit-learn library to fit the linear regression model to the data.
Save the trained model to model.pkl using Python's pickle module.
