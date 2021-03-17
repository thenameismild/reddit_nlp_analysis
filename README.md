# Reddit NLP Analysis

Reddit is a collection of online discussion boards known as "subreddits", which cover a variety of topics. The goal of this project is to classify which subreddit a given post came from. 

In this project I will be classifying posts from two subreddits, /r/himym and /r/bigbangtheory. These two subreddits were picked becuase of their similarity in topics and the content in them.  We pulled the data using a for loop through Reddit API.

Due to the popularity of both shows, there are many people who already watched the shows, but also some who have no idea what the shows are about. Through this project I hope to identify keywords to help new viewers identify what keywords to search for more information about the show or to classify which post or information belongs to which shows.

##### Key Terms

- The Big Bang Theory will be refer as BBT or The Big Bang Theory interchangably.
- How I Met Your Mother will be refer as HIMYM or How I Met Your Mother interchangably.

# The Data
|HIMYM Data|Big Bang Theory Data|
|---|---|
|869 reddit posts|1012 reddit posts|
|114 features|114 features|
|Features contain: titles, post text, post name, media links|Features contain: titles, post text, post name, media links|
|Show ran from 2005 to 2014|Show ran from 2007 to 2019|

In both data the features we process to only picked the text data which were contained in the title and post text. From this a new data frame was created with columns consisted of:
- post id
- post subreddit
- post title
- post text

# Data Preprocessing
The HIMYM data and The Big Bang Theory data were join to a dataframe where it consisted of a total of 1881 posts to worked with. 

The data was cleaned by removing url links and non letter words first. Then split the sentence into individual words and tolkenized it. After they were classified to stopwords and removed those and lematized them. Finally they are joined back into a string of words.

# Recommendation
From our findings the recommended words for users to search and learn more about the show on reddit or search engines would be specific chracter names, catchphrase or location names:

|HIMYM Key Words|Big Bang Theory Key Words|
|---|---|
|ted|sheldon|
|robin|penny|
|barney|leonard|
|lily|nobel|
|marshall|amy|
|time|raj|
|bro|smart|
|tracy|bernadette|
|victoria|bazinga|
|stella|comics|
