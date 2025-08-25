
# 🎬 Movie Recommendation System (MovieLens Dataset)

This project implements a **movie recommender system** using the [MovieLens Latest-Small Dataset](https://grouplens.org/datasets/movielens/latest/).  
It demonstrates **collaborative filtering** techniques and **matrix factorization** to generate personalized movie suggestions.

---

## 📖 Project Description
The system recommends movies for users based on their past ratings and the behavior of similar users.  
We use **three models**:
1. **User-Based Collaborative Filtering (User-CF)** – recommends movies by finding similar users.
2. **Item-Based Collaborative Filtering (Item-CF)** – recommends movies by finding similar movies.
3. **Matrix Factorization (SVD-MF)** – learns latent factors for users and movies.

The system evaluates recommendations using:
- **Leave-One-Out Split** (hold out 1 last rating per user for testing)
- **Precision, Recall, Accuracy @K**
- **Confusion Matrix Heatmaps**
- **Bar Charts comparing models**

---

## 🌟 Key Features
- Loads **MovieLens ratings.csv + movies.csv**
- Builds a **sparse user–movie rating matrix**
- Generates **Top-K recommendations** for each user
- Evaluates models with **Accuracy, Precision, Recall**
- Provides **visualizations** (bar chart + confusion matrix)
- Easily extendable for hybrid / deep models

---

## 📦 Requirements
Install required libraries with:

```bash
pip install numpy pandas scipy scikit-learn matplotlib seaborn
