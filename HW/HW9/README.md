This file contains HW9, which is on the CART method; particularly on implementations of the Random Forest (RF) and Gradient Boosted Tree (GBT) Classifiers and Regressors. For this homework, I worked in a group with Sarah, Paula, and Masooma. We all did the work in each individual notebooks, but we especially had discussions on different ways to run the model. 
First, it was mainly about how to deal with the missing values in the data (I explained some of our different approaches in the notebook). I was initially still leaving the missing data and using Imputer, but then that would be contradictory to our main goal of dealing with the NaN values as it distorts the data, so I ended up removing the NaN values the way I describe in the notebook. In running the RF and GBT classifiers, I followed along with the skeleton while looking at examples/documentation. I also had to take note that because the classifiers were predicting labels, I had to "encode" the "s" and "b" labels (into binary-like form) before running it through the forest classifier methods. 

I was also having trouble with the forest classifiers because when I printed the score, I always got 1.0. After discussion with teammates, I realized I need to specify parameters especially max_depth as this really influences the tree method. I also ended up using accuracy_score() instead of classifier.score() as I kept on getting 1.0 with the latter. (I also needed to remind myself that I need to print a score for each train (vs prediction) and test (vs prediction) in order to evaluate the model, whether it is good or overfitting etc.) I also realized from my teammates that I needed to drop "Weights" from the feature matrix X, which gave me better comparisons. 

The Regressor process was quite similar; I followed the skeleton code and the documentations. Though, I was a bit confused about calculating the score. Then, Paula pointed out that that was the reason why we're calculating L1 and L2, and we can evaluate the scores/performance for regression.






