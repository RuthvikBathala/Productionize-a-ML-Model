# **T20 Match Score Predictor**
## **Overview**

The T20 Match Score Predictor is a machine learning model deployed as a Streamlit web application. The model predicts the score of a T20 cricket match based on various input features such as batting team, bowling team, host city, current score, overs completed, wickets out, last five overs score, average score, and wickets in the last five overs.

The underlying machine learning model is built using XGBoost, a popular gradient boosting algorithm. The model is trained on a dataset containing historical T20 match statistics, including team performances, city information, and match outcomes.

## **Project Structure**

app.py: The Streamlit web application script. It defines the user interface, takes user inputs, and utilizes the pre-trained XGBoost model for score prediction.

model_training.ipynb: Jupyter Notebook containing the code for training the XGBoost regression model. It includes data preprocessing, model creation, and evaluation.

pipe.pkl: Pickle file containing the serialized pre-trained XGBoost model. This file is loaded in the Streamlit app for making predictions.

dataset.csv: The dataset used for training the model. It includes various features such as batting team, bowling team, city, delivery details, score, and final score.

## **Dependencies**

streamlit: Web application framework for creating interactive and shareable apps.

pandas: Data manipulation library for handling input data.

scikit-learn: Machine learning library for preprocessing and scaling.

xgboost: Gradient boosting library for building regression models.
