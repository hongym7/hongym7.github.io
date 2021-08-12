---
title: "Deep Compression"
date: 2021-06-01 14:00:00
categories: Paper
---


## Deep Compression: Compressing Deep Neural Networks with Pruning, Trained Quantization and Huffman Coding  

### Deep Compression은 딥러닝 모델 네트워크를 압축하여 모델의 용량과 에너지 소비량을 획기적으로 줄임
#### 1. Network Pruning
가중치가 작은 연결에 대해 연결을 끊는다 (0 값으로 대체). Dropout과 유사한 메카니즘

#### 2. Trained Quantization
가중치 표현의 비트 수를 감소 시키고, 가중치를 공유.  
공유되어지는 가중치(Centroids)는 Fine Tunning을 통해 학습되어진다.

#### 3. Huffman Coding
