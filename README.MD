# Google Brain - Ventilator Pressure Prediction for Kaggle Project


구성원 : 김경은, 김영우, 이현희, 최종수

카테고리: 의료 (시계열 예측 / 정형데이터 회귀)

주제 :  Google Brain - Ventilator Pressure Prediction 

목표 :  인공호흡기의 압력을 예측

## 데이터 피쳐 상세

| 피쳐 | 설명 |
| --- | --- |
| id | time step 기반 식별자 |
| breath_id | 호흡에 대한 식별자 |
| R(resistance) | 폐의 입구크기(저항성:공기를 많이받냐,적게받냐) |
| C(Compliance) | 폐의 최대용량(순응성:호흡이들어갈수있는크기의한계) |
| time_step | 실제 시간 기록 |
| u_in | 공기 입력값 0~100 |
| u_out | 흡기/배기 여부 0~1 (0은흡기,1은배기) |
| pressure | 폐의압력, cmH2O 단위로 측정 |