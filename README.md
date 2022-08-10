# Credit_Risk_Analysis

### Overview of the Analysis:
Credit risk can be a problem within the process of loan applications. Through the use of data given from "LendingClub", this analysis uses several types of algorithms to calculate credit. Through the use of RandomOverSampler, SMOTE, and ClusterCentroids, followed by the SMOTEEN algorithm. Finally we use machine models to predict accurate credit risk in order to set a reccomendation for potential credit risk.

## NAIVE RANDOM OVERSAMPLING
![Screen Shot 2022-08-09 at 7 06 36 PM](https://user-images.githubusercontent.com/100393032/183794764-fe6c02e2-214b-484e-b9b3-347ee996cf4a.png)

- The balanced accuracy is 0.640324421824783 
- Precision is 1% in high_risk and 100% in low_risk
- Recall is slightly higher in high_risk (.66/.62)

## SMOTE OVERSAMPLING
![Screen Shot 2022-08-09 at 7 15 56 PM](https://user-images.githubusercontent.com/100393032/183795589-1115d3ee-15ba-4417-b169-25b4b0caecdc.png)

- The balanced accuracy is 0.6514992150524688
- Precision is 1% in high_risk and 100% in low_risk
- Recall is almost ten points higher in Low_risk (.61/69)

## UNDERSAMPLING
![Screen Shot 2022-08-09 at 7 27 53 PM](https://user-images.githubusercontent.com/100393032/183796895-af0dde83-1967-4016-b6e2-4b6a9f437011.png)

- The balanced accuracy is 0.5443538770387797
- Precision is 1% in high_risk and 100% in low_risk
- Recall is considerably higher in High_risk (.69/.40)

## COMBINATION (OVER AND UNDER) SAMPLING
![Screen Shot 2022-08-09 at 7 30 29 PM](https://user-images.githubusercontent.com/100393032/183797219-f5584ab5-63a1-425a-a6f1-71d3f268630a.png)

- The balanced accuracy is 0.6550612907408608
- Precision is 1% in high_risk and 100% in low_risk
- Recall is very high in High_risk (.75/.56)

## BALANCED RANDOM FOREST CLASSIFIER
![Screen Shot 2022-08-09 at 7 59 57 PM](https://user-images.githubusercontent.com/100393032/183800733-cfb93eea-f9b5-4256-84a5-53eca3d547a4.png)


- The balanced accuracy is 0.7885466545953005
- Precision is 3% in High risk and 100% in Low_risk
- Recall is very high in both high_risk and low_risk (.70/.87)

## EASY ENSEMBLE ADABOOST CLASSIFIER
![Screen Shot 2022-08-09 at 7 49 39 PM](https://user-images.githubusercontent.com/100393032/183799478-e92fbcc0-fc4e-4b9e-a20a-72f9de43cc5c.png)

- The balanced accuracy is 0.9316600714093861
- Precision is 9% in High risk and 100% in Low_risk
- Recall is very high in both high_risk and low_risk (.92/94)

# Analysis Summary
The results of the first four algorithms were very similar with a precision that was mirrored across the board. There are some patterns to see, but for the highest amount of accuracy I would go with the East Ensemble AdaBoost Ckassifier. The balanced accuracy of this model was much higher than the rest with a precentage of 93, the closest to 100% of all these models. This model would give the Loan provider the least amount of credit risk based on the data given. The least lkely model to use would have to be the Undersampling as it has an accuracy of just 54%. 
