---
title: "RetinaFace: Single-stage Dense Face Localisation in the Wild"
date: 2020-05-18 17:40:00 -0400
categories: Paper Review
---

Face Recognition는 크게 이미지에서 Face를 찾는 Face Detection 단계와 이미지의 Face와 DB 의 Face를 비교하는 단계. 크게 2 단계로 나눌 수 있다.
RetinaFace는 Face Detection 하는 단계에서 사용된다.
Face Detection 을 상세하게 살펴본다면 이미지에서 (Face를 찾고 Landmark를 찾아서) Face 영역을 Crop하고 Wrapping 해주는 작업 수행.

Multi Task Learning
1. face localization
2. face landmarks
3. dense localization mask
이를 통해 face detection 성능을 높힘


