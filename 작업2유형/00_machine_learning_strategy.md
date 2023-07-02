# 1. 머신러닝의 종류

머신러닝은 크게 3가지 종류로 나눌 수 있다.

1. **지도 학습**

   - 분류 분석

   - 회귀 분석

2. **비지도 학습**

   - 차원 축소
   - 군집화
   - 연관성 규칙 발견

3. **강화 학습**

그리고 이러한 머신러닝을 쉽게 할 수 있도록 도와주는 라이브러리인 **sklearn**이 있다.

<br>

# 2. SciKit-learn

사이킷런의 주요 모듈로는 다음과 같은 것들이 있다.

- **데이터 분리, 검증, 파라미터 튜닝**
  - `sklearn.model_selection`
- **피쳐 처리**
  - `sklearn.preprocessing`
  - `sklearn.feature_selection`
  - `sklearn.feature_extraction`
- **피쳐 처리 및 차원 축소**
  - `sklearn.decomposition`
- **머신러닝 알고리즘**
  - `sklearn.ensemble`
  - `sklearn.linear_model`
  - `sklearn.naive_bayes`
  - `sklearn.neighbors`
  - `sklearn.svm`
  - `sklearn.tree`
- **평가**
  - `sklearn.metrics`
- **유틸리티**
  - `sklearn.pipeline`

<br>

그리고 어떤 머신러닝 알고리즘을 어떤 것을 골라야 할지 모르겠다면 사이킷런의 공식 지침을 따르면 좋을 것 같다.



![Move mouse over image](01_machine_learning_strategy/ml_map.png)

<br>

# 3. Machine Learning Process

머신러닝을 수행하는 데에 있어 개인차가 있겠지만, 나는 그동안 다음과 같은 프로세스로 진행해왔으며, 이번 시험 또한 이렇게 진행해보려고 한다.

1. **데이터 탐색적 분석(EDA)**
   - 데이터 타입 확인
   - 결측치 확인
   - 이상치 확인
2. **데이터 전처리**
   - 학습에 사용할 수 있도록 int, float 형식으로 인코딩
   - `LabelEncoder`, `OneHotEncoder`, `pd.get_dummies`, `astype('category').cat.codes`
3. **데이터 분할(훈련/검증)**
4. **모델 준비**
   - **분류**
     - DecisionTreeClassifier, RandomForestClassifier, XGBClassifier, KNeighborsClassifier,  CatBoostClassifier, LGBMClassifier
   - 회귀
     - LinearRegression, CatBoostRegressor, LGBMRegressor
5. **모델 학습(훈련 데이터)**
6. **예측(검증 데이터)**
7. **모델 평가**
8. **모델 선택 및 활용**



# 참고

- [Choosing the right estimator](https://scikit-learn.org/stable/tutorial/machine_learning_map/index.html)