📰 Fake News Classification System


📌 Project Overview

In the era of information overload, identifying the authenticity of news is a critical challenge. This project implements a Machine Learning solution to classify news articles as either Real or Fake. By utilizing Natural Language Processing (NLP) techniques, the system processes textual data to identify patterns and linguistic features characteristic of misinformation.

🚀 Key Features
Text Preprocessing: Full implementation of data cleaning, including removal of stop words, punctuation, and special characters.

Stemming: Reducing words to their root form using the PorterStemmer to improve model efficiency.

Vectorization: Converting text data into numerical format using the TfidfVectorizer (Term Frequency-Inverse Document Frequency).

Binary Classification: A trained Logistic Regression model optimized for determining the veracity of news content.

📊 Methodology & Workflow
Data Acquisition: Processing a dataset containing news titles, authors, and body text.

Data Cleaning:

Handling missing values by filling nulls with empty strings.

Merging 'Author' and 'Title' fields to create a rich feature set.

NLP Pipeline:

Regex Operations: Filtering out non-alphabetic characters.

Stop Word Removal: Eliminating common words (e.g., "the", "a") that do not contribute to the meaning.

Stemming: Standardizing words to ensure the model recognizes different forms of the same word.

Feature Extraction: Transforming the processed text into a matrix of TF-IDF features.

Model Training: Splitting the data into training and testing sets, followed by model fitting using Logistic Regression.

🛠️ Tech Stack
Language: Python

NLP Tools: NLTK (Natural Language Toolkit)

Data Analysis: NumPy, Pandas

Machine Learning: Scikit-Learn (Logistic Regression, TF-IDF, Accuracy Score)

⚙️ Installation & Setup
Clone the Repository:

Bash
git clone https://github.com/Sheesaliakbar/fake-news-detector.git
Install Dependencies:

Bash
pip install numpy pandas nltk scikit-learn
Download NLTK Data:
Ensure the stopwords corpus is downloaded within your Python environment:

Python
import nltk
nltk.download('stopwords')
📈 Performance
The model is evaluated using the Accuracy Score, providing a reliable metric for its ability to correctly identify fake news articles from the test dataset.
