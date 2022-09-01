# Credit_Risk_Analysis

## Overview of the loan prediction risk analysis
The purpose of this analysis is to predict credit card risk. This will be done by using various algorithms such as RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN, BalancedRandomForestClassifier, and EasyEnsembleClassifier. These algorithms will be compared to see which one better predicts the credit card risk.

## Results

#### RandomOverSampler

![RandomOverSampler](https://user-images.githubusercontent.com/64383146/187827869-247f584c-5362-44c7-abfa-28fc0e3a1bfa.png)

- The **balanced accuracy score** for this algorithm was 0.6158560660083559
- The **precision score** was 0.01 and the **recall score** was 0.60

#### SMOTE

![SMOTE](https://user-images.githubusercontent.com/64383146/187827808-f6247d64-2036-4f62-8f76-bd0707ed6da5.png)

- The **balanced accuracy score** for this algorithm was 0.6216978699574153
- The **precision score** was 0.01 and the **recall score** was 0.60

#### ClusterCentroids

![ClusterCentroids](https://user-images.githubusercontent.com/64383146/187827906-fd2acc01-f0ad-41be-8a33-75fb35a2f59d.png)

- The **balanced accuracy score** for this algorithm was 0.5159612184794389
- The **precision score** was 0.01 and the **recall score** was 0.60

#### SMOTEENN

![SMOTEENN](https://user-images.githubusercontent.com/64383146/187827163-1426334b-12b0-4bba-9e86-a3c4211fcc6b.png)

- The **balanced accuracy score** for this algorithm was 0.6375241226214794
- The **precision score** was 0.01 and the **recall score** was 0.70

#### BalancedRandomForestClassifier

![BalancedRandomForestClassifier](https://user-images.githubusercontent.com/64383146/187827341-66222a7a-d365-408b-9a68-e08b43e8107e.png)

- The **balanced accuracy score** for this algorithm was 0.783495695194814
- The **precision score** was 0.03 and the **recall score** was 0.68

#### EasyEnsembleClassifier

![EasyEnsembleClassifier](https://user-images.githubusercontent.com/64383146/187827497-a6720a36-07fb-49ea-a2f9-39b9aeceda2a.png)

- The **balanced accuracy score** for this algorithm was 0.9250476409184122
- The **precision score** was 0.07 and the **recall score** was 0.91

## Summary

In summary, the precision and recall score for the RandomOverSampler, SMOTE and ClusterCentroids algorithms were the same, with the SMOTEENN one also being very similar, only having its recall score be 0.70 instead of 0.60 like the others. Closely behind those ones, the BalancedRandomForestClassifier algorithm had a precision score of 0.03 and a recall score of 0.68. With the best scores out of all 6, the EasyEnsembleCLassifier had a precision score of 0.07 and a recall score of 0.91.

The model that should be used is the **EasyEnsembleClassifier** as its balanced accuracy score, precision score, and recall score were all higher than the other models. It was 92.5% accurate in predicting the correct results, 14.2% higher than the BalancedRandomForestClassifier which was the second highest. This model had a recall rate of 91%, which means that for all high-risk loans, the model had a 91%  chance of predicting that it was high-risk.
