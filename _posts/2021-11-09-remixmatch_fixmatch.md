---
title: "RemixMatch, FixMatch"
date: 2021-11-09 10:00:00
categories: Words
---


## Semi-Supervised Learning  
- Supervised Learning은 Labeled data만을 이용하여 만들어진다.  
- But, 현실세계에서는 Unlabeled data가 훨씬 많고 Labeled data와 Unlabeled data를 같이 학습시키는 것이 Semi-Supervised Learning 이다.
  
## Consistency regularization  
- SSL 의 한 부류로
- Input에 변화(Augmentation)을 가했을 때, Output이 변화 전의 Output가 차이가 없어야 한다는 가정으로 모델을 Regulazie하는 방법이다.
- 이 방법의 큰 장점은 label이 없는 데이터에도 적용하다는 것이다.
- 절차 : Unlabeld data의 모델을 통해 나온 예측 값을 정답으로 정하고, Augmentation 적용한 data의 결과값과 이 정답값을 CrossEntropy Loss 를 이용하여 모델을 학습한다
