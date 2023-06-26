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

Assignment1: 

In this Assignment we play around with false discovery rates for a completely random dataset and we use it on a synthesized one "autos.csv"
False Discovery Rate Analysis
This repository explores the concept of False Discovery Rate (FDR) and provides examples of its application using R code.

What is False Discovery Rate?
False Discovery Rate is a statistical concept used in hypothesis testing when multiple comparisons are made simultaneously. It addresses the issue of controlling the proportion of false positives among the significant results.

In statistical testing, researchers often set a significance threshold (e.g., p-value < 0.05) to determine which results are considered statistically significant. However, when performing numerous tests simultaneously, such as testing multiple variables in a regression model or conducting multiple hypothesis tests, the likelihood of obtaining false positive results increases.

The False Discovery Rate provides a way to control the expected proportion of false positives among the significant results, allowing researchers to make more accurate interpretations of their findings.

Repository Content
This repository contains R code that demonstrates the application of False Discovery Rate analysis on two datasets: a randomly generated dataset and a synthesized dataset called "autos.csv."

Randomly Generated Dataset
The code begins by generating a random matrix, where each element is drawn from a standard normal distribution. The first column of the matrix is set as the target variable for logistic regression. The logistic regression model is then fitted, and the p-values for the estimated coefficients are extracted. The code also counts the number of significant coefficients based on a predefined threshold.

False Discovery Rate Analysis
The repository includes a function called fdr that performs the False Discovery Rate analysis. This function takes a vector of p-values, an FDR threshold, and an optional parameter to plot the p-values against the FDR line.

The fdr function ranks the p-values in ascending order, calculates the adjusted FDR for each coefficient, and determines the point at which the inequality changes. If the plot option is enabled, the function generates a plot illustrating the relationship between the p-values and the FDR line.

Usage
To use the code in this repository, follow these steps:

Clone or download the repository to your local machine.
Make sure you have R and the required packages installed (e.g., dplyr).
Modify the code or datasets as needed for your specific analysis.
Run the R code in your preferred development environment or the R console.
Note: The code provided serves as an example and may require modifications to suit your specific use case.

References
Benjamini, Y., & Hochberg, Y. (1995). Controlling the false discovery rate: a practical and powerful approach to multiple testing. Journal of the Royal Statistical Society: Series B (Methodological), 57(1), 289-300.
Storey, J. D. (2002). A direct approach to false discovery rates. Journal of the Royal Statistical Society: Series B (Statistical Methodology), 64(3), 479-498.
Please refer to the references above for more detailed information on the False Discovery Rate concept and its applications.

![image](https://github.com/avelmurugan/Machine-Learning/assets/123327239/3323f385-8db5-4ddb-95d4-02b90e55173e)
