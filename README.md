# 🎬 Movie Recommendation System with KNN & Surprise

This repository demonstrates a User-Based Collaborative Filtering recommender system built using the Python `scikit-surprise` library on the popular MovieLens 100k (`ml-100k`) dataset.

## 🚀 Overview

The system predicts movie ratings and generates top-N personalized movie recommendations for users by finding similar user profiles using Cosine Similarity within a k-Nearest Neighbors (KNN) algorithm framework.

## 🧠 Methodology & Workflow

1. **Dataset Loading:** Uses the built-in MovieLens 100k dataset containing user IDs, item IDs (movies), and ratings.
2. **Train/Test Split:** Splits user-item interaction records into 80% training and 20% testing sets.
3. **Similarity Modeling:** Configures `KNNBasic` with user-based cosine similarity (`user_based: True`).
4. **Evaluation:** Measures rating prediction error across test samples using Root Mean Squared Error (RMSE).
5. **Top-N Generation:** Groups predictions by user ID, sorts them in descending order based on estimated scores, and returns the top-N highest scoring movie recommendations.

## 🛠️ Tech Stack
- Python
- scikit-surprise

## 💻 Installation & Usage

1. Install dependencies:
pip install scikit-surprise

2. Run the script:
python recommender_knn.py

## 📊 Example Output

- Computes overall model performance metric:
  - `RMSE: ~1.01`
- Generates top 5 recommended movie IDs and their predicted ratings for a specified user:
  - `top 5 recommendation for user 2`
  - `item id: <movie_id>, score: <predicted_rating>`
