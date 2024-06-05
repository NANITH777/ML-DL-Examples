# COVID-19 Vaccine Sentiment Analysis

## Overview

This project aims to analyze sentiments expressed in tweets about the COVID-19 vaccine. The analysis includes preprocessing the data, performing sentiment analysis, and visualizing the results. The focus is on identifying the most positive and negative sentiments and exploring the common words used in these tweets.

## Project Structure

- **Data Loading**: Import and read the dataset containing tweets about the COVID-19 vaccine.
- **Data Preprocessing**: Clean the data by removing unnecessary elements like Twitter handles, hashtags, URLs, special characters, and extra spaces.
- **Sentiment Analysis**: Use NLTK's VADER Sentiment Intensity Analyzer to compute sentiment scores (positive, neutral, and negative) for each tweet.
- **Visualization**: Generate plots and word clouds to visualize the distribution of sentiments and the most common words in positive and negative tweets.

## Files

- **`vaccination_tweets.csv`**: The dataset containing tweets about the COVID-19 vaccine.
- **`README.md`**: This file, providing an overview and instructions for the project.

## Results

The analysis results include:

- **Sentiment Distribution**: KDE plots showing the distribution of positive, neutral, and negative sentiments across the tweets.
- **CDF of Sentiments**: Cumulative distribution functions for the sentiment scores.
- **Word Clouds**: Visual representations of the most common words in the most positive and negative tweets.
- **Top Words**: Lists of the top 10 words in the most positive and negative tweets.

## Conclusion

This project provides insights into public sentiments about the COVID-19 vaccine by analyzing tweets. The sentiment analysis helps understand the general perception and the common topics discussed in relation to the vaccine.