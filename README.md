# 🎬 Emotion-Based Content Recommendation System

An intelligent movie recommendation system powered by **Natural Language Processing (NLP)** and **Machine Learning**. This system analyzes the user's current feelings through text input and suggests movies that perfectly match their mood.

## 🚀 Overview
Traditional recommendation systems often suggest content based on historical data. This project introduces a **Mood-Aware Recommendation** approach. It uses a trained Machine Learning model to detect emotions (Joy, Sadness, Anger, Fear, Surprise, etc.) from natural language and maps them to movie genres to provide real-time personalized suggestions.

## ✨ Features
- **Real-time Emotion Detection:** Uses a trained Multinomial Naive Bayes model to classify text into 6 different emotions.
- **NLP Powered:** Implements advanced text cleaning, stopword removal, and TF-IDF Vectorization.
- **Smart Genre Mapping:** Dynamically connects human emotions to relevant movie genres (e.g., Sadness → Drama/Romance, Joy → Comedy).
- **Interactive Interface:** Easy-to-use input system within the Google Colab environment.

## 🛠️ Tech Stack
- **Language:** Python 3.x
- **Platform:** Google Colab
- **Libraries:** 
  - `Scikit-learn` (Machine Learning & Vectorization)
  - `NLTK` (Natural Language Processing)
  - `Pandas` (Data Manipulation)
  - `NumPy` (Numerical Computing)

## 📊 Datasets Used
1. **Emotions Dataset for NLP:** A labeled dataset containing thousands of text samples categorized into 6 basic human emotions.
2. **TMDB 5000 Movie Dataset:** A comprehensive dataset containing movie titles, genres, and user ratings.

## ⚙️ How It Works
1. **Data Cleaning:** The input text is processed to remove special characters and common "stopwords."
2. **Model Training:** The model is trained using the **Multinomial Naive Bayes** algorithm to understand the relationship between words and emotions.
3. **Emotion Prediction:** When a user types how they feel, the model predicts the dominant emotion.
4. **Content Filtering:** The system filters the movie list based on the predicted emotion and selects 5 random high-rated movies.

## 📝 How to Run
1. Open the project in **Google Colab**.
2. Upload the required files: `train.txt` and `tmdb_5000_movies.csv`.
3. Run all cells in sequence.
4. When prompted, type your mood (e.g., *"I'm having a great day!"*) and press **Enter**.

## 📌 Example Output
**User Input:** *"I feel very lonely and sad today."*  
**Detected Emotion:** `SADNESS`  
**Suggested Movies:**  
- 🎬 The Shawshank Redemption | Rating: 8.5
- 🎬 Forrest Gump | Rating: 8.2
- 🎬 The Fault in Our Stars | Rating: 7.6

---
**Developed by:** Al Amin Kabir
**Topic:** Machine Learning & NLP Project
