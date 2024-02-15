# Google Brain - Ventilator Pressure Prediction for Kaggle Project


구성원 : 김경은, 김영우, 이현희, 최종수

카테고리: 의료 (시계열 예측 / 정형데이터 회귀)

주제 :  Google Brain - Ventilator Pressure Prediction 

목표 :  인공호흡기의 압력을 예측

# **Title Name :  인공호흡기 압력예측**

<p style="font-weight:bolder; font-size : 21px">
    Step : 문제해결프로세스 [step:1]
<p>
<p style="font-weight:bolder; font-size : 21px">
   RegDate : 2023.11.07
<p>

------------------------------------------------------------


# 1. 개요




> 설명

```
환자 맞춤형 호흡 지원의 개선과
호흡기 제어방법의 비용을 감소하기 위해
인공호흡기의 압력을 예측할 필요가 있음
이를위해
```
**딥러닝을 이용하여 인공호흡기의 압력을 예측할 예정**

[링크 : Google Brain - Ventilator Pressure Prediction](https://www.kaggle.com/c/ventilator-pressure-prediction)


# 2. 데이터 피쳐 상세


| 피쳐          | 설명                                                |
|---------------|-----------------------------------------------------|
| id            | time step 기반 식별자                               |
| breath_id     | 호흡에 대한 식별자                                  |
| R(resistance) | 폐의 입구크기(저항성:공기를 많이받냐,적게받냐)      |
| C(Compliance) | 폐의 최대용량(순응성:호흡이들어갈수있는크기의한계)  |
| time_step     | 실제 시간 기록                                      |
| u_in          | 공기 입력값 0~100                                   |
| u_out         | 흡기/배기 여부 0~1 (0은흡기,1은배기)                |
| `pressure`    | `폐의압력, cmH2O 단위로 측정`                       |


# 3. 문제해결 프로세스 정의


> **문제정의**

```
    호흡기 제어 패턴에 따른 분석이
    기존의 알고리즘에서 파악하기 어려운듯함
```
> **기대효과**

```
    비용감소와 맞춤형 호흡기 지원
```

> **해결방안**

```
    호흡관련 피쳐의 분석을 통해 기도압(pressure)를 예측

        + Session 1
          - Data 전처리 및 EDA
        
        + Session 2
          - 가설을 수립하고 데이터를 통해 검증
        
        + Session 3
          - MLP,LSTM 등등 여러 적합한 모델을 활용하여 기도압(pressure)예측 모델링 수행
```

> **성과측정**  

```
    모델 활용 전/후 채용 프로세스 진행 속도 비교
```
