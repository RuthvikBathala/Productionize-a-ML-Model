# **T20 Match Score Predictor**
## **Overview**

This project involves the development and deployment of a T20 Match Score Predictor using machine learning. The predictor is designed to estimate the final score of a T20 cricket match based on various input parameters. The machine learning model is trained on historical cricket match data, incorporating features such as batting team, bowling team, host city, current score, overs completed, wickets out, last five overs score, average score, and wickets in the last five overs.

## **Key Components**

**1. Machine Learning Model:** The project utilizes the XGBoost regression model, trained on a dataset containing diverse cricket match statistics. The model considers both numerical and categorical features, making predictions based on the input parameters provided by the user.

**2. Streamlit Web Application:** The user interacts with the model through a Streamlit web application. The application features a user-friendly interface where users can input relevant information such as batting team, bowling team, host city, current score, overs completed, wickets out, last five overs score, average score, and wickets in the last five overs.

**3. Deployment on Streamlit Cloud:** The trained model and the Streamlit app are deployed on Streamlit Cloud, allowing users to access and utilize the T20 Match Score Predictor from any device with an internet connection.

## **Project Structure**

app.py: The Streamlit web application script. It defines the user interface, takes user inputs, and utilizes the pre-trained XGBoost model for score prediction.

model_training.ipynb: Jupyter Notebook containing the code for training the XGBoost regression model. It includes data preprocessing, model creation, and evaluation.

pipe.pkl: Pickle file containing the serialized pre-trained XGBoost model. This file is loaded in the Streamlit app for making predictions.

dataset.csv: The dataset used for training the model. It includes various features such as batting team, bowling team, city, delivery details, score, and final score.

## **Usage**
Users can select the participating teams, the host city, and input the current match statistics. Upon clicking the 'Predict Probability' button, the model processes the inputs and provides an estimated final score for the T20 match.

## **Outcome**
The deployed application serves cricket enthusiasts, analysts, and fans who are interested in predicting T20 match scores based on historical data. It provides a convenient and accessible tool for score estimation, potentially enhancing the overall cricket-watching experience.

**Technologies Used**

Python
Scikit-learn (for machine learning)
XGBoost
Streamlit (for web application development)
Streamlit Cloud (for deployment)

