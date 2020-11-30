---
title: "Pseudo Labeling"
date: 2020-11-30 14:00:00
categories: Terms
tags: [PseudoLabeling, SemisupervisedLearning]
---
   
### Pseudo Labeling 이란 ?  
#### - Test Data 에 대하여 Predict한 Label 값을 이용하여 Re-Train 하여 성능을 높히는 Semi-supervised Learning 의 한 방법  
  
  
### 단계
1. Build a model using training data.
2. Predict labels for an unseen test dataset.
3. Add confident predicted test observations to our training data
4. Build a new model using combined data.
5. Use your new model to predict the test data  
  


