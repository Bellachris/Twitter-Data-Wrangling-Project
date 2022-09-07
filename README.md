# Twitter-Data-Wrangling-Project

**This is the second project in the Udacity/ALX Data Analysis Nanodegree program.**

## Introduction

Real-world data rarely comes clean. Using Python and its libraries, you will gather data from a variety of sources and in a variety of formats, assess its quality and tidiness, then clean it. This is called data wrangling. You will document your wrangling efforts in a Jupyter Notebook, plus showcase them through analyses and visualizations using Python (and its libraries) and/or SQL.

The dataset that you will be wrangling (and analyzing and visualizing) is the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has over 4 million followers and has received international media coverage.

WeRateDogs downloaded their Twitter archive and sent it to Udacity via email exclusively for you to use in this project. This archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017. 

## Project Details

On this project, the task to work on are as follows:

1- Gathering data
2- Assessing data
3- Cleaning data
4- Storing data
5- Analyzing, and visualizing data
6- Reporting on
   data wrangling efforts
   data analyses and visualizations
   
## Gathering the Data for this project
   
Gather each of the three pieces of data as described below in a jupyter Notebook titled wrangle_act.ipynb:
   
1. **twitter_archive_enhanced.csv**: this file was downded manually from the URL provided by Udacity.
   
2. **The tweet image prediction**: This file (image_predictions.tsv) is hosted on Udacity's servers and e downloaded programmatically using the Requests library and the following URL: https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv

3. **Json file Twitter API**: This file will contain each tweet's retweet count and favorite count at minimum, and any additional data you find interesting. using the tweet IDs in the WeRateDogs Twitter archive, query the Twitter API for each tweet's JSON data using Python's Tweepy library and store each tweet's entire set of JSON data in a file called tweet_json.txt file. Each tweet's JSON data should be written to its own line. Then read this .txt filen line by line into a pandas DataFrame with tweetID,retweet count , and favorite count.

## Assessing the Data

After gathering all the three pieces of data, assess them visually and programmatically for quality and tidiness issues. Detect and document at least **eight quality issues** and **two tidiness issues** in the "Accessing Data" section in the wrangle_act.ipynb Jupyter Notebook

## Points to Note

* You only want original ratings (no retweets) that have images. Though there are 5000+ tweets in the dataset, not all are dog ratings and some are retweets.

* Assessing and cleaning the entire dataset completely would require a lot. Therefore, assess and clean at least 8 quality issues and at least 2 tidiness issues in this dataset.

* The fact that the rating numerators are greater than the denominators does not need to be cleaned. This unique rating system is a big part of the popularity of WeRateDogs.

* You do not need to gather the tweets beyond August 1st, 2017. You can, but note that you won't be able to gather the image predictions for these tweets since you don't have access to the algorithm used.

## Cleaning the Data
In the Analyzing and Visualizing Data section in your wrangle_act.ipnb Jupyter Notebook, analyze and visualize your wrangled data

* You must produce at least (3) insights and one (1) visualization.

*You must clearly document the piece of assessed and cleaned data used to make each analysis and visualization.

## Storing, Analyzing and Visualizing Data 

Store the cleaned master DataFrame in a CSV file with the main one named twitter_archive_master.csv. If additional files exist because multiple tables are required for tidiness, name these files appropriately. Additionally, you may store the cleaned data in a SQLite database.

Analyze and visualize your wrangled data in your wrangle_act.ipynb Jupyter Notebook to produce at least three (3) insights and one (1) visualization.

## Reporting the project

Create a 300-600 word written report called wrangle_report.pdf or wrangle_report.html that briefly describes your wrangling efforts. This is to be framed as an internal document.

Create a 250-word-minimum written report called act_report.pdf or act_report.html that communicates all the insights and displays the visualization(s) produced from your wrangled data. This is to be framed as an external document, like a blog post or magazine article, for example.
