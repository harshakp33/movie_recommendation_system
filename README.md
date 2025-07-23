# movie_recommendation_system
This project is a Content-Based Movie Recommendation System developed using Python and built in Google Colab. It suggests movies similar to a user-given title based on textual features like genre, keywords, and overview. The system uses TF-IDF vectorization and cosine similarity to find and recommend the most relevant films.

## 📌 Project Overview

This system recommends top 10 movies that are similar in content to a selected movie. It uses **TF-IDF Vectorization** and **Cosine Similarity** to measure the closeness between movies.

## 🎯 Objective

- Take a movie name as input
- Compare its content with all other movies
- Recommend similar movies based on textual metadata

## 📁 Dataset

- **Source**: [Kaggle - TMDb Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)
- **File Used**: `tmdb_5000_movies.csv`
- **Important Columns**: `title`, `genres`, `overview`, `keywords`

- 
## 🛠️ Technologies Used

- **Platform**: Google Colab (Python Notebook)
- **Libraries**:
  - `pandas` for data processing
  - `scikit-learn` for TF-IDF and cosine similarity
  - `Google Colab` for interactive development
 
  - ## 🧠 How It Works

1. Load movie metadata
2. Combine content features (genre + overview + keywords)
3. Convert combined text into vectors using `TfidfVectorizer`
4. Calculate cosine similarity between all movie vectors
5. Recommend top 10 similar movies

6. ## 💡 Sample Code

```python
recommend("Avatar")
## 💡 Sample Code

 #output
['Aliens',
 'Alien³',
 'Mission to Mars',
 'Treasure Planet',
 'The Fifth Element',
 'Moonraker',
 'Planet of the Apes',
 'Battle: Los Angeles',
 'Alien',
 'Interstellar']

