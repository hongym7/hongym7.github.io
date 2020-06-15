---
title: "Focal Loss for Dense Object Detection"
date: 2020-06-15 14:00:00 -0400
categories: Paper Review
---

focal loss 는 기존 loss 함수를 재정의한 것이다.  
분류하기 어려운 예제들 (Hard Positives examples-Object)에 높은 가중치를 부여하고 분류하기 쉬운 예제들 (Easy Negatives examples-Background)에는 작은 가중치를 할당한다.  
  
<img src='../assets/focal_loss_01.png />
