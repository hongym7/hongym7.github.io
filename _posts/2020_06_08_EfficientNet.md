---
title: "EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks"
date: 2020-06-08 10:27:00 -0400
categories: Paper Review
---


## Intro
Conv Network의 scale을 키우면서 accuracy와 efficiency를 높히는 방법을 찾아보자  
그건 network의 width/depth/resolution을 조화롭게 키우는 것이다.  
**compound scaling methods** 라 한다  
  
<img src="/assets/img/efficientnet_01.png" width="90%"/>
- width scaling : conv patch의 channel을 늘려서  
- depth scaling : conv layer를 길게 만든는
- resoulution scaling : input 시, 이미지의 w, h 를 크게 만드는
- compound scaling : 위 3가지를 조화롭게  




<img src="/assets/img/efficientnet_02.png" width="90%"/>
