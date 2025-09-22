# Text Analysis Project for Flipkart from Apify Instagram Scraper

## Project Title
**Flipkart Instagram Caption Analysis**

**Description:**  
This project performs a complete workflow for Instagram text analysis on Flipkart’s social media captions. It covers **data preprocessing, sentiment analysis, topic modeling, and word cloud visualization**. The aim is to extract insights from social media content and understand audience sentiment.

---

## 📝 Project Overview

- Collected Instagram captions from Flipkart (Excel file format).  
- Preprocessed text to **clean and normalize** it for analysis.  
- Conducted **sentiment analysis** using TextBlob to classify captions as **Positive, Negative, or Neutral**.  
- Performed **topic modeling** using NMF to discover main themes in the captions.  
- Visualized important words using **bar charts** and **word clouds**.  

---

## Step-by-Step Workflow

### Step 1: Load Data
- Imported the Excel file using **pandas**.  
- Checked all available sheets.  
- Loaded the main sheet containing Instagram captions.  

### Step 2: Preprocess Captions
- Converted all text to **lowercase**.  
- **Removed special characters** to normalize text.  
- **Tokenized** captions into individual words.  
- **Removed stopwords** to focus on meaningful words.  
- Saved preprocessed data to `flipkart_preprocessed.xlsx`.  

### Step 3: Sentiment Analysis
- Calculated **polarity scores** for each caption using **TextBlob**.  
- Categorized captions into:  
  - **Positive:** polarity > 0.05  
  - **Neutral:** -0.05 ≤ polarity ≤ 0.05  
  - **Negative:** polarity < -0.05  
- Saved results to `reviews_with_sentiment.xlsx`.  
- Visualized **sentiment distribution** using a **pie chart**.  

### Step 4: Topic Modeling
- Applied **TF-IDF vectorization** to convert text into numerical features.  
- Used **Non-Negative Matrix Factorization (NMF)** to discover topics.  
- Extracted **top words for each topic**.  
- Plotted **horizontal bar charts** to visualize the importance of words per topic.  

### Step 5: Word Cloud Visualization
- Generated **word clouds** for each topic.  
- Used **WordCloud** library with NMF weights to highlight important words.  
- Visualized the most significant words per topic clearly.  

---

## 📊 Results

- **Sentiment distribution:**  
  - Neutral: 101  
  - Positive: 87  
  - Negative: 12  
- **Main topics identified** with top words representing Flipkart campaigns, sales, and products.  
- **Word clouds** provide a visual summary of each topic’s key terms.  

---

## 🛠 Tools & Libraries Used

- **Python 3.11+**  
- **Jupyter Notebook**  
- **Pandas** – Data manipulation  
- **NLTK** – Text preprocessing & tokenization  
- **TextBlob** – Sentiment analysis  
- **scikit-learn** – TF-IDF vectorization & NMF for topic modeling  
- **Matplotlib** – Chart visualizations  
- **WordCloud** – Word cloud visualizations  
