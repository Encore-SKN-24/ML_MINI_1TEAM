# 🏆 ML 미니 프로젝트 1팀

## 1. 프로젝트 주제 및 배경
- **주제**: (여기에 주제를 적어주세요)
- **주제 선정 배경**: (비용 절감, 문제 해결 등 선정 이유를 적어주세요)

## 2. 데이터셋 개요 및 전처리
- **데이터셋 정보**: (데이터 출처, 행/열 개수 등)
- **전처리 과정**: (EDA 단계와 머신러닝 단계의 차이점을 간략히 기술)

## 3. 모델링 및 성능 평가
- **사용한 모델**: Decision Tree, Logistic Regression, XGBoost 등
- **성능 향상을 위한 노력**: (하이퍼파라미터 튜닝, 특성 공학 등)
- **최종 모델 및 성능 결과**: (정확도, F1-score 등)

## 4. 실제 예측 결과 및 기대 효과
- **예측 결과**: (최종 선택 모델의 예측 결과 요약)
- **기대 효과**: (머신러닝 도입에 따른 기회비용 절감 및 기대 효과)

<img width="731" height="333" alt="image" src="https://github.com/user-attachments/assets/35231abd-31c1-4755-a780-99cda409cbcc" />

<img width="705" height="553" alt="gb_roc" src="https://github.com/user-attachments/assets/0b495d3b-caf3-45f4-ae82-658aa3140046" />
  
<img width="784" height="584" alt="gb_ftimportance" src="https://github.com/user-attachments/assets/6e919e0c-06e4-46f4-ac75-ffcad7c6f02b" />



---
### 📂 폴더 구조 안내
- **data/**: 데이터셋 파일 (raw, processed)
- **notebooks/**: EDA 및 실험용 주피터 노트북
- **src/**: 실제 실행용 파이썬 코드
- **models/**: 학습된 모델 저장 (.pkl, .h5 등)



## eda 부분 재훈님 그래프 다음에 와야 해요!!
![산불 상관관계 히트맵](https://github.com/user-attachments/assets/8653d96c-532a-49f1-93e3-1e12b59efb41)

- 산불발생은 실효습도와 약한 음의 상관관계를 가짐
- 밭_비율과는 약한 양의 상관관계를 가짐
- 평균기온, 일강수량, 풍속 등과는 거의 상관관계가 없음

