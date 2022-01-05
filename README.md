# Vehicle Claim Fraud
[This](https://www.kaggle.com/shivamb/vehicle-claim-fraud-detection) dataset contains vehicle insurance claims comparing whether not they are fraudulent claims or not. Using the data I've made visuals to further show the data and compare key details within the data. Later I used machine learning classification models to determine whether or not the claims are fraudulent or not.

## Total Monthly Claims
The data contains information from three years 1994-1996. This first graph shows all the years combined and categorized by each month. From the graph, January is the highest month for claims and August is the lowest. Most of the months are pretty close in the number of claims with no outstanding outliers.  
![total Claims by Month](https://user-images.githubusercontent.com/88803320/146809108-b92a6220-811c-40ff-9309-d24e44821fec.png)


## Policy Holders
This graph shows the different age groups of the policyholder. Knowing that a lot of times lower age groups will likely not have their own car as they can use their parents this explains why the age groups 16-25 are very low compare to the other age groups. With the age group, 26-30 is where the 1st incline begins from this we can gather that a lot of people will get their first car around that age group and by 31 to 35 most people have their own car. The number of policyholders start to decline after this could be due to several things such as age, marital status, work location, etc. When people get older they are less likely to drive around since they might have kids or someone to do that for them. A lot of times too some people, when they are married, will just have one car for the entire family which will save money, but lower the number of people that are on the policy. Also, people's work locations can change if you work close to home or work from home you are less likely to need a car as transportation is easier and not needed as much. 

![policy holders](https://user-images.githubusercontent.com/88803320/148271630-77976774-be15-41d8-9665-df79cf2912f3.png)


## Fraud Count for Each Month Over 3 Years
This Graph shows the comparision of 3 years for each separate months. It seams as if 1996 was an odd year as most of the time when the other two years spike 1996 takes a dip and visversa. however comparing 1994 and 1995 they are very similar interms of spiking and dips in the fraud count. One good thing to see from this graph is that over the course of the 3 years the fadulant claims have decreased by a good margin. The highest month for 95 and 94 was the lowest month for 96. 

![3 year Fruad count](https://user-images.githubusercontent.com/88803320/146809119-22b6d9a1-0f6d-4276-9380-3fc04a3b82b8.png)


## Correlation 
![corr](https://user-images.githubusercontent.com/88803320/147151370-7c576902-efac-41f0-830d-4db3053fd99a.png)

## Files Reported Based On Witness
It's more likely that there won't be a witness present. However, 7 more files were reported without a witness present. In most cases, no file will be reported regardless of a witness. 15,000 cases occurred without a witness present whereas 400 cases occurred with a witness present. 

![reports](https://user-images.githubusercontent.com/88803320/148271670-10feb864-0622-45eb-b0fb-00e13c08f90b.png)


## Machine Learning
To determine if a claim was fraudulent or not I used some machine learning models on the target column of the data. Three models were used in comparison to each other KNN, Random Forest, XGBoost. 

### KNN Classification Model
First running a base knn model produced good scores both for the training and testing in the low 90s. After, I ran a grid search to find the best parameters for the model. It didn't improve much other than the training score going up from a 93 to a 94 and the testing score stayed within the 93s.

Train Score: 0.9409\
Testing Score: 0.9377

### Random Forest Model 
To keep some checks within the models I ran a random forest model to compare to the knn. with similar results, the base model gave scores in the low 90s for the train and testing. After running the grid search the testing score increased from low 93s to high 93s. Not a drastic change that's worth noting.

Train Score: 0.9423\
Testing Score: 0.9369

### XGBoost Model
I figured if there was any way to get higher scores than in the low 90s it would be with a boosting model. With the base boosting model the testing scores started in the high 93s and the training in the low 94s. Just like the other models, I ran a gridsearch and the results after left no change.

Train Score: 0.9416\
Testing Score: 0.9364

### Final thoughts 
Out of all the results with each machine learning model all of them had testing scores in the 93s and testing scores in the 94s so the best option, in this case, is to go with the fastest run time. The runtime for the knn model was 0.6s, the runtime for Random forest was 1.2s, and the runtime for the xgboost was 0.5s. With all these results the best model to go with is the KNN model having a fast runtime and the highest of all model scores for testing.