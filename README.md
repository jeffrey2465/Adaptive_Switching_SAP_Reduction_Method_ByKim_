# Salt And Pepper Noise 제거 알고리즘 구현

2021.03.03

용량으로 인해 주관적 화질, 테스트 이미지, 노이즈 이미지는 전체를 포함하고 있지 않음
SAP 노이즈 제거의 두번째 방법으로 잡음 비율에 따라 적응적으로 반영
코드에서는 비율에 따라 선택하는 부분은 따로 구현되어 있지 않으며 비율에 따라 결과 merging 함

### 주요 결과
  * MF: opencv api   
  * AMF: NAMF의 Step1에 해당하는 내용 구현 (논문 구현 Code 파이썬 포팅)   
  * NAMF: NAMF 논문 Step1 + Step2 (논문 구현 Code 파이썬 포팅)   
  * Proposed1 : AMF+거리 기반 weighted sum    
  * Proposed2 : Proposed1 + bilateral   
  * Proposed3 : namf + 거리 기반 weighted sum + bilateral   
  * Proposed4 : proposed3 + 자신 weight 포함   
  * Proposed5 : Proposed1 + pixel 신뢰도 weight average   
