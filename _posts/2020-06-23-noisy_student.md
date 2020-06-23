---
title: "Self-training with Noisy Student improves ImageNet classification"
date: 2020-06-23 14:50:00 -0400
categories: Paper Review
---

#### - self training  
 - ImageNet dataset 을 이용하여 Teacher model 학습
 - JFT-300M dataset 을 이용하여 Teacher model 테스트
 - ImageNet dataset + JFT-300M dataset 을 이용하여 Student model 학습  
    
    
#### - 3가지 noisy를 준다. 
 - stochastic depth
 - dropout
 - rand augment
