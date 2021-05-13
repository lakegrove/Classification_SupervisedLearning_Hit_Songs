# Creating Song Rankings to Predict Hit Songs
Jonathan Wyatt

## Abstract
The goal of this project was to use classification models to predict what song features best predict what makes a great song and therefore a hit song. I worked with data provided in a [Spotify Kaggle Datset](https://www.kaggle.com/theoverman/the-spotify-hit-predictor-dataset), including a separate data with [artist genre information](https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-160k-tracks?select=tracks.csv), leveraging musical and categorical feature engineering inside of an XGBoost model to achieve a strong hit predicting model. After building the model, I utilized the Spotify API to pull in the Billboard top 100 hits for the week and an album to try and predicting the ranking of success of songs and the exoected number of hits. 

## Design
This project was designed to use the Spotify Dataset features with labeled target values of 0 for "Flop" and 1 for "Hit".  The goal of this exercise is to help labels and artists figure out which song are most likely to be successful and therefore be used as things like the first single of the album for promotion or finding which artist to sign based on likelihood of success.  

With the US music industry worth $12 billion in revenue last year and the top 100 streamed songs worth nealry $450 million alone, its as lucrative as ever to find the next great song that we all can't stop singing. 

## Data
The main dataset contains 41,000 plus songs with 15 features for each, with things like danceability, tempo and valence (happy or sad) as features directly from Spotify.  This data set includes a target label based on if the song spent time in the Billboard Top 100 at anytime and had a feature distribution of nealry 50-50 between "Flop" and "Hit"

I also engineered a grene classification using a second kaggle dataset using a word search feature to classify buckets of genre an artist falls into as labeled by Spotify. I also created a feature in an attempt to measure brand value factor on hits, by including previous hits by an artist as a running tally of the number of times they've been featured in the Billboard Top 100 previously


## Algorithms

*Feature Engineering*
1. Converting categorical features to binary dummy variables for Genre
3. Create Previous Artist Song Success

*Models*
  
Logistic regression, k-nearest neighbors, random forest, Naive Bayes, Voting Classifier and XG Boost were used before settling on XG Boost as the model with strongest performance. 

*Model Evaluation and Selection*
  
The entire training dataset of 41,000 records was split into 80/20 train/validation vs. holdout.  The scores shown below reflect the AUC ROC for the train vs validation set and the test model based on a refit mode with train and validation together.

The official metric for this project ROC AUC for the ranking; however but accuracy of predicting a hit song was also watched closely throughout the analysis.

**Final Gradient Boosts:** 23 features 
   - Accuracy 0.921
   - AUC ROC .977

**Holdout** 
   - Accuracy 0.917
   - AUC ROC .976

## Tools
- Numpy and Pandas for data manipulation
- Scikit-learn for modeling
- Matplotlib and Seaborn for plotting


## Communication
The Slides for this analysis are included in this repo with further work to be done, so stay tuned. 
