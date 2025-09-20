
# Yelp Restaurant Recommender System

This project builds a personalized restaurant recommendation engine using Yelp reviews and business metadata. It integrates sentiment analysis and collaborative filtering to predict star ratings and recommend top restaurants.

## Objectives
- Combine user reviews and restaurant data from Yelp.
- Analyze review sentiments using VADER.
- Predict star ratings using Latent Factor Models (Baseline and Truncated SVD).
- Recommend Top 10 restaurants per user.

## Dataset
- Sourced from [Yelp Dataset on Kaggle](https://www.kaggle.com/datasets/yelp-dataset/yelp-dataset)
- Used:  
  - `yelp_academic_dataset_review.json`  
  - `yelp_academic_dataset_business.json`

## Techniques Used:
- **Sentiment Analysis**: VADER
- **Dimensionality Reduction**: Truncated Singular Value Decomposition (SVD)
- **Baseline Models**: Popularity-based, user mean, business mean
- **Evaluation Metric**: Mean Squared Error (MSE)

## Results
- MSE on Test Data: **0.0168**
- Recommendations are personalized using latent factor embeddings, sentiment, and state-based context.

## Project Structure
```
.
├── YelpRecommenderSystem.py # Main codebase
├── YelpRecommenderSystem.ipynb # Colab development notebook
├── ProjectReport.pdf # Final project report
└── README.md # About the project
```

## Setup
```bash
pip install pandas numpy scikit-learn matplotlib nltk vaderSentiment
```

## Run
```bash
python YelpRecommenderSystem.py
```
