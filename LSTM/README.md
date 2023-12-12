# LSTM
예측할려는 window 구성 데이터와 예측 데이터의 수가 동일해야 한다.
## 시계열 예측

### [lstm_tensorflow](https://github.com/stockmanager1/-_-/blob/main/LSTM/lstm_tensorflow.ipynb)

tensorflow를 사용해서 lstm을 구축하고 주식 가격을 예측하는 코드

데이터 셋 크기 : 2933*1

### [제주_특산물_가격_예측_AI_경진대회_lstm](https://github.com/stockmanager1/-_-/blob/main/LSTM/%EC%A0%9C%EC%A3%BC_%ED%8A%B9%EC%82%B0%EB%AC%BC_%EA%B0%80%EA%B2%A9_%EC%98%88%EC%B8%A1_AI_%EA%B2%BD%EC%A7%84%EB%8C%80%ED%9A%8C_lstm.ipynb)

tensorflow로 lstm을 구축하고 제주_특산물_가격_예측_AI_경진대회의 데이터를 이용해서 모델을 구축. 근데 정확도가 너무 떨어진다. 스케일링 부분에서 좀 문제가 생겼거나 모델의 특성인거 같다. 보면 스케일링을 안하면 학습 과정에서 문제가 생기고 스케일링을 하고 학습을 하면 학습은 어느정도 진행되는데 다시 스케일을 복원하는 과정에서 너무 성능차이가 심하다. 이게 약간 카테고리 변수가 많으면 많을수록 성능하락에 큰 영향을 끼치는 것 같은데, 이래서 시계열 모델이 딥러닝을 사용해도 머신러닝보다 퍼포먼스가 약하다는 것을 다시 한번 더 상기하게 되었다.

자세한 코드 리뷰는 velog에 진행할 예정이다.

### [에코프로](https://github.com/stockmanager1/-_-/blob/main/LSTM/%EC%97%90%EC%BD%94%ED%94%84%EB%A1%9C%EB%A5%BC_lstm%EC%9C%BC%EB%A1%9C_%EC%98%88%EC%B8%A1%ED%95%98%EB%8A%94_%EC%BD%94%EB%93%9C.ipynb)
에코프로 가격을 예측하는 lstm 모델. 근데 급등주는 시간의 정형성에서 벗어나, 예측이 상당히 어려운 것을 알 수 있다.

### [서울시_평균_기온_예측_해커톤](https://github.com/stockmanager1/-_-/blob/main/LSTM/%EC%84%9C%EC%9A%B8%EC%8B%9C_%ED%8F%89%EA%B7%A0_%EA%B8%B0%EC%98%A8_%EC%98%88%EC%B8%A1_%ED%95%B4%EC%BB%A4%ED%86%A4_lstm.ipynb)
12월 12일 기준으로 31등이다. 생각보다 성능이 떨어짐.
