# Metis Music Label


#### Question/need:
* The purpose of my model will be to use Spotify features to figure out what characterisitcs make up a hit song.  A hit song will be defined by time spent on the weekly 100 billboard chart.  While we are interested in accuracy in general to predict if a song is a hit or not, we will focus our target on ROC AUC as a measure creating soft probabilities to allow for rankings of songs.

The goal of this is to help producers or record labels get feedback from our models to emphasize what songs on an album make sense to be a debut or perhaps an artist to sign because the model is predicting a song with particular features to outperform others. 

Ideally, here at Metis Music label we will beat them all to the punch and start the best record label around.

#### Data Description:
* For this I will be using Kaggle data assmebled via the Spotify API from the past five decades in combination with a target variable of 0 or 1 if that song for that artist appeared in the weekly top 100 at that time. There are roughly 5,000 to 7,000 songs per decade.  

* I expect to work with things like spotify's own meaures of Danceability, Energy, Key, Loudness, Speechiness, Acoustiness, Instrumnetalness and others.  

* The target will be whether the song is a hit or not.  We may also be interetsed in identifying genres so we can figure out who belongs to what genre so we have a balanced line up. 

* At the end I hope to use the Billboard API to identify this week's Top 100 to see how our rankings compare with Billboard.  To do this we will use the Spotify API and compare the two and how well they correlate in ranking muisc.  Additionally we will look at an album by Kendrick Lamar to see how well the algorithm compares with the relative success of the songs on that album.


#### Tools:
Logistics Regression

KNN

Trees

Gradient Boost

Python

Spotify API

Tableau

Excel

Matplotlib

Seaborn
