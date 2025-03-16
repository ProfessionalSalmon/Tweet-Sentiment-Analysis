# Tweet Sentiment Analysis
## 🧸Overview
This project focuses on analyzing the sentiment of tweets using Natural Language Processing (NLP). The goal is to classify tweets into sentiment categories such as positive, negative, and neutral based on their textual content.

## 🧸Dataset
The dataset consists of tweets with labeled sentiment categories. Each entry typically includes:
- Text: The actual tweet content
- Sentiment Label: Categorical labels (0 = Negative, 1 = Neutral, 2 = Positive)

## 🧸Model Architecture
The project uses a Text Classification Model built with PyTorch. The model consists of:
- Embedding Layer: nn.EmbeddingBag to handle word embeddings efficiently.
- Dropout Layer: Prevents overfitting by randomly dropping activations.
- Fully Connected Layer: Maps the extracted features to sentiment classes.
- Weight Initialization: Custom initialization for embeddings and linear layers to improve stability.
