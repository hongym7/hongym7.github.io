---
title: "Focal Loss for Dense Object Detection"
date: 2020-06-15 14:00:00 -0400
categories: Paper Review
---

focal loss 는 기존 loss 함수를 재정의한 것이다.  
분류하기 어려운 예제들 (Hard Positives examples-Object)에 높은 가중치를 부여하고 분류하기 쉬운 예제들 (Easy Negatives examples-Background)에는 작은 가중치를 할당한다.  
  
<img src="/assets/img/focal_loss_01.png" />
Cross entropy Loss  

<img src="/assets/img/focal_loss_02.png" />
Focal Loss  

<img src="/assets/img/focal_loss_03.png" />
Focal loss 는 어떤 batch 의 트레이닝 데이터에 같은 weight 를 주지 않고, 분류 성능이 높은 클래스에 대해서는 down-weighting 을 한다. 이 때, gamma (위 그림) 를 주어, 이  down-weighting 의 정도를 결정한다. 이 방법은 분류가 힘든 데이터에 대한 트레닝을 강조하는 효과가 있다  
  
  

출처: https://3months.tistory.com/414
