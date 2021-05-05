# Metis Music Label


#### Question/need:
* The purpose of my model will be to use Spotify features to figure out what characterisitcs make up a hit song.  A hit song will be defined by time spent on the weekly 100 billboard chart.  Given the nature of music and what constitutes a hit is always changing, we will break up the data by decade.  This way we can see if we can predict what makes a hit song during a particular time frame as well as the features most common among those songs that are hits in the same time frame.

By identifying good song features we can sell this information to producers looking for the next best thing and whats hot or even to producers looking to blend in success from a particular time period into new music releases today. As music tastes are all over the spectrum with many, for example calling the sixties and seventies the best time for music while many in the younger crowd preferring the styles of the current day. 

Metis Music label can then figure out what type of artists to go out and sign depending on which type of music characteristics fit with that artist and target audience they want to pursue to make a successful label. 

#### Data Description:
* For this I will be using Kaggle data assmebled from the past five decades in combination with a target variable of 0 or 1 if that song for that artist appeared in the weekly top 100 at that time. There are roughly 5,000 to 7,000 songs per decade.  

* I expect to work with things like spotify's own meaures of Danceability, Energy, Key, Loudness, Speechiness, Acoustiness, Instrumnetalness and others.  

* The target will be whether the song is a hit or not.  We may also be interetsed in identifying genres so we can figure out who belongs to what genre so we have a balanced line up. 

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


#### MVP Goal:
* Ideas for a minimum viable product might as simple as comparing, showing or ranking the feature importance for a particular decade and an example song that scores well along those items that is in fact a hit (as well as one that was a "miss")
