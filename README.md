# 🏆 ML 미니 프로젝트 1팀

## 1. 프로젝트 주제 및 배경
- **주제**: (여기에 주제를 적어주세요)
- **주제 선정 배경**: (비용 절감, 문제 해결 등 선정 이유를 적어주세요)

## 2. 데이터셋 개요 및 전처리
- **데이터셋 정보**: (데이터 출처, 행/열 개수 등)
- **전처리 과정**: (EDA 단계와 머신러닝 단계의 차이점을 간략히 기술)

## 3. 모델링 및 성능 평가
- **사용한 모델**:LightGBM
- **성능 향상을 위한 노력**: (optuna 활용 최적의 하이퍼파라미터 활용)
- <img width="726" height="425" alt="1  lightGBM 하이퍼파라미터" src="https://github.com/user-attachments/assets/57d3c10a-1f44-4179-82d1-90ed6d306d89" />

- **최종 모델 및 성능 결과**: (정확도, F1-score 등)
## 4. 실제 예측 결과 및 기대 효과
- **예측 결과**: (최종 선택 모델의 예측 결과 요약)
**애들이 작성한 표 추가 및 해석**
  **ROC Curve**
  <img width="699" height="551" alt="2  lightXGB_ROC_curve" src="https://github.com/user-attachments/assets/f5da1754-31cf-434a-abf0-b1e738107358" />

  **Feature importance** 
<img width="791" height="544" alt="3  Feature Importances (LightGBM)" src="https://github.com/user-attachments/assets/3d6db174-5d8a-46a3-b08e-3905ab9af392" />

- **기대 효과**: (머신러닝 도입에 따른 기회비용 절감 및 기대 효과)

---
### 📂 폴더 구조 안내
- **data/**: 데이터셋 파일 (raw, processed)
- **notebooks/**: EDA 및 실험용 주피터 노트북
- **src/**: 실제 실행용 파이썬 코드
- **models/**: 학습된 모델 저장 (.pkl, .h5 등)
