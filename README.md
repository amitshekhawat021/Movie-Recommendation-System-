
# Movie-Recommendation-System-

This project involves building a content-based movie recommendation system using machine learning techniques. The goal is to suggest movies that are similar to a given movie based on various features like genres, keywords, cast, and crew.

## Steps followed in the project:

Data Loading:

Two datasets were loaded — one containing movie details (movies.csv) and another with credits information (credits.csv).

Data Merging and Cleaning:

The datasets were merged on the movie title, and unnecessary columns were removed. The remaining columns were cleaned by:
Converting JSON-like strings into Python objects using ast.literal_eval.
Extracting important features like director, genres, cast, and keywords.
Combining all relevant textual data into a single column called tags.

Text Preprocessing:

All text data was converted to lowercase and spaces were removed from multi-word phrases.
Stemming was applied to reduce words to their root form using PorterStemmer from NLTK.

Feature Extraction:

The CountVectorizer from Scikit-learn was used to convert text data (tags) into numerical vectors.
A cosine similarity matrix was calculated to measure similarity between movies based on their tags.

Recommendation Function:

A function named recommend() was created, which takes a movie name as input and returns the top 5 most similar movies based on cosine similarity.

# Conclusion :

In this project, we built a smart system that can suggest movies similar to the one you like. We did this by looking at things like the movie's genre, keywords, cast, and director. We cleaned this data, turned it into numbers using machine learning tools, and calculated how similar the movies are to each other. The final result is a working movie recommendation system that gives good suggestions based on what a user searches for. This kind of model is helpful in apps like Netflix or IMDb to improve user experience.
