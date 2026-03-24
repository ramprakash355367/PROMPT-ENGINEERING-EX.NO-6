# Ex.No.6 Development of Python Code Compatible with Multiple AI Tools

# Aim: 
    To Development of Python code compatible with multiple AI Tools Slots

# Python Code: 

from nltk.sentiment import SentimentIntensityAnalyzer
import nltk

nltk.download('vader_lexicon')

#Simulated AI-generated text
generated_text = input()

print("Generated Review:\n")
print(generated_text)

#Sentiment analysis
sia = SentimentIntensityAnalyzer()
sentiment = sia.polarity_scores(generated_text)

print("\nSentiment Analysis:")
print(sentiment)

#Insight generation
if sentiment['compound'] > 0:
    print("\nInsight: The review is positive and suitable for marketing promotion.")
else:
    print("\nInsight: The review tone is neutral or negative.")
    
# Input 1: 

This smartphone offers outstanding battery life and an intelligent AI camera that captures stunning photos.

# Output 1:

This smartphone offers outstanding battery life and an intelligent AI camera that captures  stunning photos. 
Generated Review:
This smartphone offers outstanding battery life and an intelligent AI camera that captures  stunning photos. 

Sentiment Analysis:
{'neg': 0.0, 'neu': 0.556, 'pos': 0.444, 'compound': 0.8625}
Insight: The review is positive and suitable for marketing promotion.

# Input 2: 

This smartphone struggles with battery life and often needs frequent charging. The so
called AI camera fails to deliver consistent results, producing dull and unimpressive 
photos.

# Output 2:

This smartphone struggles with battery life and often needs frequent charging. The so called AI camera fails to deliver consistent results, producing dull and unimpressive  photos. 
Generated Review:
This smartphone struggles with battery life and often needs frequent charging. The so called AI camera fails to deliver consistent results, producing dull and unimpressive  photos. 
Sentiment Analysis:
{'neg': 0.321, 'neu': 0.679, 'pos': 0.0, 'compound': -0.8555}
Insight: The review tone is neutral or negative.

# Result: 
      Thus the Development of Python code compatible with multiple AI Tools Slots is verified and given.
