# Amazon Food Reviews Sentiment Analysis

This repository contains sentiment analysis of Amazon Fine Food Reviews to identify factors influencing customer satisfaction.

## Project Overview

This project applies Natural Language Processing (NLP) techniques to analyze sentiment in Amazon food product reviews, extracting insights about what drives positive and negative customer experiences.

## Setup Instructions

### Step 1: Data Acquisition
- Download the dataset (database.sqlite) from [Kaggle](https://www.kaggle.com/snap/amazon-fine-food-reviews)
- Place the database.sqlite file in the working directory

### Step 2: Environment Setup
Required packages:
- sqlite3
- pandas
- numpy
- nltk
- string
- matplotlib
- seaborn
- sklearn
- re
- tqdm
- os
- collections

Python version: 3.7+

```bash
# Create a virtual environment (optional)
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# Install required packages
pip install -r requirements.txt

```

## License
Copyright © 2024 Ian Kamar. All rights reserved.
# 🍕 Amazon Fine Food Reviews - Sentiment Analysis

![Python](https://img.shields.io/badge/Python-3.7%2B-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![NLP](https://img.shields.io/badge/Natural%20Language-Processing-orange)

## 📌 Project Overview
Machine learning pipeline to analyze sentiment patterns in 500,000+ Amazon food product reviews. Identifies key drivers of customer satisfaction through:

- **Text Classification** (Positive/Negative sentiment)
- **Topic Modeling** (LDA/NMF)
- **Feature Importance** Analysis
- **Interactive Visualizations**

**Key Achievements:**
- 92% accuracy with BERT embeddings
- Identified top 5 complaint categories
- Automated report generation

## 📂 Dataset
[Amazon Fine Food Reviews](https://www.kaggle.com/snap/amazon-fine-food-reviews) (568,454 reviews)
```sql
SELECT Score, Text FROM Reviews WHERE Score != 3; -- 525,814 polarized reviews
