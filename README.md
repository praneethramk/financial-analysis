Financial News Sentiment Analysis
Overview
This project is a Python-based tool for scraping financial news articles from the Livemint website and performing sentiment analysis on the collected articles. The tool identifies the most positive and negative articles based on sentiment scores and provides a summary.

Features
Scrapes financial news articles from various sections of Livemint.
Performs sentiment analysis on the collected articles using the NLTK library.
Identifies and displays the most positive and negative articles.
Provides a user-friendly interface to run the sentiment analysis repeatedly.
Tech Stack
Programming Language: Python
Libraries/Frameworks:
requests for making HTTP requests.
BeautifulSoup (from bs4) for HTML parsing.
re and string for text processing.
textwrap for wrapping text.
nltk.sentiment for sentiment analysis.
Sentiment Analysis Tool: SentimentIntensityAnalyzer from nltk
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/financial-news-sentiment-analysis.git
cd financial-news-sentiment-analysis
Install the required libraries:

bash
Copy code
pip install requests beautifulsoup4 nltk
Download NLTK data:

python
Copy code
import nltk
nltk.download('vader_lexicon')
Usage
Run the script:

bash
Copy code
python financial_news_sentiment_analysis.py
The script will scrape financial news articles from Livemint and perform sentiment analysis.

The most positive and negative articles will be displayed with their sentiment scores and links.

You can choose to run the analysis again by following the prompt.

Code Explanation
The script performs the following steps:

Imports the necessary libraries.
Defines the URLs for different sections of Livemint.
Scrapes the articles from the specified sections and collects the links.
Processes each link to extract the article content.
Performs sentiment analysis on the extracted content.
Sorts the articles based on their sentiment scores.
Displays the most positive and negative articles.
Provides an option to run the analysis again.
