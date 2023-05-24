# Twitter-sentiment-analysis-MSterczewski
Project that analyses tweets in order to detect their sentiment

# 1. The aim
The aim of this project was to collect tweets about a specific topic and then perform sentiment analysis on them in order to create a tweet sentiment prediction model.<br />
The project was conducted as a grading project for ZUM subject on PJATK.

# 2. The data
Original data was supposed to be scraped from Twitter using Twitter API with academic access. Unfortunately, due to changes in Twitter policy, it was no longer possible to scrape tweets using free version of Twitter API and application for academic access was denied. <br />
Tweets were supposed to be gathered using Tweepy, and they should be about a specific topic, preferably a controversial one. My idea was to gather tweets about Elon Musk. <br />
Instead of scraping the tweets myself, I used a prepared dataset from the web. The dataset contains unprepared and uncleaned tweets. It also contains sentiment labels, but only the text is loaded into memory.

# 3. How to use the project
In order to start the project, few steps should be performed:
1. You should open jupyter notebook and open .ipynb file
2. You should upload tweets.csv file into runtime memory
3. You should login to wandb (or create an account) and pass the auth code when asked by the program.

# 4. Uploaded files
The project structure (on github) contains files:
1. part3.model - best neural model achieved in Etap 3
2. part4.model - model based on BERT. Unfortunately, the model itself was too large for upload (260MB) even after compression.
3. saved_files.png - a file structure on jupyter notebook to show that the part4 model was saved on the disk.
4. wandb.png - a wandb report on the 16 fine tuned runs of part3 model.

The analysis of wandb.png file shows that lowering learning rate from 0.01 to 0.001 made the biggest impact on the accuracy of the model.
