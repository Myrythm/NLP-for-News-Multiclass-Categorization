# NLP for News Multiclass Categorization

This project demonstrates how to categorize news articles into multiple classes using Natural Language Processing (NLP) techniques and machine learning models. The goal is to build a text classification model that can automatically predict the category of news articles based on their content.

## Project Overview

1. **Dataset**: The dataset used in this project is sourced from Kaggle. It contains news articles categorized into five different topics: Business, Entertainment, Politics, Sport, and Tech.

2. **Data Preparation**:
   - **Loading the Dataset**: The dataset is downloaded and unzipped using Kaggle's API.
   - **Data Cleaning**: The text data is preprocessed to lower-case, remove punctuation, lemmatize words, remove numbers, and eliminate stopwords.

3. **Model Building**:
   - **Tokenization**: The text data is tokenized and padded to prepare it for model input.
   - **Model Architecture**: A Sequential model is created using TensorFlow/Keras with the following layers:
     - Embedding layer
     - LSTM layer
     - Dense layers
     - Dropout layer
   - **Training**: The model is trained with a custom callback to stop training once the accuracy exceeds 90% on both training and validation datasets.

4. **Evaluation**:
   - **Accuracy and Loss Plots**: Training and validation accuracy and loss are plotted to visualize model performance over epochs.
