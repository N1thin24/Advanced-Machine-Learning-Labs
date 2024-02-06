# Advanced-Machine-Learning-Labs

1)**Gaussian Mixture Model**:

A Gaussian mixture model is a probabilistic model that assumes all the data points are generated from a mixture of a finite number of Gaussian distributions with unknown parameters. After estimation of those parameters we get an estimation of the distribution of our data. For the clustering task, one can think of mixture models as generalizing k-means clustering to incorporate information about the covariance structure of the data as well as the centers of the latent Gaussians.

The following image displays two clustering results from applying the K-Means and Gaussian Mixture Model (GMM) algorithms on a dataset. The GMM appears to perform better because it can accommodate clusters with different shapes and densities. While K-Means assumes clusters to be spherical and tends to work well on isotropic data distributions, GMM is more flexible as it incorporates covariance between the points in each cluster, allowing for elliptical shapes. The data shown has non-spherical, elongated clusters, which GMM can model more accurately due to its ability to account for such variance, hence providing a better fit than K-Means.

![image](https://github.com/N1thin24/Advanced-Machine-Learning-Labs/assets/107985125/d830880c-c60a-492e-806a-21aa64ed9ef9)

![image](https://github.com/N1thin24/Advanced-Machine-Learning-Labs/assets/107985125/f6eb06f8-a10b-4146-b64f-d23e88ff647c)

2)**BIC, AIC and Cross-Validation**

AIC estimates the relative amount of information lost by a given model; the less information lost, the higher the quality of the model. It favors models that fit the data well while penalizing for complexity (number of parameters).

BIC is similar to AIC but adds a stronger penalty for models with more parameters. It's based on Bayesian probability and penalizes complexity more heavily, often resulting in simpler models than those selected by AIC.

In this lab, we apply AIC and BIC to a GaussianMixtureModel and a logistic regression model to find the optimal number of mixtures and parameters respectively.

Next, we utilise Cross-Validation as a method of evaluating our model. The basic idea is to partition the dataset into K subsets, often called "folds," and then train and evaluate the model K times, each time using a different fold as the test set and the remaining folds as the training set. This process allows the model to be tested on different subsets of the data, providing a more robust estimate of its performance.

Finally, we define a 99% confidence interval of our observed accuracy on the test set for which we believe the real accuracy should be using the Central Limit Theory (CLT) and Hoeffding inequality.


3)**PCA and TSNE**

In this lab, We apply PCA to a medical dataset, in order to do data analysis and to finally tell which medical features could allow doctors to diagnose breast cancer.
First, we plot the variance returned vs number of principal components


![image](https://github.com/N1thin24/Advanced-Machine-Learning-Labs/assets/107985125/d9064b3c-73c0-46de-be2e-941d698f9a31)
![image](https://github.com/N1thin24/Advanced-Machine-Learning-Labs/assets/107985125/95a5ed21-6e7b-4f84-9a36-4e2023a0020a)

 
We then find the most important principal components to retain as well as a plot of the data points as well as their labels along the first two principal components.
![image](https://github.com/N1thin24/Advanced-Machine-Learning-Labs/assets/107985125/6a6755e3-f012-4091-a04b-4ef83a9459a5)

**t-SNE** is a tool to visualize high-dimensional data. It converts similarities between data points to joint probabilities and tries to minimize the Kullback-Leibler divergence between the joint probabilities of the low-dimensional embedding and the high-dimensional data.

We try with plotting PCA results on a more complicated dataset. It can be seen it is very hard to distinguish most clusters in 2D here.
In order to visualize dataset accurately, we are going to project our data using non linear methods in order to decompose faithfully the dataset in order to extract the intrisec structure of the data.

![image](https://github.com/N1thin24/Advanced-Machine-Learning-Labs/assets/107985125/b110d279-c0d3-4779-9344-588a498d0d2e)
![image](https://github.com/N1thin24/Advanced-Machine-Learning-Labs/assets/107985125/0b552aa9-6d95-4cf4-8704-2bdfcabad61a)




