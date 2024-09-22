# Repeat_Buyer_Prediction
 
## ✍ 요약
- 재구매 확률 예측 모델링
- 본 프로젝트는 Tmall.com의 'double11 day' 당일 프로모션 기간 동안 획득한 가맹점 세트와 해당 신규 구매자를 활용하여 분석 및 예측 모델링을 진행
- 특정 기간(6개월) 내 특정 판매자의 신규 구매자들에 대해 반복 구매가 발생할 확률을 예측
- 불균형 데이터셋의 성능을 높이기 위한 다양한 방식 적용 (MICE, Cost sensitive learning)

### 데이터 전처리 및 EDA
- 사용자 정보, 로그 데이터, 트레인/테스트 데이터 로드
- 결측치 처리: MICE 방법으로 age_range와 gender 변수 보간
- 시계열 데이터 분석: 11월 11일(더블11) 기준으로 구매 패턴 분석

### 특성 엔지니어링
- 사용자, 판매자, 사용자-판매자 쌍에 대한 다양한 집계 특성 생성
- 월별 특성 및 추세선 특성 생성
- 더블11 관련 특성 생성
- PCA를 통한 차원 축소


##
![캡스톤디자인 경진대회  Cart+Tracer](https://github.com/seongyeon1/Repeat_Buyer_Prediction/assets/83098550/0ec83a8f-4ac6-44e0-b9f6-8524d996c84c)

## 🏆 최종결과
- XGBoost와 CatBoost를 활용한 모델링을 통해 재구매 확률 예측 성능을 개선. AUC 0.69 달성, 글로벌 대회 73위 기록
- 캡스톤 디자인 본선 진출 및 부스 참여
