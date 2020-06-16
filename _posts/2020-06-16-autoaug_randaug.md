---
title: "AutoAugment and RandAugment"
date: 2020-06-16 14:00:00 -0400
categories: Terms
---
  
## Auto Augment  
* 수동으로 정하는 Augmentation을 자동으로 Augmentation 찾아주도록 함
* 여러가지 sub policies로 구성된 설계 공간을 탐색하고 각 미니 배치의 각각 이미지에 대해 랜덤으로 선택
* sub policies는 Rotation, Translation, shearing 과 같은 처리 방법 과 적용되는 확률,크기 로 구성  
* 강화학습 이용  
* PBA, Fast autoaugment - 기존 auto augment의 처리속도를 향상
  
## Rand Augment
* 기존 연구에서는 proxy task에서 학습한 augmentation이 큰 타겟 task에도 적용된다고 가정하지만 이러한 가정에 문제가 있음을 지적
* augmentation의 정도는 모델과 데이터 셋 사이즈에 의존하기 때문에 proxy task에서 찾은 해는 최적해가 아니라 차선이라는 것
* 항상 1/k 균등분포로써 transformation이 선택되도록 함
* 
  
    
           

출처 : http://blog.naver.com/PostView.nhn?blogId=laonple&logNo=221833957779&categoryNo=0&parentCategoryNo=0&viewDate=&currentPage=1&postListTopCurrentPage=1&from=postView
