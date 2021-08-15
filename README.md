# Credit_Risk_Analysis

## Credit Risk Analysis Project Overview:
*Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans.*

*Using a credit card credit dataset and Python, several machine learning modules will be used to evaluate and predict credit risk.*

*Once these models have been completed, their performance will be evaluated and a written recommendation will be made on whether they should be used to predict credit risk*

Technicals used in this project to predit credit risk:

   - Oversample the data using the RandomOverSampler and SMOTE algorithms.
   - Undersample the data using the ClusterCentroids algorithm.
   - A combinatorial approach of over- and undersampling using the SMOTEENN algorithm.
   - Compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

### Deliverables:
   - Deliverable 1: Use Resampling Models to Predict Credit Risk
   - Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk
   - Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
   - Deliverable 4: A Written Report on the Credit Risk Analysis

### Resources:
Data Sources: 
    - LoanStats_2019Q1.csv

Software:
    - Jupyter Notebook 6.1.4
    - Python 3.8.5


## Credit Risk Analysis Project Results:

## Deliverable 1 Results: Use Resampling Models to Predict Credit Risk
### Oversampling RandomOverSampler Model:

![randomoversampler_balanced_accuracy](https://user-images.githubusercontent.com/36451701/129460568-458b92a1-a644-4a1b-b27c-1b2a877df4b8.png)

![randomoversampler_confusion_matrix](https://user-images.githubusercontent.com/36451701/129460574-f136466c-779f-468c-892f-fd2aa55de885.png)

![randomoversampler_classification_report](https://user-images.githubusercontent.com/36451701/129460579-f27c5f5a-5265-4dfd-9e11-63cd73f34036.png)

   - Accuracy Score for the RandomOverSampler model is 63%
   - The precision for the high-risk is 1% and F1 score is 2%, which are not good enough to state that the model will be good at classifying.

### SMOTE Oversampling Model:

![smote_balanced_accuracy](https://user-images.githubusercontent.com/36451701/129460626-00ce42b6-f294-4423-b0b7-f9d7efd8422c.png)

![randomoversampler_confusion_matrix](https://user-images.githubusercontent.com/36451701/129460629-c3de3ce0-0b7a-41d2-bc07-371b460f2738.png)

![randomoversampler_classification_report](https://user-images.githubusercontent.com/36451701/129460631-6f5e94c8-5291-4cae-ab30-1ffb2ba626a6.png)

   - The accuracy score of the SMOTE model is a little bit better than the RandomOverSampler.
   - The precision for the high-risk is very low at 1%, indicating a large number of false positives, which indicates an unreliable classification.
   - The F1 score is 2% which also very low. 

### Undersampling ClusterCentroids Model:

![undersampling_balanced_accuracy](https://user-images.githubusercontent.com/36451701/129460635-91291144-4e69-4b62-a191-765d0e4dd7a8.png)

![undersampling_confusion_matrix](https://user-images.githubusercontent.com/36451701/129460640-fa638bb6-0616-4e16-9d75-1d3d88f3f2ec.png)

![undersampling_classification_report](https://user-images.githubusercontent.com/36451701/129460638-c9605e7a-91cc-499f-8490-3f82de939349.png)

   - The 51% accuracy score of ClusterCentroids model performs poorly when compared to the RandomOverSampler and SMOTE models.
   - The precision (1%) and the F1 (1%) are still very low just like the RandomOverSampler and SMOTE models.
   - The ClusterCentroids model is not good at classifying fraudulent loan applications because the model's accuracy, 0.516, and F1 score are low.

## Deliverable 2 Results: Use the SMOTEENN Algorithm to Predict Credit Risk

### Combination Sampling SMOTEENN Model:

![combo_balanced_accuracy](https://user-images.githubusercontent.com/36451701/129460722-b30b8979-fb61-46d7-8d79-1edb6e29e879.png)

![combo_confusion_matrix](https://user-images.githubusercontent.com/36451701/129460732-945aa41b-bde0-4c7d-a58c-42d8322b454a.png)

![combo_classification_report](https://user-images.githubusercontent.com/36451701/129460736-eda47aad-3b26-4be5-8599-0c853f49e2b7.png)

   - We do see an increase accuarcy score (63%) over the ClusterCentroids model (51%) but still about same as RandomOverSampler and SMOTE models accuarcy scores.
   - The precision (1%) and the F1 (1%) are still very low for high-risk group, just like the RandomOverSampler, SMOTE and Clustercentroids models.

## Deliverable 3 Results: Use Ensemble Classifiers to Predict Credit Risk

### Balanced Random Forest Classifier Model:

![balanced_random_forest_classification](https://user-images.githubusercontent.com/36451701/129460824-8527e234-53ee-4489-afb2-327c5794b0a0.png)

   - The precision score for the high-risk has imporved at bit (4%), but still indicates a large number of false positives, which indicates an unreliable positive classification.
   - The F1 score is still low (14) but improving.

### Easy Ensemble AdaBoost Classifier Model:

![Easy_Ensemble_AdaBoost_Classifier](https://user-images.githubusercontent.com/36451701/129460837-711f9aad-88f6-4455-938a-f8e5604937d2.png)

   - The accuracy score of the EasyEnsembleClassifier model is a much improved 93% over all the other models. 
   - The high-risk precision (7) and F1 score (14) have improved over all the other models. 
   - The low-risk precision (1.0) and recall (94) and F1 (97) are the highest of all the models. 


## Credit Risk Analysis Project Summary:

Overview of the analysis: Explain the purpose of this analysis.

Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results

Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

There are two things you may research to improve your model.

Modify your model
Balance your dataset to improve data quality

Such is why the F1 score is so important in evaluating models on unbalanced datasets; it accounts for the performance of all classes.
