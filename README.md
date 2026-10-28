# Sentiment Analysis Using Python and NLP

## Project Overview

This project explores text-based sentiment analysis using Python. It analyzes positive and negative reviews, examines text patterns, and applies Natural Language Processing (NLP) techniques to clean and prepare review data for machine learning.

The project demonstrates data exploration, text preprocessing, visualization, and feature extraction using the Bag-of-Words approach.

## Objectives

- Explore and understand a text review dataset.
- Analyze the distribution of positive and negative sentiments.
- Compare review lengths across sentiment categories.
- Visualize common words using word clouds.
- Clean text by removing URLs, punctuation, numbers, emojis, and other unwanted characters.
- Remove stop words and frequent words.
- Apply text normalization using lemmatization.
- Convert text into numerical features using CountVectorizer.
- Split the processed data into training and testing sets for machine learning.

## Technologies and Libraries

- Python
- Pandas and NumPy — data manipulation and analysis
- Matplotlib and Plotly Express — data visualization
- WordCloud — word frequency visualization
- NLTK — natural language processing and text preprocessing
- Regular Expressions (re) — text cleaning
- Scikit-learn — text vectorization and dataset splitting

## Project Workflow

1. **Data Loading and Exploration:** Load the review dataset and inspect its structure, summary statistics, and sentiment distribution.
2. **Exploratory Data Analysis:** Examine review lengths and compare positive and negative reviews using histograms.
3. **Text Visualization:** Generate separate word clouds for positive and negative reviews.
4. **Text Cleaning:** Convert reviews to lowercase and remove URLs, numbers, punctuation, emojis, and selected unwanted characters.
5. **Stop-Word and Frequency Filtering:** Remove common English stop words and the ten most frequent words in the processed corpus.
6. **Lemmatization:** Apply WordNet lemmatization to normalize words.
7. **Feature Extraction:** Use CountVectorizer to represent reviews as numerical word-count features.
8. **Train-Test Split:** Split the feature matrix and sentiment labels into training and testing sets using an 80:20 ratio.

## Dataset

The project uses a CSV file named `sentiment.csv` containing review text and sentiment labels.

Expected columns:
- `review` — the text of a review
- `sentiment` — the sentiment label, such as positive or negative

The dataset is loaded from Google Drive in the original notebook. Update the file path when running the project in another environment.

## Model Preparation

The sentiment labels are encoded as:
- `0` — Negative
- `1` — Positive

The reviews are transformed into a Bag-of-Words feature matrix using CountVectorizer. The data is then split into training and testing sets with an 80% training allocation and a 20% testing allocation.

**Note:** The current notebook prepares the data for model training. Model fitting, predictions, and evaluation metrics are not included in the code shared here.

## How to Run

1. Open the notebook in Google Colab or Jupyter Notebook.
2. Install any missing dependencies:

   ```bash
   pip install numpy pandas matplotlib plotly wordcloud nltk scikit-learn
   ```

3. Make the dataset available in your environment and update the CSV path.
4. Run the notebook cells in order.
5. Allow the required NLTK resources to download when prompted by the notebook.

## Skills Demonstrated

- Exploratory Data Analysis (EDA)
- Data cleaning and preprocessing
- Natural Language Processing (NLP)
- Text visualization
- Feature engineering
- Bag-of-Words representation
- Preparation of datasets for machine learning

## Future Improvements

- Train a sentiment classification model, such as Multinomial Naive Bayes or Logistic Regression.
- Evaluate performance using accuracy, precision, recall, F1-score, and a confusion matrix.
- Compare different text preprocessing strategies.
- Improve lemmatization by processing individual tokens.
- Test the model on unseen reviews.

## Conclusion

This project demonstrates an end-to-end text preprocessing workflow, from exploring review data to preparing numerical features for sentiment classification. It provides a foundation for further experimentation with machine learning-based sentiment analysis.
