# Credit_Risk_Analysis

## Challenge Overview:
*Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans.*

*Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm.*

*Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm.*

*Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.*

*Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk*


### Deliverables:
Deliverable 1: Use Resampling Models to Predict Credit Risk
Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk
Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
Deliverable 4: A Written Report on the Credit Risk Analysis

### Resources:
Data Sources: LoanStats_2019Q1.csv

Software:
    - Jupyter Notebook
    - Python


## Challenge Results:

### Deliverable 1 Results: Use Resampling Models to Predict Credit Risk
#### Oversampling RandomOverSampler Model:

![randomoversampler_balanced_accuracy](https://user-images.githubusercontent.com/36451701/129460568-458b92a1-a644-4a1b-b27c-1b2a877df4b8.png)

![randomoversampler_confusion_matrix](https://user-images.githubusercontent.com/36451701/129460574-f136466c-779f-468c-892f-fd2aa55de885.png)

![randomoversampler_classification_report](https://user-images.githubusercontent.com/36451701/129460579-f27c5f5a-5265-4dfd-9e11-63cd73f34036.png)

#### SMOTE Oversampling Model:

![smote_balanced_accuracy](https://user-images.githubusercontent.com/36451701/129460626-00ce42b6-f294-4423-b0b7-f9d7efd8422c.png)

![randomoversampler_confusion_matrix](https://user-images.githubusercontent.com/36451701/129460629-c3de3ce0-0b7a-41d2-bc07-371b460f2738.png)

![randomoversampler_classification_report](https://user-images.githubusercontent.com/36451701/129460631-6f5e94c8-5291-4cae-ab30-1ffb2ba626a6.png)

#### Undersampling ClusterCentroids Model:

![undersampling_balanced_accuracy](https://user-images.githubusercontent.com/36451701/129460635-91291144-4e69-4b62-a191-765d0e4dd7a8.png)

![undersampling_classification_report](https://user-images.githubusercontent.com/36451701/129460638-c9605e7a-91cc-499f-8490-3f82de939349.png)

![undersampling_confusion_matrix](https://user-images.githubusercontent.com/36451701/129460640-fa638bb6-0616-4e16-9d75-1d3d88f3f2ec.png)

### Deliverable 2 Results: Use the SMOTEENN Algorithm to Predict Credit Risk

#### Combination Sampling SMOTEENN Model:
combo image 1
combo image 2
combo image 3

### Deliverable 3 Results: Use Ensemble Classifiers to Predict Credit Risk

#### Balanced Random Forest Classifier


#### Easy Ensemble AdaBoost Classifier

## Challenge Summary:
