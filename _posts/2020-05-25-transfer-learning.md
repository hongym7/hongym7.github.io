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
  

 3. 두 데이터가 유사하지 않은 경우에 대해서는 해당 내용이 충분한 설명이 될지는 모르겠으나,
"cs231n 2017년 Lecture7-93 자료"를 참고하고자 합니다(http://cs231n.stanford.edu/slides/2017/cs231n_2017_lecture7.pdf).
- 상당히 다른, 그리고 적은 양의 데이터셋을 transfer learning하는 경우: classification  의 경우, '쉽지 않을 것으로 보이며, 다른 단계에서 classifier 진행할 것'을 말하고 있으며,
- 상당히 다른, 하지만 꽤 많은 양의 데이터셋을 transfer learning하는 경우: '더 많은 layer를 finetuning 하는 방향'으로 설명하고 있습니다.
출처 : https://www.youtube.com/watch?v=sXIurFr804w&lc=Ugyuja-x8x4MKT9ZuKx4AaABAg.994ELdjv08e9ACFVtU4tCw  
