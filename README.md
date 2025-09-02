# Sentiment Analysis ML Project (Complete Pipeline)

This repository contains a complete machine learning pipeline for **sentiment analysis** of product reviews using Python and scikit-learn.

The project was developed as part of a learning module, where we demonstrated all typical phases of a machine learning workflow - from raw data to a ready-to-use trained model.

---

## Project structure

├── data/

│ └── product_reviews_full.csv #dataset

├── notebooks/

│ └── exploratory_analysis.ipynb # EDA and preprocessing

├── src/

│ └── train_model.py # Script for training and saving the model

│ └── test_model.py # Script for testing saved model

└── README.md

## What We Did in This Module

Throughout this module, we covered all major steps of real-world ML project:

### 1. Project Setup

- Created a new GitHub repository
- Defined project folder structure
- Uploaded raw dataset

### 2. Data Exploration

- Loaded and analyzed a large dataset with product reviews
- Used matplotlib and seaborn for visualizations
- Investigated distribution of sentiments and text characteristics

### 3. Data Cleaning & Preprocessing

- Removed missing values
- Standardized sentiment Labels (positive / negative / neutral)
- Parsed and validated prices
- Converted review text to numerical length

### 4. Feature Engineering

- Selected meaningful input feature: revie_title, review_text and review_length
- Removed irrelevant columns
- Explored correlation between price and sentiment

### 5. Model Training & Evaluation

- Compared multiple ML models (Logistic Regression, Naive Bayes, Decision Tree, Random Forest, SVM)
- Used ColumnTransformer and Pipeline for unified preprocessing
- Evaluated using precision, recall, F1-score and confusion matrix

### 6. Model Training

- Trained final model on full dataset
- Saved the pipeline using **joblib** to **sentiment_model.pkl**

### 7. Inference & Usage

- Loaded saved model
- Built an interactive interface for predicting sentimentof new reviews
- Enabled real time testing via console input

## How to Use

### Train the Model

---bash
cd src
python train_model.py
---

This will create a file called sentiment_model.pkl in the root directory.

### Run Inference
Use the interactive script (model_test.py) to classify new review using the trained model.

## Author
This repository was developed as part of an educational program on practical machine learning using Python.
All steps were carefully documented and modularized to help students undertand and reproduce the entire workflow.

## License
This project is open-source and freely available for educational use.
