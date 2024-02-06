# Advanced-Machine-Learning-Labs

GMM:

A Gaussian mixture model is a probabilistic model that assumes all the data points are generated from a mixture of a finite number of Gaussian distributions with unknown parameters. After estimation of those parameters we get an estimation of the distribution of our data. For the clustering task, one can think of mixture models as generalizing k-means clustering to incorporate information about the covariance structure of the data as well as the centers of the latent Gaussians.

The following image displays two clustering results from applying the K-Means and Gaussian Mixture Model (GMM) algorithms on a dataset. The GMM appears to perform better because it can accommodate clusters with different shapes and densities. While K-Means assumes clusters to be spherical and tends to work well on isotropic data distributions, GMM is more flexible as it incorporates covariance between the points in each cluster, allowing for elliptical shapes. The data shown has non-spherical, elongated clusters, which GMM can model more accurately due to its ability to account for such variance, hence providing a better fit than K-Means.

![image](https://github.com/N1thin24/Advanced-Machine-Learning-Labs/assets/107985125/d830880c-c60a-492e-806a-21aa64ed9ef9)

![image](https://github.com/N1thin24/Advanced-Machine-Learning-Labs/assets/107985125/f6eb06f8-a10b-4146-b64f-d23e88ff647c)

