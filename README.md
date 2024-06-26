
# 서론
이태원 압사 사고로 많은 생명을 잃었습니다.  
이 사건을 감정적 / 정치적인 견해는 제외하고 데이터를 통해 살펴보고 싶어졌습니다.

---

## 프로젝트 개요
공공 데이터 / 서울시 오픈 데이터를 바탕으로 인구의 밀집에 대한 적절한 조사를 진행하려고 합니다.  

---

## 지표 생성
- 서울교통공사 지하철 일별 / 역별 / 시간대별 승하차 인원
    - 지하철 평균하차 대비 최대하차 지표
        - 지하철역을 행정동으로 변경하여 사용

- 소상공인시장진흥공단 상가(상권)정보    
    - 상권 (술집, 주점) clustering
    - cluster별 표준편차, 밀도, 타 군집과의 거리

- 서울특별시 행정동별 서울생활인구
    - 행정동별 평균 생활인구 대비 최대 생활인구 지표

---

### 소상공인시장진흥공단 상가(상권)정보

- 상권 clustering 후 cluster 별 특징. (44개 상권 중 6위)

![image](README_ASSETS/final_market_score.png)

---

### 서울특별시 행정동별 서울생활인구

- 행정동별 평균 생활인구 대비 최대 생활인구 지표 (180개 행정동 중 1위)

![image](README_ASSETS/final_population_score.png)

---

## 지표 합산

- 이태원의 특이점

![image](README_ASSETS/final.png)

---

### 프로젝트에 알고 싶은 것

1. `한번도 일어나지 않은 일을 예측하는 것`은 가능한가?   
`신`과 같은 존재가 "올해 압사사고가 있을 것이다."라는 언급을 해주었다면 가능 할 것 같습니다.   
그렇다면 '여의나루 / 이촌의 불꽃축제' / '이태원 할로윈' 둘 중 하나일 것이 분명할 것입니다.   
하지만 일반적으로 이태원의 압사사고를 예측하는 것은 어려운 일인 것 같습니다.


2. `데이터로 볼 때 사고가 일어날 만한 이상치`에 있는 상황이었나?   
확실히 데이터로 볼 때 이태원의 할로윈은 특이한 부분이 많습니다.   
- 이태원
    - 이태원보다 더 혼잡한 / 밀도 높은 사건과 공간이 존재한다. (ex. 여의도 불꽃축제)
        - 하지만 불꽃축제는 주최자가 존재한다.
        - 술집 상권이 아니다.
    - 이태원보다 더 고립되어있는 상권이 존재한다.
        - 하지만 이태원 할로윈 처럼 특수성을 가지며 고립된 상권은 없다.
