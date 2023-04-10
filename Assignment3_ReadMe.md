Assignment 3: Model Selection

Language: R

Due: Sunday, January 28th 11:59 PM

 

Use the data in heart.csv Download heart.csv 

Submit your writeup and code in an R Markdown and HTML document.

Provide evidence to support your answers.

 

Please:

[20 points] For the above dataset (Dependent variable: heart_attack)
How would you choose a sample subset (such as missing value, nulls, empty columns) of this dataset? What criteria would you consider when selecting a training subset from the above dataset (such as balanced distribution between training and test for the treated observations) ?
Randomly split the dataset into test and training sets using 80% observations as training set. Fit a simple linear regression model (full model) to predict the heart attack probability and test your model against the test set.  Explain your model and obtain the R^2 for the predictions of the test data set (i.e., a true OOS R^2).
 

[10 points] Explain cross-validation and highlight the problems that may be associated with a cross-validation approach.
 

[25 points] Use only the training sets from question 1 and estimate an 8-fold cross-validation to estimate the R^2 of the full model. e., use cross-validation to train (on 7/8 of the training set) and evaluate (on 1/8 of the training set).  Calculate the mean R^2 from the 8-fold cross-validation and compare it with the R^2 from question 1.  Please explain your observation.
 

[10 points] Explain Lasso regression and how does it work. List the pros and cons associated with using it.
 

[25 points] Use again the training sets from question 1 and
Fit a Lasso regression to predict the heart attack probability. Use cross-validation to obtain lambda_min as well as lambda_1se Explain the two resulting models. Which one would you choose?
Compare model outputs from questions one, three, and five.
 

[10 points] What is AIC, and how is it calculated? When to use AICc (corrected AIC)?
