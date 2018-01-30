# Amazon-Food-Reviews-Analysis
## Making predictions over amazon recommendation dataset Predictions

The purpose of this analysis is to make up a prediction model where we will be able to predict whether a recommendation is positive or negative. In this analysis, we will not focus on the Score, but only the positive/negative sentiment of the recommendation.
To do so, we will work on Amazon's recommendation dataset, we will build a Term-doc incidence matrix using term frequency and inverse document frequency ponderation. When the data is ready, we will load it into predicitve algorithms, mainly naïve Bayesian and regression.
In the end, we hope to find a "best" model for predicting the recommendation's sentiment.

## Loading the data
In order to load the data, we will use the EXCEL dataset where we will only fetch the Score and the recommendation summary.
As we only want to get the global sentiment of the recommendations (positive or negative), we will purposefully ignore all Scores equal to 3. If the score id above 3, then the recommendation wil be set to "postive". Otherwise, it will be set to "negative".
The data will be split into an training set and a test set with a test set ratio of 0.2
