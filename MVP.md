For my MVP I am taking at my accuracy of predicting a hit song.  My target distribution is a concern as the data set is nearly 50-50 (a hit song has appeared on the Billboard top 100 at some point and the song must be in the US market).  Each year around 500-700 songs will make a top 100, while hundreds of thousands of songs will be released.  So for the business case at the end we will want to test an average album to see if we can hit the right distribution of hits or compare a few example songs of flops and hits to see how this algorithm expands to real life case of predicting hit songs so we know who to sign and which songs to promote.

For my dummy classifier in this case we get around 51% accuracy guessing no on all our songs as the flops slightly outweigh the hits.


Using K Nearest Neighbors with ten to start, we perform fairly well on accuracy at around 84% and 81% on the validation set. And looking at our accuracy using the train and validation as one with cross validation it looks like about 10-15 nearest neighbors performs about the best.



![Screen Shot 2021-05-11 at 4 39 38 PM](https://user-images.githubusercontent.com/19785958/117888313-7fce2200-b277-11eb-9ca1-fcf7fdb0abf4.png)

![Screen Shot 2021-05-11 at 4 50 02 PM](https://user-images.githubusercontent.com/19785958/117889320-f91a4480-b278-11eb-8fe1-e0952fcad440.png)


Looking at logistic regression, this data appears to perform similarly at 80% so just slightly below k nearest neighbors (training on training and scoring on validation set with scaled data).  

I will look into trees and gradient booting as my next steps as well as adding dummy genre variables to test out some feature engineering. 

In terms of the final metric I will be looking to optimize for, I will be targeting F1 or F1 Beta with an emphasis on optimizing for recall.  Reason being, a hit song can be worth millions, if not, hundreds of millions in streaming revenues while studio costs can range from as low as 5 to 10K to upwards of a million dollars for a major record label artist.  Given the upside potential could easily outweigh multiple albums worth of busts, my bias is to skew towards hit songs especially because they are more rare than the data set presents.  That said, we can't gamble on a ton of artist studio and marketing costs and bleed by a thousand paper cuts while never getting a hit song to generate royalities and concert revenues. 
