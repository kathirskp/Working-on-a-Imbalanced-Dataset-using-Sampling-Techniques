Breast_Cancer_Prediction

This repository will show how to work on the unbalanced dataset. This is the first time I am working on such an imbalanced dataset, and I am learning how to deal with such scenarios. 

The dataset is small dataset with 500+ rows and 32 variables. The target variable is "diagnosis" in which 0 - for normal, and 1 - for cancer predicted. The positive class 1 (cancer) accounts less than 5% of the whole dataset

The dataset used is a raw data and not a standardized data. So, I have standardized all the columns and reduced the columns to 10 by creating the Principal components. Principal Components is one the dimension reduction technique used to reduce the dimension of the model (reduce the columns)

Things I've learnt today while working on this problem - If the event to be predicted belongs to a minority class and the event rate is less than 5%, it is referred to as a 'rare event', and this makes the data imbalanced.

Standard ML methods like Logistic Regression and Decision Trees do not work well with imbalanced data. They tend to predict the majority classes better, and treat the minority classes as NOISE. Hence, there is a HIGH probability of Misclassification of the minority class as compared to the majority class.

Accuracy is not the best parameter to measure the performance of the imbalanced data set. Because Accuracy give equal weightage to both 1's and 0's. Recall and Precision score is used for measure the performance of the model. 

Following are the SAMPLING TECHNIQUES used:

RANDOM UNDER-SAMPLING - Randomly Reduces the instances of the MAJORITY class.

RANDOM OVER-SAMPLING - Randomly Increases the instances of the MINORITY class.

Synthetic Minority Over Sampling Technique (SMOTE) - This process creates synthetic samples of the minority class, which are then added to the main dataset. This method prevents over-fitting caused by random sampling as we are using synthetic samples and not randomly replicating the minority classes instances.

Suggestions are welcomed!
