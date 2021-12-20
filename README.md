# Vehicle Claim Fraud
[This](https://www.kaggle.com/shivamb/vehicle-claim-fraud-detection) dataset contains vehicle insurance claims comparing whether not they are fraudulent claims or not. Using the data I've made visuals to further show the data and compare key details within the data. Later I used machine learning classification models to determine whether or not the claims are fraudulent or not.

## Total Monthly Claims
The data contains information from three years 1994-1996. This first graph shows all the years combined and categorized by each month. From the graph, January is the highest month for claims and August is the lowest. Most of the months are pretty close in the number of claims with no outstanding outliers.  
![total Claims by Month](https://user-images.githubusercontent.com/88803320/146809108-b92a6220-811c-40ff-9309-d24e44821fec.png)


## Policy Holders
This graph shows the different age groups of the policyholder. Knowing that a lot of times lower age groups will likely not have their own car as they can use their parents this explains why the age groups 16-25 are very low compare to the other age groups. With the age group, 26-30 is where the 1st incline begins from this we can gather that a lot of people will get their first car around that age group and by 31 to 35 most people have their own car. The number of policyholders start to decline after this could be due to several things such as age, marital status, work location, etc. When people get older they are less likely to drive around since they might have kids or someone to do that for them. A lot of times too some people, when they are married, will just have one car for the entire family which will save money, but lower the number of people that are on the policy. Also, people's work locations can change if you work close to home or work from home you are less likely to need a car as transportation is easier and not needed as much. 
![poclicy holders](https://user-images.githubusercontent.com/88803320/146809114-54f866b7-870d-44ff-8e29-fe51f11551fe.png)


## Fraud Count for Each Month Over 3 Years
This Graph shows the comparision of 3 years for each separate months. It seams as if 1996 was an odd year as most of the time when the other two years spike 1996 takes a dip and visversa. however comparing 1994 and 1995 they are very similar interms of spiking and dips in the fraud count. One good thing to see from this graph is that over the course of the 3 years the fadulant claims have decreased by a good margin. The highest month for 95 and 94 was the lowest month for 96. 
![3 year Fruad count](https://user-images.githubusercontent.com/88803320/146809119-22b6d9a1-0f6d-4276-9380-3fc04a3b82b8.png)

## Machine Learning
