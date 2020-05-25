---
title: "How transferable are features in deep neural networks?"
date: 2020-05-25 18:00:00 -0400
categories: Paper Review
---

<img src="/assets/img/transfer_learning.PNG" width="90%"/>

baseA         : A dataset Train </br>
baseB         : B dataset Train </br>
selffer BnB   : baseB를 가져와 n 번째 layer 까지 freezing 하고 Train </br>
selffer BnB+  : baseB를 가져와 n 번째 layer 까지의 가중치로 초기화하여 전체 Train </br>
transfer AnB  : baseA를 가져와 n 번째 layer 까지 freezing 하고 Train </br>
transfer AnB+ : baseA를 가져와 n 번째 layer 까지의 가중치로 초기화하여 전체 Train (Fine Tunning, 성능 가장 우수) </br>

단, A B dataset이 유사한 경우.

