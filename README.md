Reddit Stock Sentiment Analysis and Stock Movement Prediction

Overview
This project focuses on predicting stock price movements by analyzing sentiment from Reddit posts. It uses Natural Language Processing (NLP) to extract insights from user-generated content in stock-related subreddits. The pipeline involves scraping data, performing sentiment analysis, and training a machine learning model to forecast stock trends.


Features
Data Scraping:
Collects posts from subreddits like r/stocks or r/investing.
Extracts relevant features such as post titles, content, engagement metrics (upvotes, comments), and timestamps.
Data Preprocessing:
Removes noise, duplicates, and missing values from the scraped data.
Sentiment Analysis:
Calculates sentiment polarity (positive, neutral, or negative) for each post.
Prediction Model:
Builds a machine learning model to predict stock movements based on sentiment and engagement metrics.
Evaluation:
Provides performance metrics like accuracy, precision, and recall to assess the model's predictive capabilities.


Installation
Prerequisites
Ensure you have the following installed:

Python >= 3.8
Jupyter Notebook
Dependencies
Install the required Python libraries using the command:
!pip install praw pandas textblob scikit-learn matplotlib

Reddit API Setup
Go to Reddit Apps and create a new app:
App Name: (e.g., StockSentimentProject).
App Type: Script.
Redirect URI: http://localhost:8080.
Copy the client_id, client_secret, and user_agent provided by Reddit.
Update these credentials in the reddit.ipynb notebook under the PRAW configuration section.


Usage Instructions
Step 1: Run the Notebook
Open the reddit.ipynb Jupyter notebook.
Follow the steps in order:
Data Scraping: Scrape Reddit posts and save them as reddit_data.csv.
Data Preprocessing: Clean the scraped data and save it as cleaned_reddit_data.csv.
Sentiment Analysis: Perform sentiment analysis and save results as sentiment_reddit_data.csv.
Model Training and Evaluation: Train a machine learning model and evaluate its performance.
Expected Outputs
Scraped Data: reddit_data.csv (Raw data from Reddit).
Cleaned Data: cleaned_reddit_data.csv (Processed and noise-free data).
Sentiment Analysis Results: sentiment_reddit_data.csv (Data with sentiment polarity and labels).
Model Evaluation Metrics: Printed metrics in the notebook, including:
Accuracy
Precision
Recall
F1-Score
Files and Project Structure
Reddit_Stock_Sentiment_Project/
│
├── reddit.ipynb              
├── reddit_data.csv           
├── cleaned_reddit_data.csv   
├── sentiment_reddit_data.csv 
├── README.md                 
Results
Insights:
Sentiment distribution: Percentages of positive, negative, and neutral posts.
Engagement metrics: Average score, comments, and popularity of stock-related posts.
Model Performance:
Evaluation metrics (Accuracy, Precision, Recall, F1-Score).
Model performance trends based on sentiment-based features.
Future Work
Incorporate data from multiple subreddits for diverse insights.
Combine Reddit sentiment with other sources (e.g., Twitter or news websites).
Optimize the machine learning model using advanced techniques like deep learning.
Credits
Developed by: [Sai Krishnavi]
Tools Used: Python, PRAW, TextBlob, scikit-learn, pandas, matplotlib.
