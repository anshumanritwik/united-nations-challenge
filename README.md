# united-nations-challenge

open competition on driven data

The above competition is based on prediction of  values for the specified indicators one and five year into the future. The indicators are a part of the larger goals as specified by Unitd Nations. For more details on the challenge please visit the following link :- https://www.drivendata.org/competitions/1/united-nations-millennium-development-goals/

Considering the predictive nature of the problem, The techniques used in the associated jupyter notebook include different variations of regression namely-

1.LARS regression
2.LASSO regression
3.RIDGE regression
4.ELASTIC NET 
5.Simple Linear regression
6.ARD regression

The available solution has been broken down to elaborate each step from pre-processing to the model evaluation process. 

Another variation present in the solution is that of the years being taken into consideration while making the predictions-
- The first approach is to include all the 35 years provided
- The second approach involves considering the most recent three or four years to enhance the quality of predictions
- This approach can again have two variations 
- considering the most recent three years and adding the predicted year's value after every iteration
  - eg. 1st iteration y= [[2005],[2006],[2007]] for predicting 2008; 
  - 2nd iteration y= [[2005],[2006],[2007],[2008]] for predicting 2009 and so on
- conidering only the most recent three years 
  - eg. 1st iteration y= [[2005],[2006],[2007]] for predicting 2008;
  - 2nd iteration y= [[2006],[2007],[2008]] for predicting 2009 and so on.
                
 
CONCLUSION
- Ridge regression with the second variation of years has produced the best result for me so far.
- Random forest regression is another successful regression technique for this problem.
- This problem can also be solved as a typical time series problem. 
