# Xbot
sentiment analysis bot in python

Here's a README file for your Twitter Sentiment Analysis Bot:

---

# Twitter Sentiment Analysis Bot

This project is a Python-based sentiment analysis tool that fetches tweets from Twitter using the Tweepy library and performs sentiment analysis using TextBlob. The bot can be used to analyze public opinion about a specific topic based on tweets.

## Features

- Fetches tweets related to a specific query from Twitter.
- Performs sentiment analysis on each tweet, classifying them as positive, negative, or neutral.
- Displays the percentage of positive, negative, and neutral tweets.
- Displays the text of the top positive and negative tweets.

## Requirements

- Python 3.x
- [Tweepy](https://www.tweepy.org/) for accessing the Twitter API
- [TextBlob](https://textblob.readthedocs.io/en/dev/) for sentiment analysis
- [Regex](https://docs.python.org/3/library/re.html) for cleaning tweet text

## Setup Instructions

### Step 1: Install Required Libraries

Make sure you have `tweepy` and `textblob` installed in your Python environment. If not, you can install them using pip:

```bash
pip install tweepy textblob
```

### Step 2: Obtain Twitter API Credentials

1. Go to the [Twitter Developer Console](https://developer.twitter.com/en/apps).
2. Create a new app if you haven't already.
3. Obtain the following credentials:
   - **API Key**
   - **API Secret Key**
   - **Access Token**
   - **Access Token Secret**

### Step 3: Update API Credentials

In the script, replace the following placeholders with your actual Twitter API credentials:

```python
consumer_key = 'XXXXXXXXXXXXXXXXXXXXXXXX'
consumer_secret = 'XXXXXXXXXXXXXXXXXXXXXXXXXXXX'
access_token = 'XXXXXXXXXXXXXXXXXXXXXXXXXXXX'
access_token_secret = 'XXXXXXXXXXXXXXXXXXXXXXXXX'
```

### Step 4: Run the Script

Once you have updated the credentials, you can run the script. The bot will fetch the tweets based on the query you specify and perform sentiment analysis. You can change the query in the `main()` function to any topic of your choice (e.g., 'Donald Trump'):

```python
tweets = api.get_tweets(query='Donald Trump', count=200)
```

To run the script, use the following command:

```bash
python xbot.py
```

### Step 5: View the Results

Once the script runs, it will output:
- The percentage of positive, negative, and neutral tweets.
- The top positive tweets.
- The top negative tweets.

## Example Output

```
Positive tweets percentage: 45.5 %
Negative tweets percentage: 32.2 %
Neutral tweets percentage: 22.3 %

Positive tweets:
Tweet 1: This is a great example of positive sentiment!
Tweet 2: I love this topic, it's so amazing!

Negative tweets:
Tweet 1: This is so frustrating, I can't believe it.
Tweet 2: I really dislike this situation.
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to customize it based on your exact needs.
