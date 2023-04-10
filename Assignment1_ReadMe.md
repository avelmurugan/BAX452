#Part of Machine Learning at UC Davis MSBA

Assignment 1: Linear Regression and FDR

Language: R

Due: Sunday, January 15th 11:59 PM

 

Use the data in autos.csv Download autos.csv 

Submit your writeup and code in one R Markdown document.

Provide evidence to support your answers.

 

Please:

[5 pts] Write code that produces a 10,000 x 1001 matrix (rows x cols) of random numbers drawn from N(0,1). Seed your code using the last 4 digits of your phone number (this number will be different for everyone).  Every time you run the code, it should now yield the exact same (“random”) dataset.
[5 pts] Treat the first column as “y” and the remaining 1000 columns as x’s.
[15 pts] Regress y on x’s. Is an intercept needed?  Why?  Why not?
[5 pts] Create a histogram of the p-values from the regression in Q3. What distribution does this histogram look like?
[15 pts] How many “significant” variables do you expect to find knowing how the data was generated? How many “significant” variables does the regression yield if alpha = 0.01?  What does this tell us?
[10 pts] Given the p values you find, use the BH procedure to control the FDR with a q of 0.1. How many “true” discoveries do you estimate?
[5 pts] Explore the “autos.csv” data. Include any metrics and / or plots you find interesting.
[15 pts] Create a linear regression model to predict price. Explain your model.
[10 pts] Why might false discoveries be an issue?
[15 pts] Use the BH procedure to control the FDR with a q of 0.1. How many true discoveries do you estimate? Plot the cutoff line together with the significant and insignificant p-values.
