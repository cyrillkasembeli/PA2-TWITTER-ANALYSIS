# PA2-TWITTER-ANALYSIS
we are going to play with Twitter data.

The data is represented as rows of of JSON strings. It consists of tweets, messages, and a small amount of broken data (cannot be parsed as JSON).

we will only focus on tweets and ignore all other messages.

Tweets
A tweet consists of many data fields. Here is an example. You can learn all about them in the Twitter API doc. We are going to briefly introduce only the data fields that will be used in this homework.

created_at: Posted time of this tweet (time zone is included)
id_str: Tweet ID - we recommend using id_str over using id as Tweet IDs, becauase id is an integer and may bring some overflow problems.
text: Tweet content
user: A JSON object for information about the author of the tweet
id_str: User ID
name: User name (may contain spaces)
screen_name: User screen name (no spaces)
retweeted_status: A JSON object for information about the retweeted tweet (i.e. this tweet is not original but retweeteed some other tweet)
All data fields of a tweet except retweeted_status
entities: A JSON object for all entities in this tweet
hashtags: An array for all the hashtags that are mentioned in this tweet
urls: An array for all the URLs that are mentioned in this tweet
Data source
All tweets are collected using the Twitter Streaming API.
