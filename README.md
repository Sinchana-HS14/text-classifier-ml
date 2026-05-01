# Review Sentiment Analysis System

## Overview

This project is a machine learning-based review analysis system that classifies user reviews into positive or negative categories. The system uses Natural Language Processing (NLP) techniques to preprocess text data and machine learning algorithms for classification.

The goal of this project is to build an end-to-end text classification pipeline and understand how machine learning can be applied to real-world review data.

---

## GitHub Repository

https://github.com/Sinchana-HS14/review-classification-system

---

## Problem Statement

User reviews on platforms such as movies, products, and services contain valuable feedback. Manually analyzing large volumes of reviews is inefficient. This project automates the process by classifying reviews as positive or negative using machine learning.

---

## Dataset

The dataset consists of labeled text reviews:

- train_data.csv: Training dataset with review text and sentiment labels
- test_data.csv: Testing dataset for model evaluation

Each record contains:
- review: User review text
- sentiment: Label (positive or negative)

---

## Methodology

### 1. Data Preprocessing
- Conversion of text to lowercase
- Removal of punctuation
- Removal of stopwords using sklearn English stopword list
- Tokenization of text

### 2. Feature Extraction
- TF-IDF Vectorization
- Use of n-grams (1,2) for better context representation

### 3. Model Training
- Algorithm used: Multinomial Naive Bayes
- Trained on TF-IDF transformed feature vectors

### 4. Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

---

## Results

- Accuracy: ~86%
- Balanced performance across both classes (positive and negative)
- Consistent precision and recall values indicate stable model performance

---

## Technologies Used

- Python
- Pandas
- Scikit-learn
- Natural Language Processing (NLP)

---

## Project Structure

review-classification-system/
│── train_data.csv
│── test_data.csv
│── Naive_bayes_classifier.ipynb
│── README.md

---

## How to Run the Project

### 1. Clone the repository
git clone https://github.com/Sinchana-HS14/review-classification-system.git

### 2. Navigate to project directory
cd review-classification-system

### 3. Install dependencies
pip install pandas scikit-learn

### 4. Run the notebook
Open the Jupyter Notebook and execute all cells

---

## Input and Output Example

Input:
"This movie was really good and enjoyable"

Output:
Positive

Input:
"The movie was boring and not worth watching"

Output:
Negative

---

## Future Improvements

- Implementation of Logistic Regression and SVM for performance comparison
- Integration of advanced models such as BERT for improved accuracy
- Development of a web interface using Streamlit
- Model persistence using pickle for deployment
- Hyperparameter tuning for improved performance
- Expansion of dataset for better generalization

---

## Learning Outcomes

- Understanding of text preprocessing techniques in NLP
- Implementation of TF-IDF vectorization
- Training and evaluation of machine learning models
- Building a complete machine learning pipeline
- Working with real-world text datasets

---

