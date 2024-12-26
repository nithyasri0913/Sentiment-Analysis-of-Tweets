# Twitter Sentiment Analysis

This project is a sentiment analysis application that uses Tweepy and TextBlob to fetch and analyze tweets for their sentiment (positive, neutral, or negative).

## Features
- Authenticates with the Twitter API using OAuth.
- Fetches tweets based on a search query.
- Cleans tweets by removing links, mentions, and special characters.
- Classifies tweets as positive, neutral, or negative using TextBlob's sentiment analysis.
- Calculates and displays the percentage of positive, neutral, and negative tweets.
- Displays sample tweets for each sentiment category.

## Requirements
To run this project, you'll need the following Python packages:
- `tweepy`: For fetching tweets from the Twitter API.
- `textblob`: For sentiment analysis.
- `re`: For cleaning tweet text.
- `nltk`: For TextBlob's dependency.

## Installation
1. Clone the repository or download the script.
2. Install the required packages:
   ```bash
   pip install textblob tweepy
   ```
3. Download NLTK corpora for TextBlob:
   ```bash
   python -m textblob.download_corpora
   ```

## Setup
1. Obtain your Twitter Developer credentials from the [Twitter Developer Portal](https://developer.twitter.com/):
   - Consumer Key
   - Consumer Secret
   - Access Token
   - Access Token Secret
2. Replace the placeholder values in the script:
   ```python
   consumer_key = ''
   consumer_secret = ''
   access_token = ''
   access_token_secret = ''
   ```

## Usage
1. Run the script:
   ```bash
   python twitter_sentiment_analysis.py
   ```
2. Enter a search query (e.g., `Iran`) and specify the number of tweets to fetch (default is 200).
3. The script will:
   - Display the percentage of positive, neutral, and negative tweets.
   - Print the first 10 positive and 10 negative tweets.

## Notes
- The script limits fetched tweets to a default count of 200. You can adjust this in the `get_tweets` function.
- Ensure your Twitter Developer account is approved to access the API.

## License
This project is open-source and available for use under the MIT License.
