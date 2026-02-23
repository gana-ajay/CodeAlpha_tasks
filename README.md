# Code Alpha Internship Projects - Complete Portfolio
## 📌 Overview
This repository contains three data analysis projects completed during the Code Alpha internship program, demonstrating skills in Exploratory Data Analysis, Data Visualization, and Natural Language Processing.

## PROJECT 1: Sales Data Analysis (EDA)
📊 Exploratory Data Analysis
🎯 Objective
Analyze sales data to identify regional performance, category profitability, and sales-profit relationships.

📁 Dataset
Sales transactions with 8 columns (Order_ID, Date, Region, Product, Category, Sales, Quantity, Profit)

10+ records across multiple regions and categories

🔍 Key Questions Answered
Which region generates the highest sales?

Which category is most profitable?

Are higher sales giving higher profit?

Which product has low profit despite high sales?

📈 Key Findings
Region	Sales
South	₹80,000
North	₹57,500
East	₹37,000
West	₹30,000
Category	Profit
Furniture	₹17,400
Electronics	₹16,600
💡 Insights
South region dominates with highest sales (₹80,000)

Furniture is most profitable category (₹17,400)

Strong correlation (0.96) between sales and profit

No missing values or duplicates in dataset

🛠️ Tools Used
Python (Pandas, NumPy)

Matplotlib for visualizations

Jupyter Notebook

## PROJECT 2: Amazon Sales Dashboard
📊 Power BI Visualization
🎯 Objective
Create an interactive dashboard analyzing Amazon sales across regions, categories, and payment methods.

# 📁 Dataset Metrics
Total Quantity: 150K units

Average Rating: 3.00

Total Reviews: 12M

Monthly Revenue: $2.5M - $2.9M

# 📈 Regional Performance
Region	Revenue
Middle East	$8.3M
North America	$8.3M
Asia	$8.2M
Europe	$8.1M
# 📦 Category Quantity
Category	Units Sold
Beauty	25,422
Fashion	25,089
Books	25,065
Electronics	24,898
Sports	24,753
Home & Kitchen	24,743
# 💳 Payment Distribution
Cash on Delivery: 20.32%

UPI: 20.02%

Debit Card: 19.92%

Credit Card: 19.90%

Wallet: 19.84%

# ⭐ Ratings by Category
Books: 3.02 (Highest)

Sports: 3.00

Home & Kitchen: 3.00

Electronics: 2.99

Fashion: 2.99

Beauty: 2.99

# 📅 Monthly Trends
Peak: January ($2.88M)

Lowest: June ($2.51M)

Strong Q4 performance

# 💡 Key Insights
Balanced revenue across all regions ($8.1M-$8.3M)

Even payment method distribution (~20% each)

Beauty products lead in quantity sold

Books receive highest customer ratings

# 🛠️ Tools Used
Power BI Desktop

DAX Calculations

Power Query

## PROJECT 3: Sentiment Analysis
🧠 Natural Language Processing
🎯 Objective
Classify customer feedback into positive, negative, and neutral sentiments using TextBlob and evaluate model accuracy.

# 📁 Dataset
50 customer reviews/text samples

Balanced classes: 17 Positive, 17 Negative, 16 Neutral

Binary columns: text, sentiment

🔧 Preprocessing Steps
Lowercase conversion

Regex special character removal

Text cleaning and standardization

# 🧠 Methodology
python
def get_sentiment(text):
    polarity = TextBlob(text).sentiment.polarity
    if polarity > 0: return "positive"
    elif polarity < 0: return "negative"
    else: return "neutral"
# 📊 Model Performance
Class	Precision	Recall	F1-Score
Negative	0.81	0.76	0.79
Neutral	0.43	0.19	0.26
Positive	0.56	0.88	0.68
# 📈 Overall Accuracy: 62%
🔍 Sample Predictions
Text	Actual	Predicted
"I love this product"	Positive	Positive ✓
"This is the worst purchase"	Negative	Negative ✓
"It works fine"	Neutral	Positive ✗
"Amazing quality"	Positive	Positive ✓
"Terrible experience"	Negative	Negative ✓
# 💡 Key Insights
Strong negative detection (81% precision)

Excellent positive recall (88%)

Neutral sentiment challenging (only 19% recall)

TextBlob shows positive bias in predictions

# 🛠️ Tools Used
Python (Pandas, re)

TextBlob for sentiment analysis

Matplotlib for visualizations

Scikit-learn for metrics

# 📊 Projects Summary Table
Project	Type	Tools	Key Achievement
Sales EDA	Data Analysis	Python, Pandas	Found 0.96 sales-profit correlation
Amazon Dashboard	Visualization	Power BI	Created interactive business dashboard
Sentiment Analysis	NLP	TextBlob, Python	Achieved 62% accuracy in classification
🛠️ Common Technologies Used
Python (Pandas, NumPy, re, Matplotlib)

Power BI (DAX, Power Query)

Jupyter Notebook

Scikit-learn (Metrics, Evaluation)

TextBlob (NLP)

