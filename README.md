# Credit Risk Analysis

## Purpose

In this analysis, we are identifying potential Credit Risks based on a given data set, and training a model to predict whether or not a new applicant would be high-risk, or low-risk. This is achieved using Pandas, Imbalanced Learn, and SciKit Learn on Python.

## Results

# For Random Over-Sampling:

![Random Oversampling](https://i.imgur.com/zxVZGPR.png)

Our accuracy is 64.7%.
High-Risk is around 1% Precision, and a 62% sensitivity.
Low-Risk is at 100% Precision due to out-numbering High-Risk, with a 67% sensitivity rating.

# For SMOTE Over-Sampling:

![SMOTE Oversampling](https://i.imgur.com/IvjFy5S.png)

Our accuracy is 62.5%.
High-Risk is around 1% Precision, and a 62% sensitivity.
Low-Risk is at 100% Precision due to out-populating High-Risk, with a 63% sensitivity rating.

# For Under-Sampling:

![Undersampling](https://i.imgur.com/cyU6S3j.png)

Our accuracy is 51.2%.
High-Risk is around 1% Precision, and a 57% sensitivity rating.
Low-Risk is at 100% Precision due to out-populating High-Risk still, with a 45% sensitivity rating due to false-positives.

# For SMOTEENN:

![SMOTEENN](https://i.imgur.com/xVhZBRT.png)

Our accuracy is 61.9%.
High-Risk is around 1% Precision, and a 69% sensitivity rating.
Low-Risk is at 100% Precision, again because of out-populating High-Risk, and a sensitivity rating of 55%, caused by false-positives.

# For Balanced Random Forest:

![BRFC](https://i.imgur.com/qwyQoh6.png)

Our accuracy is 78.8%.
High-Risk is around 4% Precision, and a 67% sensitivity rating.
Low-Risk continues to stay at 100% Precision, with a 91% sensitivity rating, indicating a lower number of false-positives.

# For AdaBoost:

![AdaBoost](https://i.imgur.com/1G0VoYW.png)

Our accuracy is 92.5%.
High-Risk is around 7% Precision, and a 91% sensitivity rating.
Low-Risk still is at 100% Precision, and a 94% sensitivity rating.
Take note of the F1 rating for this report for High-Risk, as it is the highest of all of our previous models.
This should have an overall lower number of false-positives.

## Summary

All of the models do not have the best precision in determining whether a credit risk is high. The most improvement we saw was when the Ensemble Models were used, greatly improving the overall scores seen, and is the best of all the models we have tried.

The AdaBoost model seems to be the best use case for detecting high risk, though there are low risk credits being detected as high risk, which more than likely does not work in the banks favor too much by missing opportunities.

If a model absolutely needed to be chosen, and they were okay with the missed opportunities, then using the AdaBoost model is certainly the way to go, in example for a high-end credit account. But, it may not be worth using any of these models for assessing whether an applicant is high-risk or not.
