# Text-Analysis-Project-for-Flipkart-from-Apify-Instagram-Scrapper
Text Analysis for Flipkart
Flipkart Instagram Caption Analysis

This project performs a complete workflow for Instagram text analysis on Flipkart’s social media captions. It covers data preprocessing, sentiment analysis, topic modeling, and word cloud visualization. The aim is to extract insights from social media content and understand audience sentiment.

📝 Project Overview

Collected Instagram captions from Flipkart (Excel file format).

Preprocessed text to clean and normalize it for analysis.

Conducted sentiment analysis using TextBlob to classify captions as Positive, Negative, or Neutral.

Performed topic modeling using NMF to discover main themes in the captions.

Visualized important words using bar charts and word clouds.

Step-by-Step Workflow

Step 1: Load Data

Imported the Excel file using pandas.

Checked all available sheets and loaded the main sheet containing captions.

Step 2: Preprocess Captions

Lowercased all text.

Removed special characters to normalize the text.

Tokenized captions into words.

Removed stopwords to focus on meaningful words.

Saved the preprocessed data to flipkart_preprocessed.xlsx.

Step 3: Sentiment Analysis

Used TextBlob to calculate polarity scores for each caption.

Categorized captions into:

Positive (polarity > 0.05)

Neutral (-0.05 ≤ polarity ≤ 0.05)

Negative (polarity < -0.05)

Saved results to reviews_with_sentiment.xlsx.

Visualized sentiment distribution with a pie chart.

Step 4: Topic Modeling

Applied TF-IDF vectorization to convert text into numerical features.

Used Non-Negative Matrix Factorization (NMF) to discover topics in the captions.

Extracted top words for each topic and plotted horizontal bar charts.

Step 5: Word Cloud Visualization

Generated word clouds for each topic to visualize the most important words.

Used WordCloud library with NMF weights as word importance.

📊 Results

Sentiment distribution:

Neutral: 101

Positive: 87

Negative: 12

Main topics identified with top words representing Flipkart campaigns, sales, and products.

Word clouds for visual representation of each topic.

🛠 Tools & Libraries Used

Python 3.11+

Jupyter Notebook

Pandas – Data manipulation

NLTK – Text preprocessing & tokenization

TextBlob – Sentiment analysis

scikit-learn – TF-IDF vectorization & NMF for topic modeling

Matplotlib – Visualization of charts

WordCloud – Visualization of topics
