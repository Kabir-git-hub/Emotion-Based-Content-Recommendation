🎬 Emotion-Based Content Recommendation System
An intelligent movie recommendation system powered by Natural Language Processing (NLP) and Machine Learning. This system detects the user's current emotional state from text input and suggests movies that align with their mood.
🚀 Overview
Unlike traditional recommendation systems that rely solely on watch history, this project uses Real-time Emotion Analysis. By analyzing the sentiment behind a user's words, the system classifies the mood into categories like Joy, Sadness, Anger, Fear, Surprise, or Love and recommends movies from the TMDB dataset accordingly.
✨ Features
Real-time Emotion Detection: Uses a trained Multinomial Naive Bayes model to predict emotions from text.
Dynamic Content Mapping: Maps movie genres (Comedy, Horror, Drama, etc.) to specific human emotions.
Natural Language Processing: Implements text cleaning, stopword removal, and TF-IDF vectorization.
Interactive UI: Simple input-output interface in Google Colab.
🛠️ Tech Stack
Language: Python 3.x
Environment: Google Colab / Jupyter Notebook
Libraries:
Pandas & NumPy (Data Manipulation)
Scikit-learn (Machine Learning & Vectorization)
NLTK (Natural Language Processing)
Re (Regular Expressions)
📊 Datasets Used
Emotions Dataset for NLP: Used for training the emotion classifier (contains text labeled with 6 emotions).
TMDB 5000 Movie Dataset: Used to fetch movie titles, ratings, and genres.
⚙️ How It Works
Text Preprocessing: User input is cleaned (lowercase, removing special characters, and removing stopwords).
Vectorization: Text is converted into numerical data using TfidfVectorizer.
Classification: A MultinomialNB model predicts the emotion.
Recommendation: The system filters the movie dataset based on the predicted emotion and suggests 5 random highly-rated movies.
📝 How to Run
Clone this repository or download the .ipynb file.
Upload the train.txt and tmdb_5000_movies.csv files to your environment.
Run all the cells in the notebook.
When prompted "How are you feeling right now?", type your mood and press Enter.
📌 Example
Input: "I had a very productive day and I'm feeling wonderful!"
Detected Emotion: JOY
Recommendations:
🎬 Toy Story | Rating: 7.7
🎬 Bruce Almighty | Rating: 6.7
🎬 Finding Nemo | Rating: 7.6
