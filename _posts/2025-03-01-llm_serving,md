---
title: "RemixMatch, FixMatch"
date: 2021-11-09 10:00:00
categories: Words
---


# Semi-Supervised Learning  
- Supervised Learning은 Labeled data만을 이용하여 만들어진다.  
- But, 현실세계에서는 Unlabeled data가 훨씬 많고 Labeled data와 Unlabeled data를 같이 학습시키는 것이 Semi-Supervised Learning 이다.
  
## Consistency regularization  
- SSL 의 한 부류로
- Input에 변화(Augmentation)을 가했을 때, Output이 변화 전의 Output가 차이가 없어야 한다는 가정으로 모델을 Regulazie하는 방법이다.
- 이 방법의 큰 장점은 label이 없는 데이터에도 적용하다는 것이다.
- 절차 : Unlabeld data의 모델을 통해 나온 예측 값을 정답으로 정하고, Augmentation 적용한 data의 결과값과 이 정답값을 CrossEntropy Loss 를 이용하여 모델을 학습한다

## MixMatch
- Consistency Training과 Mixup 이용한 SSL 방법론

## ReMixMatch
- 기존 MixMatch에서 두 가지 추가점을 제안
1. Distirbution Alignment : Labeled data 와 Unlabeled data에서 각 class 비율을 맞춰준다.
2. Augmentation Anchoring : Weak Augmentation 1번, Strong Augmentation 8번을 수행. String Augmentation의 정답 분포가 Weak Augmentation의 정답 분포를 따라가도록 학습한다.

## FixMatch
- Labeled Image는 Supervised Learning
- Unlabeled Image는 Weekly Augment 를 수행하여 일정한 Threshold를 넘은 class 값으로 Pseudo-label로 이용하여, Strongly Augment 한 것이 이 Psedo-label을 따라가도록 학습한다. Threshold를 넘지 않으면 loss 계산을 하지 않는다. 즉 Labeled Image만 학습된다.
- 이는 초반에는 labeled data만 학습될 것이고, 학습이 진행되면서 Threshold를 넘으면서 점점 unlabed data도 학습이 될 것이다
