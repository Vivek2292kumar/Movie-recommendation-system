# Movie-recommendation-system
A content-based movie recommendation system built using the TMDB 5000 dataset. It analyzes movie overviews, genres, cast, crew, and keywords to suggest similar titles. Cosine similarity and NLP techniques are used to compute recommendations.


## 📁 Dataset

- **TMDB 5000 Movies and Credits** from Kaggle.
- Files used:
  - `tmdb_5000_movies.csv`
  - `tmdb_5000_credits.csv`

## 🧠 Objective

To recommend movies that are similar to a given movie using natural language processing (NLP) and cosine similarity techniques.

## 🧰 Tools & Technologies

- Python
- Pandas, NumPy
- Scikit-learn
- NLTK
- Cosine Similarity
- Streamlit (for deployment, if applicable)

## ⚙️ Features Used for Recommendation

- Overview (description)
- Genres
- Cast
- Crew (Director)
- Keywords

These features are combined into a **"tags"** column which is processed using:
- Lowercasing
- Removing spaces
- Tokenization and stemming

## 📈 Methodology

1. **Data Merging & Cleaning**
2. **Feature Engineering** – Creating combined tags from relevant columns
3. **Text Vectorization** using `CountVectorizer`
4. **Similarity Score** calculation using cosine similarity
5. **Recommendation Function** that returns top 5–10 similar movies

## 💡 How It Works

```python
recommend("Avatar")

