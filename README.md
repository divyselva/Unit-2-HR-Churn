# Project Overview
### Problem Statement:

* Wants to know why high performers are churning
* Comparison of churn rates of high performers to non high performers

### Outcomes Predictions:

* Churn model, identifying factors that increase the likelihood of high performer churning
* Same as overall (?)

### Data Acquisition:

* Data acquired was clean
* Columns include: 'id', 'satisfaction_level', 'last_evaluation', 'number_project', 'average_montly_hours', 'time_spend_company', 'Work_accident', 'churn', 'promotion_last_5years', 'sales', 'salary'.

### Data Preparation: 

* Renamed columns: average_montly_hours → average_monthly_hours, sales → dept
* looked at df shape, head, tail, unique values, datatypes, columns
* Separated columns into variable types: Categorical, Numerical, Ordinal, Target
* Dummy Variables = Ordinal (salary) and dept
* looked at histograms for numerical variables
* Separated high performers in new df (high performer = last eval >0.8, number of projects > 3 

### Modeling:

* LogisticRegression to model overall data and compare coefficients
* Created DecisionTreeClassifier 

### Model Evaluation:

* DecisionTreeClassifier had a good recall score

### Deliverable:

* important factors affecting churning for overall company
* factors affecting churning in high performers
* Pockets of churners (high likelihood of churning) 

## CONCLUSION
* The main points for why the high performing employees are churning: 
  * They feel unsatisfied 
  * Feel overworked (*long hours, too many projects*)
  * Have spent a long time at the company
  * Not enough promotions
  * Low salary levels
  
 #### Future Works
 * Further advance the model by:
  * Identifying how the factors may relate to each other - *Can use other methods to find what causes employees on the verge of churning to churn*
  * Use the model and insights to design a program that is targeted towards the employees you want to retain 


