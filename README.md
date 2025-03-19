# Tweet Sentiment Analysis
## 🧸Overview
This project focuses on analyzing the sentiment of tweets using Natural Language Processing (NLP). The goal is to classify tweets into sentiment categories such as positive, negative, and neutral based on their textual content.

## 🧸Dataset
The dataset consists of tweets with labeled sentiment categories. Each entry typically includes:
- **Text**: The actual tweet content
- **Sentiment Label**: Categorical labels (0 = Negative, 1 = Neutral, 2 = Positive)

## 🧸Feature Engineering
- **Preprocessing**: Cleans tweets by removing special characters, URLs, and expanding contractions

## 🧸Model Architecture
This project analyzes the sentiment of tweets using two different models:

**1. PyTorch-based Text Classifier**
  - **Embedding Layer**: `nn.EmbeddingBag` to handle word embeddings efficiently
  - **Dropout Layer**: Prevents overfitting by randomly dropping activations
  - **Fully Connected Layer**: Maps the extracted features to sentiment classes
  - **Weight Initialization**: Custom initialization for embeddings and linear layers
    
**2. VADER (Valence Aware Dictionary and sEntiment Reasoner) – A rule-based sentiment analysis tool**
  - **Model**: `nltk.sentiment.vader.SentimentIntensityAnalyzer`
  - **Hyperparameter Tuning**: Positive/Negative Threshold

**3. TensorFlow-based Text Classifier**
  - **Embedding Layer**: Pre-trained Universal Sentence Encoder from TensorFlow Hub for embedding text into 512-dimensional vectors
  - **Fully Connected Layer**: Maps the extracted features to sentiment classes
