# 🛒 Flipkart Review Sentiment Analysis (VADER NLP)

## 📌 Overview
This project performs sentiment analysis on Flipkart product reviews using the VADER (Valence Aware Dictionary and sEntiment Reasoner) model from NLTK.

It analyzes customer reviews and classifies them into:
- Positive
- Negative
- Neutral

The project also provides visual insights using charts and allows users to analyze custom reviews interactively.

## 🚀 Features
- Load and clean Flipkart review dataset
- Rating distribution visualization (Pie Chart)
- Sentiment analysis using VADER
- Sentiment distribution visualization (Bar Chart)
- Aggregated sentiment score analysis
- Real-time sentiment prediction for user input

## 🧠 How It Works

### 1. Data Loading
- Reads dataset using Pandas
- Removes missing values

### 2. Sentiment Analysis
- Uses NLTK’s VADER SentimentIntensityAnalyzer
- Extracts:
  - Positive score
  - Negative score
  - Neutral score
  - Compound score

### 3. Classification Logic
Compound ≥ 0.05 → Positive  
Compound ≤ -0.05 → Negative  
Else → Neutral  

### 4. Visualization
- Pie chart for rating distribution
- Bar chart for sentiment distribution

## 📂 Dataset
The dataset should be in CSV format and contain:
- Review → Text reviews
- Rating → Numerical ratings

Update dataset path in the code:
df = load_and_clean_data('path_to_your_dataset.csv')

## ⚙️ Technologies Used
- Python
- Pandas
- Matplotlib
- NLTK (VADER)
- Jupyter Notebook / Python Script

## 📊 Output
- Rating distribution chart
- Sentiment distribution chart
- Sentiment score summary:
  - Total Positive Score
  - Total Negative Score
  - Total Neutral Score
- Real-time sentiment prediction for custom input

## ▶️ How to Run

Step 1: Clone Repository
git clone https://github.com/your-username/flipkart-sentiment-analysis.git
cd flipkart-sentiment-analysis

Step 2: Install Dependencies
pip install pandas matplotlib nltk

Step 3: Run the Script
python sentiment_analysis.py

## 📦 Requirements
Download VADER lexicon before running:
import nltk
nltk.download('vader_lexicon')

## ⚠️ Important Note
Fix this line in your code before running:

Incorrect:
if _name_ == "_main_":

Correct:
if __name__ == "__main__":

## 📈 Use Cases
- Analyze customer reviews
- Understand product feedback
- Improve business decision-making

## 🔮 Future Improvements
- Add Machine Learning models (Naive Bayes, Logistic Regression)
- Use Deep Learning models (LSTM, BERT)
- Deploy as a web application (Flask/Streamlit)
- Real-time Flipkart data scraping

## 👤 Author
Your Name

## 📜 License
This project is open-source and available under the MIT License.
