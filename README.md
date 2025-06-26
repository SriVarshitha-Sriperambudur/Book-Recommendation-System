📚Book Recommendation System using Machine Learning


This project is a content-based book recommendation system built using Machine Learning and Natural Language Processing (NLP) techniques. It suggests books similar to a given title by analyzing the textual content (descriptions) of the books.

🚀 Project Overview

The Book Recommendation System leverages TF-IDF Vectorization and Cosine Similarity to compute the similarity between book descriptions. Based on the user's input (book title), it returns the top 5 most similar books.

This approach is ideal when you want to suggest recommendations based solely on the content, without relying on user ratings or reviews.

📂 Dataset

The dataset used is a collection of books with their corresponding titles and dBook Recommendation System using Machine Learningescriptions.

Initially, a CSV file with ~52,000 books was tested, but due to memory constraints, the final model was trained and evaluated on a refined dataset containing 1027 books.

Format: .xlsx (Excel) file

Columns used:

book_title

book_desc

🛠️ Technologies & Libraries Used
Python

Pandas

Scikit-learn

NumPy

SciPy

openpyxl (for reading Excel files)

🧠 ML/NLP Techniques

TF-IDF Vectorization: To convert book descriptions into numerical feature vectors.

Cosine Similarity: To measure the similarity between books.

K-Nearest Neighbors (KNN): For retrieving the closest books based on their vectorized features.

💡 How it Works

Loads and preprocesses the dataset (removing null descriptions).

Converts book descriptions into a sparse TF-IDF matrix.

Uses KNN with cosine distance to find similar books.

Takes a book title as input and returns 5 most similar titles based on content.

