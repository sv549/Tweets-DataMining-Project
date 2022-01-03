# Tweets-DataSet-Project
Using RAPIDMINER, took an excel data set regarding Tweets/Retweets from Former Presidents. Used a few machine learning algorithms 

There were a few algorithms used in this project to determine/figure out a relationship between the tweets and retweets in our data set. 

**K Nearest Neighbors**

Using the K nearest neighbors algorithm, setting the value for K to 7 changed up the results slightly. The reason for choosing 7 instead of a number lower than 5 was due to the fact that there could be an error in the measurement. There were 496 True Positives that came up in this process compared to the 479 from the K=5 process. The 496 Positives for Trump’s retweets seems to be a bit off the actual number that is portrayed by the data along with 547 non retweets being 2 numbers off the actual number of non retweets. 
	The accuracy of the model is at a staggering 69.53% which can lead us to believe that setting the value at K=7 helped us analyze the proper amount of Positives that come out of this test. The class recall comes in at 72.73% which shows us how precise the model is for a positive case. The FPR in the study comes out to be about 28%. Using K=7 showed us a study with a higher accuracy compared to that of K=5.  


**Decision Trees**

The decision tree with depth ten leads to the interpretation that “realdonaldtrump” which is the root is the key variable that determines whether a tweet was a retweet from another user. When the first level variable is < 0.055 thresholds, the next component added to the decision is the word “great” which appears on the second level. On the third level, the words “congressman” and “economic” are added to the decision path. 

The confusion matrix indicates that 2672 retweets were predicted to be retweets(TP), while 54 retweets were predicted to be not retweets(FN). In other words, the recall score for this algorithm is 98.02% which is an indicator that this algorithm is good in that regard. 
Recall = TP/(TP+FN)

However, the confusion matrix also indicates that 1501 that is not retweeted were predicted to be retweets(FP). This gives our algorithm a precision of 64.03%.
Precision = TP/(TP+FP)

Lastly, when observing the area under the curve(AUC), we get a value of 0.713 which suggests the algorithm performed fairly. 

**What does the finding tell you? Can you take action to improve the performance and solve a problem based on the findings? Do you have any recommended action?**

“Realdonaldtrump” is the most important attribute in predicting whether it was a retweet or not.
Donald Trump likes to support those that tweet about him, by retweeting that user’s tweet.
Most commonly used words for Donald Trump other than his twitter handle (in order)
Great, people, president, new, thank, state, trump, Biden, job, and fake.

 To improve the results of our text mining the first step would be to mine more data records.  Our original file of tweets had 56,000 records, which was too much for our computers to handle.  Due to this issue we chose a subset of 5,000 records.  With more records our models would have more data to be trained on, resulting in more complete analysis and accurate results.  Another nuisance we ran into were emojis, which affected approximately 5% of our training data.  Although this did not make or break our results, it would make the process of mining the data clearer.  These improvements would create a more complete model which would be more reliable in solving our problem of predicted Donald Trump's tweets vs retweets.

