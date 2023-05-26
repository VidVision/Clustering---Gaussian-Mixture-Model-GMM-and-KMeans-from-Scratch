# Clustering-Gaussian Mixture Model (GMM) and KMeans from Scratch
GMM and KMeans Clustering algorithms are coded from scratch in Python. They both are implemented on MNIST dataset and the results are compared.


In this project I implement the EM algorithm for fitting a Gaussian mixture model for the MNIST dataset. The dataset is reduced to be only two cases, of digits "2" and "6" only. Thus, I will fit GMM with $C = 2$. The data file _data.mat_ is used. True label of the data are also provided in _label.mat_ and _label.dat_
 
The matrix _images_ is of size 784-by-1990, i.e., there are totally 1990 images, and each column of the matrix corresponds to one image of size 28-by-28 pixels (the image is vectorized; the original image can be recovered by map the vector into a matrix.) 
 
The following steps are taken in this project:
 
1. Select from data one raw image of "2" and "6" and visualize them, respectively. 

2. Use random Gaussian vector with zero mean as random initial means, and two identity matrices $I$ as initial covariance matrices for the clusters. Plot the log-likelihood function versus the number of iterations to show the algorithm is converging.

3. Report, the fitting GMM model when EM has terminated in the algorithms, including the weights for each component and the mean vectors ( reformat the vectors into 28-by-28 images and show these images ). Ideally, we should be able to see these means corresponds to _average_ images.  

4. Use the $p_{ic}$ to infer the labels of the images, and compare with the true labels. Report the miss classification rate for digits "2" and "6" respectively. Perform $K$-means clustering with $K=2$ . Find out the  miss classification rate for digits "2" and "6" respectively, and compare with GMM.
