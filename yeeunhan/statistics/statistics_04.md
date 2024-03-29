# statistics_04

## 복습테스트

1. "주연 배우의 연기력"이 "영화의 흥행"에 영향을 준다는 모형을 만들어 데이터를 분석하려고 합니다. 여기서 **독립변수**는 무엇인가요? *

    **주연배우의 연기력**

2. "지원자의 실력"이 "합격 확률"에 영향을 준다는 모형을 만들어 데이터를 분석하려고 합니다. 여기서 **종속변수**는 무엇인가요? *

    **합격 확률**

3. 다음 중 **선형 모형의 식**을 골라 보세요. *

**y = ax + b**

4. **선형 모형의** 식에서 **파라미터**에 해당하는 것을 ****모두**** 골라 보세요 *

**a, b**

5. **선형 모형**에 대한 설명으로 올바른 것을 ****모두**** 골라보세요. *

**그래프로 그리면 x와 y의 관계가 직선의 형태가 된다**

**y의 범위가 무한대다**

**y의 예측값과 실제값의 MSE를 구할 수 있다**

6. 다음 중 **로지스틱 선형 모형의 식**을 골라 보세요. *

**y = expit(ax + b)**

7. **로지스틱 선형 모형**의 식에서 **파라미터**에 해당하는 것을 ****모두**** 골라 보세요 *

**a, b**

8. **로지스틱 선형 모형**에 대한 설명으로 올바른 것을 ****모두**** 골라 보세요. *

**그래프로 그리면 x와 y의 관계가 그림처럼 s자 곡선을 그린다**

**x의 범위는 무한대지만 y는 0에서 1사이의 범위를 갖는다 (그림 없음)**

**y는 확률로 해석할 수 있다 (그림 없음)**

**y의 실제값과 예측된 확률을 이용해서 우도를 구할 수 있다 (그림 없음)**

9. **MSE**에 대한 설명으로 올바른 것을 ****모두**** 골라 보세요 *

**오차(Error)를 제곱(Squared)한 것을 평균(Mean)낸 것이다.**

**제곱 대신 절대값(Absolute value)을 사용하면 MAE가 된다**

**파라미터를 추정할 때는 MSE를 가장 작게 만드는 파라미터를 찾는다**

**선형 모형에서 MSE를 가장 작게 만드는 파라미터는 항상 하나가 존재한다**

10. **우도**에 대한 설명으로 올바른 것을 ****모두**** 골라 보세요. *

**우도는 영어로 likelihood이다**

**우도는 모형과 파라미터를 가정했을 때 현재 가진 데이터를 관찰할 확률이다.**

**우도를 최대로 만드는 파라미터를 찾는 방법을 최대우도법(Maximum Likelihood)라고 한다**

11. 다음 각 문제를 분석하려고 할 때, **"선형 모형"과 "로지스틱 선형 모형"** 중 더 적절한 모형을 고르세요. *

배우의 연기력이 영화를 관람한 관객수에 미치는 영향 (**선**

담당 직원의 친절도가 고객의 재구매 여부에 미치는 영향 (**로**

고객의 나이와 성별이 구매 액수에 미치는 영향 (**선**

환자의 생활습관과 의사의 실력이 질병의 회복 여부에 미치는 영향 (**로**

# 통계04file.

## 신뢰구간

- 오차의 추정치 범위

### 표본분포 : 샘플링의 분포 (smapling distribution)

- 샘플을 할 때마다 값이 달라지는 데, 그거의 분포는?
- 모분포(엄마 분포) → 샘플링을 할때마다 한번씩 뽑는 거를 smapling이라 하고, 이 작업을 하면 sample이 여러개가 나옴.
- 모분포는 균등분포라서 데이터가 0-100사이 고르게 나옴. 그러니까 샘플들도 대체로 완전 고르지는 않지만 대체로 고르게 나옴.
- 그래서 샘플들을 표본분포 해보면 대체로 50주변에 몰려있는 값이 나옴.
- 동일한 분포에서 같은 크기의 표본(sample)을 추출
- 각 표본에서 통계치(예: 평균, 중간값 등)를 추정
- 표본 분포: 추정된 통계치의 분포
- sampling 분포 ≠ sample 분포
- 샘플링분포의 95% 신뢰구간

## 신뢰구간

- 현실에서 우리가 가진 것은 하나의 표본(샘플)
- 중심극한정리에 따라 표본 평균의 분포를 알 수 있음
- 95% 신뢰구간 = 95%의 표본들에서 평균이 어느 범위에 있는가?

## bootstrapping

- 표본에서 다시 표본을 재추출(resample)하는 방법
- 표본이 모집단 분포를 잘 반영할 경우
- 비모수적(non-parametric)
- 노트 필기 참조

### 데이터 희망편

- 데이터의 존재 이유 중 하나 → 의사결정을 돕기 위해

- **만약 계수가 - 와 + 범위값이라면? 달라짐: -구간인 경우에는 속도가 빨라지면 제동거리가 줄어든다/ 반대로 +의 값에선 속도가 증가 할때 제동거리도 증가한다. -> 엇갈리는 결론이 나옴.**
- **결국, +로 일정하게 나오거나 -로 일정하게 나오면 결론은 같고 차이만 존재하지만,**
- **+-가 같이 나오면 결론이 달라짐 : 결국 action을 취할 수 없다 (해석할 수 없다) :**
    - 근데 참고! 절편은 +-가 같이 나와도 별로 상관없음 중요한건 a임

    **데이터를 더 모아야한다 (데이터를 많이 모을수록 신뢰구간이 줄어든다 -> 같은 범위 값을 가진다)**

- **데이터를 많이 모으면 신뢰구간이 줄어든다**
- **작은 sample: 신뢰구간이 길다 -> 리샘플링을 많이 한다 :**

    **신뢰구간을 정확하게 만들기 위해서지 좁아지는 건 아니다**

- **큰 smaple : 신뢰구간이 짧다**

### **신뢰구간에 정답이 있을까?**

- 있다! 모분포를 무한히 smapling 하면 됨 ㅎㅎ
- sample 적당히 많이 smapling (이게 바로 부드스트래핑)
- 실제로는 데이터를 많이 모으면 더 넓어지는 쪽으로 신뢰구간이 길어지면서 정확해진다.

    (나오는 데이터가 많으니까..!)

- 헷갈리는 점! 신뢰구간이 좁아져야 좋고(중요), 그러면서 신뢰구간이 정확해야 한다고 한다.
- 근데 샘플이 크면 실제 신뢰구간이 좁고, 리샘플링을 많이 할수록 데이터가 많아지니까 추정된 신뢰구간이 넓어진다(그러면서 정확해짐) 요 부분이 헷갈림
- **그러니까 결론! 샘플은 커야하고, 리샘플링은 많이 할수록 좋다**
- 샘플을 키워야 현실(실제) 데이터가 바뀌고, 리샘플링은 추정치 값이 달라지는 거.

### 얼마나 많이 데이터를 모아야할까?

- 내가 원하는 신뢰구간의 범위(좁아지는)가 나올 때까지 모아야 함! : **신뢰 구간이 충분히 좁아질** 때까지
- 그래서 신뢰 구간이 중요하다. 샘플을 얼마나 모아야 할 지의 지표가 된다.

# 정리

1. 신뢰구간의 범위가 좁을 수록, 의사결정하기가 수월하다  +  Resampling을 많이 할 수록 좋다 
2. 신뢰구간의 범위가 좁다는 의미? → 최소한 -와 +가 바뀌지는 않은 정도 

    (같이 존재하면 결론이 바뀌니까 어려움ㅎ) 

    ex) 포도주와 건강의 관계 : 1년 전 기사 '포도주 마시면 건강에 도움된다' 오늘 기사 '포도주 마시면 건강에 해로워,,,,'

3. sample은 클수록 좋다. 더 많이 모아야 한다. 
4. sample이 얼마나 커야할까? 신뢰구간이 충분히 좁혀질만큼! 

- 다시 슬라이드

# 파라미터 추정 = fit

# 과적합 (overfitting)

- 현재 가진 표본에 지나치게 치우친 추정을 하는 것
- 실제 분포와 거리가 있어 예측력이 떨어진다
- ex) 가진 샘플에 비해서 너무 많은 파라미터가 존재하는 경우

    → 신뢰구간이 넓어지게 됨 = 샘플마다 다른 값을 가진다 = 모분포와 달라진다 

- 선형 모형을 통계에서 자주 쓰는 이유
    - 과적합될 확률이 적다. (파라미터가 a와 b만 존재해서 단순)

# 교차검증

- 과적합을 방지/ 내가 특정 샘플에만 치중해서 예측한 거 아닌가?
- 다른 샘플을 가지고 확인해보자 → 가지고 있는 데이터를 쪼개서 검증
- 현재 데이터를 training set와 test set으로 무작위 분할
- training set으로 추정
- test set으로 테스트
- 과적합이 있을 경우 training set에 비해 test set의 예측이 떨어짐

# 정규화

- 과적합을 방지하는 방법들

    1) 파라미터를 줄이는 방법 → 어떻게 적게 잡냐? (나중에 두둥) 

    2) 일반적으론 선형모형을 쓴다 

    3) 과도한 추정치에 페널티를 부과한다 

    - a가 100,1000 이러면 과도한 추정치일 가능성이 크다.
    - 커지면 커질 수록 패널티 부여 (수학적 트릭)

    4) 추정을 조기에 중단한다 

    - 내가 가진 샘플이 치우쳐서 모집단 이랑 좀 다르다 그럼 파라미터 추정이 이상해짐
    - 그래서 일찍 멈춘다 (그래서 샘플에는 잘 안 맞지만, 모집단하곤 맞음)
    - 그래서 모집단에 가까운 초기값을 잡아야 함. 어떻게? (나중에 두둥2)