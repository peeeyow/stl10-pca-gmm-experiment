# stl10-pca-gmm-experiment

STL10 dimensionlity reduction using PCA and labeling using GMM

## PCA and GMM from scratch

PCA and GMM were implemented from scratch by only using python and numpy. STL10 dataset was used for the whole experiment. A subset of the STL10 unlabeled split were used to find the projection matrix fitted for the dataset. Various dims were use to test how well the PCA will perform for the unseen STL10 test split.  
After analyzing the effectiveness of various dims, an optimal dim was determined. The STL10 unlabeled dataset was encoded using the optimal dim. These codes were then used in the GMM. The GMM was used to try to cluster the codes. The clusters where then labeled using the labeled STL10 test split. The performance of the GMM for clustering was then evaluated. The notebook can be accessed [here](/stl10_pca_gmm_experiment.ipynb).

## Sklearn's PCA and GMM Implementation

The sanity of the experiment and the algorithm's implementation from scratch above was verified using the well tested PCA and GMM modules of sklearn. Overall, both the implementation from scratch and sklearn's modules yield the same trend in the results. The notebook can be accessed [here](/pca_gmm_modules.ipynb).
