# Airline Sentiment Analysis using NLP and Machine Learning

## Overview

This project focuses on sentiment analysis of airline-related tweets using Natural Language Processing (NLP) and Machine Learning techniques. The objective is to classify tweets into **Positive**, **Negative**, and **Neutral** sentiments by applying different text preprocessing, feature extraction, and classification methods.

The project compares multiple machine learning approaches to evaluate their effectiveness in sentiment classification and deploys the best-performing model through a Flask web application.

---

## Dataset

The project uses the **Twitter US Airline Sentiment Dataset** from Kaggle.

The dataset contains airline-related tweets labeled as:

* Positive
* Negative
* Neutral

---

## Project Workflow

### Data Preprocessing

The following preprocessing techniques were applied:

* Text cleaning
* Lowercasing
* Stopword removal
* Punctuation removal
* HTML tag removal
* Lemmatization
* Part-of-Speech (POS) based normalization

### Feature Extraction

The following NLP techniques were explored:

* Bag of Words (BoW)
* TF-IDF Vectorization
* Word2Vec

### Machine Learning Models

Several classification models were implemented and compared:

* Multinomial Naive Bayes
* K-Nearest Neighbors (KNN)
* Random Forest

A baseline model without traditional vectorization techniques was also evaluated.

---

## Results

| Model                   | Accuracy |
| ----------------------- | -------- |
| Without Vectorization   | ~78%     |
| Multinomial Naive Bayes | ~89%     |
| K-Nearest Neighbors     | ~85–87%  |
| Random Forest           | ~85–87%  |

Among the evaluated models, **Multinomial Naive Bayes** achieved the best overall performance and was selected for deployment.

---

## Deployment

The final model was deployed using:

* Flask
* Pickle Serialization
* HTML Frontend

The application allows users to enter airline-related tweets and receive real-time sentiment predictions.

---

## Repository Structure

```text
airline-sentiment-analysis/
│
├── Airline_Sentiment_Analysis_Without_Vectorization.ipynb
├── Multinomial_NB_Airline_Sentiment_Analysis.ipynb
├── KNN_Airline_Sentiment_Analysis.ipynb
├── RF_Airline_Sentiment_Analysis.ipynb
│
├── app.py
├── nlp_model.pkl
├── transform.pkl
├── Procfile
│
├── Tweets.csv
├── README.md
└── LICENSE
```

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* NLTK
* Flask
* Jupyter Notebook
* Pickle

---

## Key Learnings

Through this project, I gained hands-on experience in:

* Natural Language Processing workflows
* Text preprocessing and feature engineering
* TF-IDF and Bag of Words vectorization
* Training and evaluating machine learning models
* Model comparison and performance analysis
* Building and deploying a Flask-based ML application
* Working with real-world social media datasets

---

## Future Improvements

Potential enhancements include:

* Hyperparameter optimization
* Integration of transformer-based models such as BERT
* Multilingual sentiment analysis
* Cloud deployment using modern hosting platforms
* Interactive dashboard for model evaluation

---

## License

This project is distributed under the MIT License.
