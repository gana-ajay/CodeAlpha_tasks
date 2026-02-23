# Sentiment Analysis - Natural Language Processing (NLP) Project

## 📊 Project Overview
This project performs sentiment analysis on customer feedback using Natural Language Processing (NLP) techniques. The analysis classifies text data into positive, negative, and neutral sentiments, comparing TextBlob's automated predictions against actual labeled sentiments to evaluate model performance.

## 🎯 Project Objectives
- Perform sentiment classification on customer reviews/feedback
- Compare TextBlob's sentiment predictions with actual labels
- Evaluate model accuracy and performance metrics
- Visualize sentiment distribution patterns

## 📁 Dataset Overview
- **Total Records**: 50 entries
- **Features**: 2 columns (text, sentiment)
- **Data Types**: Object (string) for both columns
- **Class Distribution**:
  - Positive: 17 samples
  - Negative: 17 samples
  - Neutral: 16 samples
- **Balanced dataset** with equal representation

## 🔧 Data Preprocessing

### Text Cleaning Steps:
1. **Lowercase conversion** - Standardized all text to lowercase
2. **Regex cleaning** - Removed special characters and non-alphabetic symbols
3. **Whitespace handling** - Cleaned extra spaces

### Code Implementation:
```python
def clean_text(text):
    text = str(text).lower()
    text = re.sub(r'[\^a-z\s]', '', text)
    return text