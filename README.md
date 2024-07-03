## Industrial-Copper-Modeling

# Project Overview
This project focuses on modeling the selling price and status of industrial copper using machine learning techniques. The data is preprocessed, and various models are trained to predict the selling price and status of the copper transactions. The results are presented using a Streamlit application for interactive predictions.

# Jupyter Notebook Presentation
# 1. Data Loading and Exploration
Explanation: We start by loading the dataset and performing an initial exploration to understand the structure and content of the data.
Key Points:
Loaded data from a CSV file.
Explored the data using head(), info(), and describe() to get an overview of the dataset.
# 2. Data Cleaning and Preprocessing
Explanation: Data cleaning and preprocessing are essential to prepare the data for modeling. We handle missing values, encode categorical variables, and scale numerical features.
Key Points:
Converted data types and handled missing values.
Used OrdinalEncoder and OneHotEncoder for encoding categorical features.
Applied StandardScaler for scaling numerical features.
# 3. Model Training and Evaluation
Explanation: We train a Decision Tree Regressor to predict the selling price and use GridSearchCV for hyperparameter tuning to improve model performance.
Key Points:
Split data into training and testing sets using train_test_split.
Trained a Decision Tree Regressor.
Used GridSearchCV for hyperparameter tuning.
Evaluated model performance using metrics like Mean Squared Error (MSE) and R-squared.
# 4. Saving the Model
Explanation: The trained model and preprocessing objects are saved using pickle for later use in the Streamlit application.
Key Points:
Saved the trained model, scaler, and encoders to disk using pickle.

## Streamlit Application Presentation
Overview
Explanation: The Streamlit application provides an interactive interface for users to input features and get predictions for the selling price and status of copper transactions.
# Key Points:
The application is divided into two tabs: "PREDICT SELLING PRICE" and "PREDICT STATUS".
1. User Interface
Explanation: The UI is designed with dropdown menus and input fields for users to provide the necessary features for predictions.
# Key Points:
Dropdown menus for categorical features such as status, item type, and country.
Input fields for numerical features like quantity, thickness, and width.
2. Model Loading and Prediction
Explanation: The application loads the pre-trained models and scalers, preprocesses the user inputs, and provides predictions.
# Key Points:
Models and scalers are loaded using pickle.
User inputs are preprocessed in the same way as during model training.
Predictions are made and displayed on the interface.
