Assignment 5

Language: Python

Due: Sunday, February 19th 11:59 PM

 

Please submit your writeup and code in one Python notebook.

Provide evidence to support your answers. 

The Madelon dataset Download Madelon datasetis a synthetic dataset that was generated for a machine learning competition. It is a high-dimensional dataset, with 500 features and 2,600 data points. It has a highly non-linear structure, and in this homework assignment, you’ll be diving into it further with PCA and k-means clustering. When you are asked to generate a plot, please provide the image in your final writeup along with a brief analysis of its major features.

Before performing any dimensionality reduction, write a program to use k-means clustering on the Madelon dataset. Try the following k values: 4, 8, 16, 32, 64. 
What preprocessing techniques did you apply, if any?
Describe qualitatively: how does the number of clusters affect the performance of the clustering algorithm on the dataset? 
Generate a plot of the number of clusters k (x-axis) versus the sum of squared distance (SSE) between data points and their assigned centroids (y-axis). What appears to be the optimal k from the list of values you used, and why? 
For k = 8, how did you initialize the set of cluster centroids before running k-means? Rerun k-means again, this time ensuring that the centroids are all different. Does this – and if so, to what extent – affect the final clusters created?
More generally for any dataset, what evaluation metrics can be used to assess the quality of the clusters produced?
The Madelon dataset is high-dimensional, with 500 features per data point. Some of these features might be redundant or noisy, making clustering more difficult. 
Fit the standardized data with PCA. Then, create a cumulative variance plot – showing the number of components included (x-axis) versus the amount of variance captured (y-axis). Generally, we want to retain at least 75% of the variance. How many components would you decide to keep?
Perform PCA with your selected principal components.
Plot the transformed data on a graph with the first two principal components as the axes i.e. x = PC 1, y = PC 2.
Plot the original data on a graph with the two original variables that have the highest absolute combined loading for PC 1 and PC 2 i.e. maximizing |loading PC1| + |loading PC2|.
Examine the scatter plot of PC 1 (x-axis) versus PC 2 (y-axis) for all data points that you created in the previous part. Qualitatively, can you identify visible clusters? Why or why not might this be the case with this particular dataset?
3.   Now, we will run k-means clustering on the transformed data from the previous problem.

Why is it a good idea to do this, especially for high-dimensional datasets? Name a number of reasons.
Use the same k values again (4, 8, 16, 32, 64) to again generate an elbow plot. 
What is the optimal k? Is it different from the one you found in (1)?
Compare the SSE values plotted in this exercise to the previous plot you generated in (1c) before performing PCA.
Again, create a scatter plot of PC 1 (x-axis) versus PC 2 (y-axis) for all of the transformed data points. Label the cluster centers and color-code by cluster assignment for the first 5 iterations of k = 32. Can you see the algorithm begin to converge to optimal assignments?
