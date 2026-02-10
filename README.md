# 🏆 ML 미니 프로젝트 1팀

## 1. 프로젝트 주제 및 배경
- **주제**: (여기에 주제를 적어주세요)
- **주제 선정 배경**: (비용 절감, 문제 해결 등 선정 이유를 적어주세요)

## 2. 데이터셋 개요 및 전처리
- **데이터셋 정보**: (데이터 출처, 행/열 개수 등)
- **전처리 과정**: (EDA 단계와 머신러닝 단계의 차이점을 간략히 기술)

- **변수 정리**
## 📊 주요 파생 변수 및 생성 근거

산불 발생의 주요 원인이 인적 실화와 소각 행위라는 점에 착안하여, 아래 3가지 정적 데이터를 변수로 추가하였음

### 1. 도시 산림 인접 비율 (WUI, Wildland-Urban Interface)
* **산출 방식:** $\frac{\text{지역별 산림 면적}}{\text{지역 전체 면적}} \times \text{인구 밀도}$
* **설명:** 지역의 산림(연료) 비율과 인구 밀도를 결합해, **사람이 산림 연료와 접하는 잠재적 강도(WUI 성격)**를 연속형 지표로 나타냄
값이 클수록 지역 면적 대비 산림 비중이 높고 인구가 밀집한 지역으로, 산불 발생이 상대적으로 높을 수 있음

* **근거:** 
"Stewart et al.(2007)은 WUI를 40에이커당 택지 1개 이상인 지역 중에서, 아래 둘 중 하나를 만족하는 곳으로 정의함
<table border="1" cellspacing="0" cellpadding="8">
  <thead>
    <tr>
      <th>구분</th>
      <th>정의</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>혼합형 WUI</td>
      <td>야생 식생이 전체 면적의 50% 이상인 지역</td>
    </tr>
    <tr>
      <td>접경형 WUI</td>
      <td>야생 식생이 50% 미만이더라도, 1.5마일 이내에 야생 식생 75% 이상으로 덮인 1,235에이커 이상의 대규모 지역이 인접한 경우</td>
    </tr>
  </tbody>
</table>

- **본 프로젝트에서는 WUI 개념을 반영하여, 지역 단위에서 산림 비중과 인구밀도를 결합한 연속형 지표를 사용하였음**
출처 : 안현진·정도채·김동욱·정호근. (2024.12). 산림 인접지역의 효과적 산불 관리를 위한 개선과제(연구보고서 R 2024-19). [한국농촌경제연구원].

### 2. 논 비율 & 3. 밭 비율 (Agricultural Ratio)
* **산출 방식:** $\frac{\text{지역별 논(밭) 면적}}{\text{전국 논(밭) 총 면적}}$
* **설명:** 지역의 농지 면적 비율을 나타낸다.
* **근거:** 최근 10년간 산불 원인 통계에 따르면 **논·밭두렁 소각(11.0%)**과 쓰레기 소각(12.4%) 등 소각 행위가 전체 산불 원인의 큰 비중을 차지함. [출처 : *2025년 산불 제대로 알기*]

---

## 📈 산불 발생 원인 통계 (Reference)

국립산림과학원 자료에 따르면, 전체 산불의 절반 이상이 사람에 의한 실화 또는 소각 행위로 발생하고 있습니다. 본 모델은 이러한 '인적 요인'을 정량화하여 예측에 반영함

<div align="center">
  <img src="https://github.com/user-attachments/assets/d375fe72-0f3c-4652-819a-386fb33750c1" alt="월별 원인별 산불발생 현황" width="600">
  <p><i>출처: [국립산림과학원] 2025년 산불 제대로 알기(수정본)</i></p>
</div>

---

## 📂 데이터 출처 및 참고 문헌
* **기상 데이터:** 기상청 공공데이터포털
* **산불 원인 통계 및 분석 논리:** 국립산림과학원(NIFoS), *2025년 산불 제대로 알기*
* **지리 데이터:** 통계청 시도별 행정구역 및 지목별 면적 통계
- 출처 :


[전국(도별) 논밭별 경지면적] https://kosis.kr/statHtml/statHtml.do?sso=ok&returnurl=https%3A%2F%2Fkosis.kr%3A443%2FstatHtml%2FstatHtml.do%3Fconn_path%3DI3%26tblId%3DDT_1EB001%26orgId%3D101%26


[산림면적] https://kosis.kr/statHtml/statHtml.do?sso=ok&returnurl=https%3A%2F%2Fkosis.kr%3A443%2FstatHtml%2FstatHtml.do%3Fconn_path%3DI2%26tblId%3DDT_11001N_2013_A022%26orgId%3D110%26


[인구밀도(인구주택총조사기준) - 시도] https://kosis.kr/statHtml/statHtml.do?sso=ok&returnurl=https%3A%2F%2Fkosis.kr%3A443%2FstatHtml%2FstatHtml.do%3Fconn_path%3DMT_ZTITLE%26list_id%3DA1_13%26obj_var_id%3D%26seqNo%3D%26tblId%3DDT_1B08024%26vw_cd%3DMT_ZTITLE%26itm_id%3D%26language%3Dkor%26lang_mode%3Dko%26orgId%3D101%26

## 3. 모델링 및 성능 평가
- **사용한 모델**: XGBoost

<div align="left">
  <img src="https://github.com/user-attachments/assets/beee3c97-fa17-4593-bffc-dad1c045ad1a" alt="auc-roc와 혼동행렬" width="600">
  <p><i>auc-roc와 혼동행렬</i></p>
</div>

- **성능 향상을 위한 노력**: 

smote로 산불이 1이 되는 값을 임의로 늘렸다. 그러나 precision이 낮게 나왔음
<div align="left">
  <img src="https://github.com/user-attachments/assets/fcf20cc6-a62b-4794-b0ec-820573ccff57" width="600">
</div>

이후에 scale_pos_weight를 사용하여 하이퍼 파라미터 탐색

<div align="left">
  <img src="https://github.com/user-attachments/assets/8e39b9cc-9f40-4169-a954-0a50d33a7555" width="600">
</div>





- **최종 모델 및 성능 결과**:
- <table border="1" cellspacing="0" cellpadding="8">
  <thead>
    <tr>
      <th>모델</th>
      <th>train/test 점수</th>
      <th>정확도(Accuracy)</th>
      <th>재현율(Recall)</th>
      <th>정밀도(Precision)</th>
      <th>f1 score</th>
      <th>ROC-AUC</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>XGboost(smote)</td>
      <td>0.81/0.81</td>
      <td>0.81</td>
      <td>0.81</td>
      <td>0.28</td>
      <td>0.42</td>
      <td>0.90</td>
    </tr>
    <tr>
      <td>XGboost(scale_pos_weigh)</td>
      <td>0.96/0.91</td>
      <td>0.91</td>
      <td>0.65</td>
      <td>0.47</td>
      <td>0.54</td>
      <td>0.90</td>
    </tr>
  </tbody>
</table>


## 4. 실제 예측 결과 및 기대 효과
- **예측 결과**: (최종 선택 모델의 예측 결과 요약)
- **기대 효과**: (머신러닝 도입에 따른 기회비용 절감 및 기대 효과)

---
### 📂 폴더 구조 안내
- **data/**: 데이터셋 파일 (raw, processed)
- **notebooks/**: EDA 및 실험용 주피터 노트북
- **src/**: 실제 실행용 파이썬 코드
- **models/**: 학습된 모델 저장 (.pkl, .h5 등)

## 4. 한계점
- 도시 산림 인접 비율은 시내에 인구가 밀집되어 있을 수 있다는 한계점이 있을 수 있음 

## 5. 한줄 회고
박수영 : 모델 학습을 하면서, 일차적으로 회귀인가 분류인가 하는 문제에 직면했고, 모델을 선택한 이후에도 하이퍼 파라미터를 조정하는 과정이 어려웠다. 특히 모델을 만들고 내가 예측하려는 산불이 
정확도보다는 재현율이 중요하기 때문에, recall을 높여야 한다는 것, 점수가 높지 않게 나와 GridSearchCV를 사용했는데, 너무 오래 걸려서 결국에 RandomizedSearchCV를 사용해서 최적의 파라미터를 찾았다.
상황에 따라, 또 목적에 따라서 모델 이외에 부수적인 것들의 선택지가 다양하다는 것을 이론 이외에 실제로 느꼈다.
