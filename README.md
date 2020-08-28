# WeRateDog Twitter Analysis
In this project, we will be wrangling WeRateDogs Twitter data to create interesting and trustworthy analyses and visualizations.

Real-world data rarely comes clean. Using Python and its libraries, we gathered data from a variety of sources and in a variety of formats, assess its quality and tidiness, then clean it. After that, we showcase them through analyses and visualizations using Python (and its libraries) and SQL.

WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has over 4 million followers and has received international media coverage.

![Image of dogs](https://video.udacity-data.com/topher/2017/October/59dd378f_dog-rates-social/dog-rates-social.jpg)

1. Data Gathering

The raw data was collected from three different sources using various techniques.
- WeRateDogs Twitter archive: Download this file manually and load the data with pandas.
- Tweet image predictions: The breed of dog is present in each tweet according to a neural network. This file is
hosted on a server. We downloaded programmatically using the Requests library and the URL provided in tis
project.
- Data scraped from Twitter API: Query the Twitter API for each tweet's JSON data using Python's Tweepy library
and store each tweet's entire set of JSON data in a file called tweet_json.txt file. Then we read this .txt file line by line into a pandas DataFrame with tweet ID, retweet count, favorite count, and follower counts.
After collected the data, load them with pandas read_csv into three separate data frame: twitter_archieve, image_predictions, tweet_api.


2. Data Assessment and Cleaning

Data was assessed manually and programmatically for both quality and tidiness issues in this session. The quality of data is assessed against four criteria: completeness, validity, accuracy, and consistency. Data tidiness is a structural issue. According to the regulations by Hadley Wikham, a tidy dataset is defined as 1. Each variable forms a column. 2. Each observation forms a row. 3. Each type of observational unit forms a table.
