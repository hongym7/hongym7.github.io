---
title: "How transferable are features in deep neural networks?"
date: 2020-05-25 18:00:00
categories: Paper Review
---

<img src="/assets/img/transfer_learning.PNG" width="90%"/>

- baseA         : A dataset Train  
- baseB         : B dataset Train  
- selffer BnB   : baseB를 가져와 n 번째 layer 까지 freezing 하고 Train  
- selffer BnB<sup>+</sup>  : baseB를 가져와 n 번째 layer 까지의 가중치로 초기화하여 전체 Train  
- transfer AnB  : baseA를 가져와 n 번째 layer 까지 freezing 하고 Train  
- __transfer AnB<sup>+</sup>__ : baseA를 가져와 n 번째 layer 까지의 가중치로 초기화하여 전체 Train (Fine Tunning, 성능 가장 우수)  

단, A B dataset이 유사한 경우.  
  
Fine Tuning 이란?  
- 기존에 학습되어져 있는 모델을 기반으로 아키텍쳐를 새로운 목적(나의 이미지 데이터에 맞게)변형하고 이미 학습된 모델 Weights로 부터 학습을 업데이트하는 방법을 말한다. 

