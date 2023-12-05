This file contains HW9, which is on the CART method; particularly on implementations of the Random Forest (RF) and Gradient Boosted Tree (GBT) Classifiers and Regressors. For this homework, I worked in a group with Sarah, Paula, and Masooma. We all did the work in each individual notebooks, but we especially had discussions on different ways to run the model. 
First, it was mainly about how to deal with the missing values in the data (I explained some of our different approaches in the notebook). I was initially still leaving the missing data and using Imputer, but then that would be contradictory to our main goal of dealing with the NaN values as it distorts the data, so I ended up removing the NaN values the way I describe in the notebook. In running the RF and GBT classifiers, I followed along with the skeleton while looking at examples/documentation. I also had to take note that because the classifiers were predicting labels, I had to "encode" the "s" and "b" labels (into binary-like form) before running it through the forest classifier methods. 

I was also having trouble with the forest classifiers because when I printed the score, I always got 1.0. After discussion with teammates, I realized I need to specify parameters especially max_depth as this really influences the tree method. I also ended up using accuracy_score() instead of classifier.score(), as Sarah suggested, as I kept on getting 1.0 with the latter. (I also needed to remind myself that I need to print a score for each train (vs prediction) and test (vs prediction) in order to evaluate the model, whether it is good or overfitting etc.) I also realized from my teammates that I needed to drop "Weights" from the feature matrix X, which gave me better comparisons. 

The Regressor process was quite similar; I followed the skeleton code and the documentations. Though, I was a bit confused about calculating the score. Then, Paula pointed out that that was the reason why we're calculating L1 and L2, and we can evaluate the scores/performance for regression.

For the next parts, I followed the skeleton again, but looked more into the concepts, and learnt some things that I listed as notes for myself in the notebook. Some of them were about hyperparameter tuning, finding best parameters for our forest model. I also realized I had to revert how I order the rf.feature_importances_ and the corresponding argsort() function, because on its own, it orders from the smallest importance (Masooma helped with this). Tali and Paula pointed out to us about the possibility of finding the "best parameters" using only our selected "most important" features, which I think is worth exploring. Moreover, I learnt a bit about the ROC curve, and thought about ways to interpret it in our context. 


Important note: 

Re-running the model again, I realized after a specific run that the best parameters was different than what I usually had. I was very worried about that, but when I re-ran the model, I had what I previously had again. So my analysis and captions from that part onwards is based on the specific "best parameters" of max_depth = 10, "auto", and n_estimators = 100. I just wanted to explicitly specify that here just in case it changes again for any reason.

My intuition about this tells me that the changes when I run, if not because of the possibility of me accidentally changing some parameters on the way, might be because of the fact that we are dealing with the RF CART method. The random forest is itself designed to introduce randomness to the modelling process, hence I remember in class that this method could be different every time we run it. 

Update note:

I realized I had to set a random seed, which I completely missed. So I think that was the issue.  






