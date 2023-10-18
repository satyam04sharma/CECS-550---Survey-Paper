# CECS-550---Survey-Paper


## Problem statement 
The paper "Robust and Sparse Linear Discriminant Analysis via an Alternating Direction Method of Multipliers" addresses the problem of polluted data and the limitations of classical L2-norm-based Linear Discriminant Analysis (LDA) in the small sample size (SSS) scenario. When dealing with polluted data, minimizing the sum of squared errors may lead the projection vectors to drift from the desired directions, making LDA easily affected by outliers and noise. Additionally, classical L2-norm-based LDA may suffer from the SSS problem since it's difficult to evaluate the scatter matrix accurately in this situation.

## Current trend on LDA
In the field of machine learning and data analysis, there have been various attempts to develop methods for linear discriminant analysis (LDA) that can handle the challenges posed by different data scenarios. For example, classical LDA methods based on L2-norm optimization have been widely used, but they are susceptible to outliers and noisy data, which can lead to unreliable results. In order to address this issue, robust LDA methods have been developed, which use different objective functions that are less sensitive to noisy data, such as L1-norm optimization or non-convex optimization techniques. Sparse LDA methods have also been proposed, which aim to identify a sparse set of discriminant features that can accurately classify the data. Other extensions of LDA include kernel LD, which can handle nonlinearly separable data, and multiclass LDA, which can classify data into more than two classes.

Currently, there is no one-size-fits-all approach for LDA, as the best method to use depends on the characteristics of the data being analyzed. In many cases, classical LDA is still used as a baseline method, but more advanced techniques are often needed for challenging datasets. Robust LDA methods are increasingly popular, as they can handle noisy data more effectively and often lead to better classification performance. Sparse LDA is also a promising area of research, as it can help to reduce the dimensionality of the data and identify the most important discriminant features. Kernel LDA is commonly used for nonlinearly separable data, and multiclass LDA is useful for classifying data into more than two classes. Overall, the choice of LDA method depends on the specific application and the characteristics of the data being analyzed, and researchers continue to explore new techniques to improve the accuracy and efficiency of LDA.

## Dataset information
Artificial Data 1: The data contain two classes, with 50 samples in each class. Class 1 is generated from a Gaussian distribution of mean (√3, 1) and covariance 
```math
\begin{bmatrix} 5 & 0 \\ 0 & 1 \end{bmatrix}
``` 
, while Class 2 is generated from a Gaussian distribution of mean (4√3, 4) and covariance 

```math
\begin{bmatrix} 1 & 0 \\ 0 & 5 \end{bmatrix}
```

Indian Females: The Indian females database contains 22 distinct subjects and each subject has 11 different images. The original size of each image is 640 × 480 pixels, with 256 gray levels per pixel. Here, we upsample all the images into 32 × 32 pixels. A random subset with p (2, 3, . . . , 10) images per subject is taken to form the training set, while the rest of the data comprise the test set. For each given p, the average result over ten random splits is considered. To test the robustness of various methods, they add three different levels of random noise to each whole face: the noise is zero-mean Gaussian  distributed with variances 0.01, 0.03, and 0.05.

IMM database: It is a face database that was collected at the Institute for Mathematical Modelling (IMM) at the Technical University of Denmark. The database consists of 14 sequences of images, with each sequence containing 16 images of the same individual captured under different lighting conditions. Each image has a resolution of 256x256 pixels and is stored in color. The authors used the grayscale version of the IMM database in their experiments.

ORL database: The ORL database is a face database that is publicly available and has been widely used in the computer vision and pattern recognition communities. The database consists of 400 grayscale images of 40 distinct individuals, with 10 images per individual taken at different times and under different lighting conditions. Each image has a resolution of 92x112 pixels. The ORL database was originally collected by the Olivetti Research Laboratory (ORL) in Cambridge, UK, and was later made publicly available for research purposes.
