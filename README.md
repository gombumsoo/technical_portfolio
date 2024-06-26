# technical_portfolio  

## 기술 평가 항목
1. Python, SQL, R, Java, Scala, Go, C/C++, Javascript 등 데이터 처리 언어 활용 능력
5. 데이터사이언스 관련 공모전 참여를 통한 공개 데이터의 활용 및 분석 능력
8. R, Python, Tableau, Power BI 등을 활용한 데이터 시각화 능력
---
## 레포지토리 소개
본 레포지토리는 KAMP에서 제공하는 [에너지(전력) 사용량 데이터](https://www.kamp-ai.kr/aidataDetail?AI_SEARCH=%EC%A0%84%EA%B8%B0&page=1&DATASET_SEQ=27&EQUIP_SEL=&GUBUN_SEL=&FILE_TYPE_SEL=&WDATE_SEL=)를 활용해 공장에서 관측된는 다양한 변수에 대해 전기 사용량을 예측하는 모델을 학습하고, 결과의 분석 내용을 정리한 것입니다.

---
## EDA
EDA에 대한 내용을 Visualization.ipynb에 정리되어 있습니다. 데이터셋에 있는 변수 각각에 대해 적절한 시각화를 통해 인사이트를 얻고, 나아가 변수간의 상관관계 또한 살펴봤습니다.

---
## 모델 학습
모델 학습에 대한 내용은 Modeling_LSTM.ipynb에 정리되어 있습니다. EDA과정에서 확인한 내용을 토대로 일일 전기 소비량 예측에 적합한 변수들을 선택했으며, LSTM모델로 학습을 진행했습니다.  
학습한 모델로 테스트 데이터셋에 대해 예측을 진행했을때, 전반적으로 전기 소비량을 잘 유추하는 것을 확인할 수 있었지만, 8월 초에 제품 생산을 진행하지 않는 특이 케이스가 있어 예측이 빗나간 것을 확인했습니다.
