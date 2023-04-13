# Credit_Risk_Analysis


Overview

In this module, we used skills in data preparation, statistical reasoning, and machine learning to perform an analysis on credit card risk. We built and evaluated models using resampling, imbalanced-learn and scikit-learn libraries to train and evaluate models with unbalanced classes.  We oversampled the credit card dataset from LendingClub using the RandomOverSampler and SMOTE algorithms, and undersample the datat with the ClusterCentroids algorithm. Next, we used a combinatorial approach of oversampling and undersampling with the SMOTEENN algorithm. Then we compared the two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifer, to predict any credit risk.


Results

Naive Random Oversampling

Balanced Accuracy Score: 0.66
Precision: 72/(72 + 6605) = 0.01
Recall: 72/(72 + 29) = 0.71
SMOTE Oversampling

Balanced Accuracy Score: 0.66
Precision: 64/(64 + 5291) = 0.01
Recall: 64/(64 + 37) = 0.63
Undersampling

Balanced Accuracy Score: 0.54
Precision: 70/(70 + 10340) = 0.01
Recall: 70/(70 + 31) = 0.69
SMOTEENN

Balanced Accuracy Score: 0.64
Precision: 73/(73 + 7411) = 0.01
Recall: 73/(73 + 28) = 0.72
Balanced Random Forest Classifier

Balanced Accuracy Score: 0.79
Precision: 71/(71 + 2153) = 0.03
Recall: 71/(71 + 30) = 0.70
Easy Ensemble AdaBoost Classifier

Balanced Accuracy Score: 0.93
Precision: 93/(93 + 983) = 0.09
Recall: 93/(93 + 8) = 0.92


Summary

The Naive Random Oversampling, SMOTEENN and the SMOTE Oversampling algorithm had similar balanced accuracy scores.  Based on the results of this analysis, it seems that Oversampling algorithms do not produce accurate results. The Undersampling algorithms appears to result in a lower balanced accuracy score.  The EasyEnsemble AdaBoost Classifier resulted in the highest balanced accuracy score.  In order to achieve the optimal results, it appears that using a model that sequentially focuses on errors and repeats the process in the next model and has the largest recall allows for the least amount of true negatives to be overlooked.  An EasyEnsemble AdaBoost Classifier would be my recommendation to approach the real world challenge of analyzing credit card risk.    
