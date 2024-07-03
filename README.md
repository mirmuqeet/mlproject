``**Student Performance Prediction**``

- This project predicts the math scores of students based on various features. It's an end-to-end machine learning project implemented in Python and designed to run on a local server using Flask.

`Files and Directories`

`.ebextensions`

Contains configuration files for deployment on AWS Elastic Beanstalk.

`artifacts/`

**data.csv**: The original dataset.

**model.pkl**: The trained model.

**preprocessor.pkl**: The preprocessor used for data transformation.

**train.csv**: Training data split.

**test.csv**: Testing data split.

`notebook/`

**1. EDA STUDENT PERFORMANCE 1.ipynb**: Exploratory Data Analysis of the student performance dataset.
**2. MODEL TRAINING Stu Performance.ipynb**: Model training and evaluation notebook.

`src/`

**components/**: Contains the various components of the pipeline such as data ingestion, data transformation, and model training.

**pipeline/**: Manages the end-to-end pipeline.

init.py: Initializes the src module.

**exception.py**: Custom exception handling.

**logger.py:** Logging functionality.

**utils.py**: Utility functions.

`templates/`

Contains HTML templates for the web application.

`application.py`

The main Flask application that runs the prediction model on a local server.

`requirements.txt`

Lists all the dependencies required to run the project.

`setup.py`

Script for setting up the project environment



`**Usage**`

Navigate to http://127.0.0.1:5000/ in your web browser to access the web application.

`Data`

The dataset (data.csv) contains the following columns:

gender

race/ethnicity

parental level of education

lunch

test preparation course

math score

reading score

writing score


`**Project Objective:**`

Predict the math scores of students based on features such as gender, race/ethnicity, parental level of education, lunch, and test preparation course.

`Data Handling:`

The dataset is split into training and testing sets.

Data preprocessing steps include handling missing values, encoding categorical variables, and scaling numerical features.

`Model Training:`

Multiple models were trained and evaluated, with the best model saved as model.pkl.

`CatBoost` was used for model training and hyperparameter tuning.

`Pipeline:`

The end-to-end pipeline includes data ingestion, transformation, and model training.

`Deployment:`

Although not yet deployed, the project includes configuration files for AWS Elastic Beanstalk.

The application runs locally using Flask and provides a web interface for predictions.

