# Sentiment Analysis for Fun Football FIFA and PSSI
This repository contains code and data for performing sentiment analysis on tweets related to fun football, FIFA, and PSSI (Football Association of Indonesia). The dataset used in this analysis has been manually collected from Twitter and manually labeled.

## Code Overview
The code provided here includes various components for sentiment analysis, including text preprocessing, feature extraction, model training, and evaluation. Here's a brief overview of the code sections:

### Importing Libraries
The code starts by importing necessary libraries for data manipulation, text processing, feature extraction, classification, and data visualization. These libraries include Pandas, NumPy, scikit-learn, Matplotlib, Seaborn, and others.

### Text Preprocessing
Text preprocessing is a crucial step in sentiment analysis. The preprocessing function is defined to clean the text by removing HTML tags, square brackets, punctuation, and non-ASCII characters. It also converts text to lowercase. This function is applied to the tweet text.

### Word Clouds
Word clouds are generated for the entire dataset and for each sentiment class (positive, negative, neutral) using the create_word_cloud function. Word clouds provide a visual representation of the most frequent words in the text.

### Sentiment Analysis
The dataset is divided into three sentiment classes: positive, negative, and neutral. Stop words are removed from the text using the Sastrawi library. The code then performs sentiment analysis using the Multinomial Naive Bayes classifier.

### Confusion Matrix
Two confusion matrices are generated to evaluate the model's performance: one without normalization and one with normalization. These matrices provide insights into the model's predictions.

### Model Evaluation
The code calculates various evaluation metrics, including accuracy, recall, precision, and F1-score, to assess the model's performance. These metrics are displayed in the classification report.

### Test Data
The code also includes a section for testing the model on additional data. Test data is preprocessed, and sentiment labels are predicted using the trained model. The accuracy score and a pie chart of predicted sentiment labels are displayed.

## Usage
1. Make sure you have the required libraries installed. You can install them using pip:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn wordcloud sastrawi beautifulsoup4 textblob
```
2. Prepare your dataset of manually collected tweets and save it as datasetFunFootball.csv. The dataset should contain two columns: "Sentence" (tweet text) and "Sentimen" (sentiment label: -1 for negative, 0 for neutral, 1 for positive).
3. Create a test dataset (if necessary) and save it as dataujiFunFootball.csv.
4. Run the provided code in your Python environment.

## Results
The code provides insights into sentiment analysis for fun football, FIFA, and PSSI tweets. It evaluates the model's performance and can be used to analyze sentiments in new test data.

Please note that the provided code assumes you have the necessary libraries installed and have prepared your dataset according to the specified format.
