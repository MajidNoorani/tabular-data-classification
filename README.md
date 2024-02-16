# tabular-data-classification

## Datasets
----------------
### Mushroom Dataset
Data is downloaded from this [web page](https://archive.ics.uci.edu/dataset/848/secondary+mushroom+dataset) which is a tabular data for classification of mushrooms. This data is placed in this [folder](/data/Secondary%20Mushroom%20Dataset/)

#### Data information:
- #Instances: 61068
- #Features: 20
- Class Labels: edible=e, poisonous=p

## Models and Implementations:
------------------
### Mushroom classification using RandomForest
File: [mushroom_classification.ipynb](mushroom_classification.ipynb)

Missing values have been handled by KNNImputer. 
- number of neighbors = 5
- samples are weighted with distance strategy

10% of the data is separated for Test set and the rest is used for training and cross-validation

Randomforest is used for the classification task and HalvingRandomSearchCV is used for cross-validation.

The model is evaluated using these metrics:

- F1 score: 0.9997
- Accuracy: 0.9996
- MCC: 0.9993
- AUC: 0.9997
- Confusion Matrix: 

<div style="text-align:center">
  <img src="https://github.com/MajidNoorani/tabular-data-classification/blob/main/assets/ConfMat.png" width="400" height="400" />
</div>

------------------