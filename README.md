# Gaussian Clustered Support Vector Machines (GCSVM) for Credit Scoring
## Overview

This repository contains the implementation of the Gaussian Clustered Support Vector Machine (GCSVM), a novel hybrid clustering-classification approach designed for credit risk assessment. GCSVM was developed to improve the efficiency and performance of the traditional Support Vector Machine (SVM), especially when dealing with the challenges posed by **imbalanced datasets** in credit scoring.

## Methodology (GCSVM)

The GCSVM model is a combination of the Gaussian Mixture Model (GMM) and the Support Vector Machine (SVM).

### The core approach is as follows:

**1- Imbalance Treatment & Clustering:** The GCSVM leverages the Gaussian Mixture Model (GMM) for partitioning the training dataset into distinct, localized subsets. A significant benefit of this approach is that the GMM's component distributions can be used to effectively manage data imbalance by guiding the sampling and segmentation process, ensuring more balanced and efficient training for the local classifiers.

**2-Classification:** A linear SVM is constructed within each resulting training subset and serves as a base classifier.

**3-Ensemble:** The final classification result is derived from the ensemble of the base SVM classifiers.

## Performance Highlights
The GCSVM approach demonstrates improved classification performance compared to the standard linear SVM method.

The model's accuracy is specifically investigated and proven effective on real-world imbalanced datasets.

GCSVM's performance is shown to be comparable or superior to four other standard credit scoring models.

