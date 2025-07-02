# Sentiment_analyzer

Sentiment Analysis Module

This module performs sentiment analysis on social media posts and news articles related to cryptocurrencies. It is designed to be part of a broader AI trading assistant, providing insight into public perception and market sentiment for any crypto asset.

Features

Text Preprocessing: Cleans raw text by removing URLs, mentions, hashtags, emojis, numbers, and special characters to prepare it for sentiment analysis.

Sentiment Scoring: Uses the textblob to classify text into positive, negative, or neutral sentiment.

Batch Analysis: Processes multiple posts or headlines and returns detailed sentiment breakdowns.

Timestamp Assignment: Assigns the current timestamp to each analyzed item for time-based tracking.

Customizable Inputs: Accepts structured input data including text, source (e.g. Twitter or Reddit), and asset name.


Input Format

Each item to be analyzed should be a dictionary with the following fields:

"text": The raw social media post or article content.

"source": The platform (e.g., "Twitter", "Reddit", "News").

"asset": The related cryptocurrency (e.g., "Bitcoin", "ETH").


Output

The output is a list of dictionaries, where each item includes:

The original cleaned text

Source and asset metadata

Sentiment classification (Positive, Negative, or Neutral)

Sentiment confidence score (compound VADER score)

Timestamp of analysis


Integration

This module is designed to be used with other components of the trading assistant, such as:

Social media scrapers

News aggregators

Data storage systems

Signal fusion engines (for combining sentiment with technical indicators)


It can be integrated into pipelines where sentiment influences trade signals or anomaly detection.

Requirements

Python 3.8 or higher

textblob

re, datetime (standard libraries)


File Location and Dependencies

File path: cryptsignal/sentiment_analysis.py

No external modules are required beyond standard libraries and nltk.


License

This module is distributed under the MIT License. You are free to use, modify, and distribute it with attribution.

Author

Part of a full-stack AI trading assistant system developed by Chukwujiekwu Collins Ifedi 

