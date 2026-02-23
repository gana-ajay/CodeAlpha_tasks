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
```
## Sentiment Analysis Methodology
# Tool Used: TextBlob
TextBlob's sentiment analysis uses a pre-trained model that returns:

Polarity Score: Ranges from -1 (negative) to +1 (positive)

Classification Rules:

Polarity > 0 → Positive

Polarity < 0 → Negative

Polarity = 0 → Neutral
### 📊 Model Performance Metrics
# Classification Report:
Class	Precision	Recall	F1-Score	Support
Negative	0.81	0.76	0.79	17
Neutral	0.43	0.19	0.26	16
Positive	0.56	0.88	0.68	17
Overall Accuracy: 62%
Average Metrics:
Metric	Macro Avg	Weighted Avg
Precision	0.60	0.60
Recall	0.61	0.62
F1-Score	0.58	0.58
### 🔍 Key Insights
# Model Strengths:
High Recall for Positive (88%) - Excellent at identifying positive sentiment

Strong Negative Detection - 81% precision for negative class

Good Negative F1-Score (0.79) - Reliable for negative sentiment classification

# Areas for Improvement:
Neutral Class Performance - Only 19% recall, 0.26 F1-score

Positive Precision (56%) - Some false positives in positive predictions

Overall Accuracy (62%) - Room for improvement with more sophisticated models

# 📈 Sentiment Distribution
Actual vs Predicted Comparison:
Sentiment	Actual Count	Predicted Count
Positive	17	~25
Negative	17	~15
Neutral	16	~10
Key Observation:
TextBlob tends to over-predict positive sentiment

Neutral sentiment is under-detected, often misclassified as positive

# 📊 Visualizations
Predicted Sentiment Distribution Bar Chart:
X-axis: Sentiment Categories (Positive, Negative, Neutral)

Y-axis: Count (0-25 range)

Shows higher positive predictions compared to actual distribution

# 🛠️ Technologies Used
Core Libraries:
Pandas - Data manipulation and analysis

Regular Expressions (re) - Text cleaning and preprocessing

TextBlob - Sentiment analysis engine

Matplotlib - Data visualization

Scikit-learn - Classification metrics and evaluation

Installation Requirements:
python
pip install pandas textblob matplotlib scikit-learn

# 💡 Business Applications
Customer Feedback Analysis - Automate review classification

Brand Monitoring - Track sentiment trends over time

Product Improvement - Identify pain points from negative reviews

Customer Support Triage - Prioritize negative feedback responses


# 📝 Sample Predictions
Text	Actual Sentiment	Predicted Sentiment
"I love this product"	Positive	Positive ✓
"This is the worst purchase I made"	Negative	Negative ✓
"It works fine"	Neutral	Positive ✗
"Amazing quality and fast delivery"	Positive	Positive ✓
"Terrible experience with customer support"	Negative	Negative ✓
### 🎓 Key Learnings
Text Preprocessing Matters - Cleaning significantly impacts accuracy

Neutral Sentiment is Challenging - Most difficult to detect accurately

Model Bias - TextBlob shows positive bias in predictions

Evaluation Metrics - Accuracy alone isn't sufficient; precision/recall provide deeper insights



