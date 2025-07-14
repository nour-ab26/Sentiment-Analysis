# 📊 Sentiment Analysis on Social Media Posts

This project is a complete pipeline for sentiment analysis using social media text data. It involves cleaning and preprocessing text data, visualizing trends, training a machine learning model, and testing it for classifying sentiments as **positive**, **neutral**, or **negative**.


## 📁 Dataset Description

The dataset used is `sentiment_analysis.csv`, containing 499 entries with the following columns:

- **Year**: Year of the post
- **Month**: Month of the post
- **Day**: Day of the post
- **Time of Tweet**: Morning / Noon / Night
- **Text**: The content of the social media post
- **Sentiment**: Target label – `positive`, `neutral`, or `negative`
- **Platform**: Platform from which the post originated (e.g., Twitter, Facebook, Instagram)



## 🔍 Exploratory Data Analysis

Several visualizations were used to understand the data:

- Distribution of sentiments
- Sentiment trends by year, time of day, and platform
- Total word count before and after preprocessing



## 🧹 Text Preprocessing

The text data was cleaned and prepared using the following steps:

- Removal of special characters and digits
- Conversion to lowercase
- Removal of stopwords (using `nltk`)
- Stemming using `PorterStemmer`

This process reduced the total word count from **5732** to **3064**.



## 🧠 Model Training

- Texts were vectorized using `TfidfVectorizer`.
- The dataset was split (80% training, 20% testing).
- Model used: **Support Vector Machine (SVM)** classifier.

### ✅ Evaluation Metrics

- **Accuracy**: `0.7300`
- **Weighted F1-Score**: `0.7247`


### 📦 Requirements
- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- nltk

