# Stopickr - 주식 거래를 위한 Deep Q-Learning 에이전트

## 개발 기간
2024. 6. 1. ~ 2024. 12. 8.


딥 Q-Learning 기반 인공지능을 활용하여, 주식 거래 시 최적의 투자 결정(매수/매도/보유)을 내리는 AI 에이전트를 개발하고 웹 서비스로 제공하는 프로젝트입니다.


## 소개

주식 시장의 복잡성과 불확실성을 효과적으로 다루기 위해 딥 Q-Learning 알고리즘을 활용한 AI 거래 에이전트를 개발합니다.

딥 Q-Learning은 강화학습의 일종으로, 심층 신경망을 통해 상태(주식 시장 데이터)에 따른 최적의 행동(매수, 매도, 보유)을 학습합니다


- 데이터 수집 및 전처리: FinanceDataReader를 활용한 주식 데이터(개장가, 최고가, 최저가, 종가, 거래량) 수집과 뉴스 데이터 감성 분석을 통합하여 AI 모델의 입력으로 사용합니다. 수집된 데이터는 정규화를 통해 동일한 스케일로 조정됩니다.

- 모델 개발 및 학습: 시간 창(window-size) 기반으로 상태를 정의하고, DNN을 활용하여 Q-Network를 구성합니다. Epsilon-Greedy 알고리즘을 통해 탐험(무작위 행동 선택)과 활용(학습된 최적 행동 선택) 사이의 균형을 유지하며 학습을 진행합니다. 배치 학습을 통해 데이터 효율성을 높이고 일반화 능력을 향상시킵니다.

- 성능 평가 및 최적화: 학습에 사용되지 않은 테스트 데이터셋을 활용하여 모델의 성능을 평가하고, 실제 시장 상황에서의 수익률을 측정합니다. 필요에 따라 하이퍼파라미터를 조정하여 성능을 최적화합니다.

- 기존의 단순한 패턴 인식 방식이 아닌, 강화학습을 통해 시장 환경의 변화에 적응하는 지능형 시스템을 구현함으로써 보다 안정적이고 수익성 높은 투자 의사결정을 지원합니다. 이는 개인 투자자에게 전문적인 분석 도구를 제공하고, 금융 분야에서 AI 기술의 실용적 활용 가능성을 보여주는 의미가 있습니다.


## 주요 기능
### 핵심 기능

- 딥 Q-Learning 기반 주식 거래 의사결정(매수/매도/보유) 추천
- 과거 주가 데이터 분석을 통한 시장 예측 
- 현재 주식 시장 상황 및 대표 지수 분석 제공
- 인기 종목 및 거래량 많은 주식 정보 제공
- AI 모델이 추천한 종목의 수익률 분석 및 표시


## 기술 스택
### 클라이언트
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Next JS](https://img.shields.io/badge/Next-black?style=for-the-badge&logo=next.js&logoColor=white)
![Styled Components](https://img.shields.io/badge/styled--components-DB7093?style=for-the-badge&logo=styled-components&logoColor=white)


### 서버
![Django](https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white)
![AWS Lambda](https://img.shields.io/badge/AWS%20Lambda-FF9900?style=for-the-badge&logo=aws-lambda&logoColor=white)
![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)


### 인프라/플랫폼
![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)
![OAuth 2.0](https://img.shields.io/badge/OAuth%202.0-31A8FF?style=for-the-badge&logo=oauth&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)


### 데이터
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)


### AI/ML
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)


### 제품/서비스
![Notion](https://img.shields.io/badge/Notion-%23000000.svg?style=for-the-badge&logo=notion&logoColor=white)
![Figma](https://img.shields.io/badge/figma-%23F24E1E.svg?style=for-the-badge&logo=figma&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
