# Disease Predictor Using Machine Learning

This project is a graphical user interface (GUI) application built using Python's Tkinter library that predicts diseases based on user input of symptoms. The prediction is carried out using three different machine learning algorithms: Decision Tree, Random Forest, and Naive Bayes.

## Table of Contents
- [Features](#features)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Machine Learning Algorithms](#machine-learning-algorithms)
- [Data](#data)
- [GUI](#gui)

## Features

- **Multiple Symptom Input:** Users can input up to five symptoms.
- **Machine Learning Models:** The application uses three machine learning models to predict diseases: Decision Tree, Random Forest, and Naive Bayes.
- **Real-Time Predictions:** The predictions are made in real-time based on the selected symptoms.
- **User-Friendly GUI:** The interface is built using Tkinter, making it easy for users to interact with the application.

## Installation

To run this project locally, follow these steps:

1. **Clone the Repository**
   ```bash
   git clone https://github.com/iamprabhanjan/disease-prediction-using-ml.git
   cd disease-predictor-ml
   ```

2. **Install Dependencies**
   Ensure you have Python installed, then run:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Application**
   ```bash
   python disease_predictor.py
   ```

## Usage

1. Upon running the application, a GUI window will appear.
2. Enter the patient's name in the "Name of the Patient" field.
3. Select up to five symptoms from the dropdown lists.
4. Click on one of the three buttons to use the respective machine learning model (Decision Tree, Random Forest, or Naive Bayes) to predict the disease.
5. The predicted disease will be displayed in the text box corresponding to the selected model.

## Machine Learning Algorithms

### 1. **Decision Tree**
   - A decision tree is a flowchart-like structure where each internal node represents a test on an attribute, each branch represents an outcome of the test, and each leaf node represents a class label.
   - The model is trained on the `Training.csv` dataset, and predictions are made based on the selected symptoms.

### 2. **Random Forest**
   - Random Forest is an ensemble learning method that operates by constructing multiple decision trees during training and outputting the mode of the classes as the prediction.
   - It reduces overfitting by averaging the predictions of multiple decision trees.

### 3. **Naive Bayes**
   - Naive Bayes is a probabilistic classifier based on Bayes' theorem. It assumes independence between predictors.
   - It is particularly effective for small datasets or when the assumption of independence is valid.

## Data

The project uses two datasets:

1. **Training.csv:** This dataset is used to train the machine learning models. It contains symptoms as features and the corresponding disease as the target variable.
2. **Testing.csv:** This dataset is used to validate the performance of the models. It follows the same structure as `Training.csv`.

## GUI

The GUI is built using Python's Tkinter library. It contains the following elements:

- **Labels and Text Fields:** To enter the patient's name and select symptoms.
- **Option Menus:** Dropdown lists to choose symptoms from a predefined list.
- **Buttons:** To trigger the prediction using one of the three models.
- **Text Boxes:** To display the predicted disease based on the selected model.
