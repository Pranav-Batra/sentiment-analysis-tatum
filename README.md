# Jayson Tatum Sentiment Analysis
Jayson Tatum is weirdly a polarizing star in the NBA, with many proclaiming him as a top 3-5 player in the league while others call him overrated and a product of the team surrounding him. This project was done to see what the general public's opinion was on Jayson Tatum after his championship and subsequent Olympics performances.

# Description

## Scraping Data
To start this project, I had to gather comments related to Jayson Tatum. I chose r/NBA as my source as it is arguably the largest connected community of NBA fans on the internet. From there, I used the PRAW API to scrape ~1000 comments that mentioned Tatum in some way. Along with these comments, I tracked the amount of upvotes/likes they got as well.

## Getting Sentiments
To get the sentiment of each comment, I used a pretrained sentiment analysis classifier model from HuggingFace. I also used their tokenizer, and combined these two to give each comment a sentiment that was either "positive", "negative", or "neutral".

## Data Analysis
After gathering sentiments on each comment, I used visualization libraries to look at what the public opinion was surrounding Tatum. I found that the majority of comments about Tatum were either negative or neutral within the past month, with positive comments lagging behind. Using the nltk and WordCloud libraries, I found that comments with negative sentiments were full of derogatory language and curse words, while positively labeled comments seemed to compliment other players over Tatum, which implies that the share of negative comments might have been even higher. Overall, the amount of upvotes on positive vs. negative comments seemed to be fairly similar, but the most popular comments were by far negative.
