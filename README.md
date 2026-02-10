# 1. 프로젝트 소개

##  **주제: ML 모델 기반 산불 발생 예측**
### **기간: 2026년 2월 4일 ~ 2026년 2월 11일**
### **팀명: 🏆 ML 미니 프로젝트 1팀**


 
### **팀원 소개**
 
| <img src="https://github.com/user-attachments/assets/192cc577-c7ac-49a9-9855-2230cd1cc55c" width="150" height="150"> | <img src="https://github.com/user-attachments/assets/3cb641b2-cfc5-4c3a-a10a-e0222ef9c673" width="150" height="150"> | <img src="https://github.com/user-attachments/assets/a60d634f-6fba-4cfb-b74e-b56d6be3f358" width="150" height="150"> | <img src="https://github.com/user-attachments/assets/a32be587-2de6-4884-8f66-0a4b303dfe53" width="150" height="150"> | <img src="https://github.com/user-attachments/assets/a367b378-429e-4117-85fa-bd968867ee28" width="150" height="150"> |
|:---:|:---:|:---:|:---:|:---:|
| **고아라** | **정재훈** | **김은우** | **나혜린** | **박수영** |
|  [![github - Akoh-0909](https://img.shields.io/badge/Akoh--0909-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Akoh-0909) | [![github - JeaHoon-J](https://img.shields.io/badge/JeaHoon--J-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/JeaHoon-J) | [![github - whitehole17](https://img.shields.io/badge/whitehole17-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/whitehole17) | [![github - ](https://img.shields.io/badge/nngpfls-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/nngpfls) | [![github - suyoung6279](https://img.shields.io/badge/suyoung6279-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/suyoung6279) |
| | | | | |


---



## **개요**

### **주제 선정 배경**: 
이전 EDA과정에서 다루었던 기상데이터를 보다 실질적인 사회적 이슈에 연결해보고자 하였으며, 단순한 상관분석을 넘어, 머신러닝을 활용하여 실제 현장에서 활용 가능한 예측 모델로 확장해 보는 것을 목표로 하였음. 

- **산불 위기대응**: 대형 산불에 대한 원인 데이터 기반의 예방 및 경보 체계 필요성 증대

- **실용적 가치**: 산불 발생 가능성을 사전에 예측하여 행정 현장의 자원 배분 및 의사 결정을 지원하고 피해를 최소화

### 🔗 News Sources
  
---

## 2. 데이터셋 개요 및 전처리
- **데이터셋 정보**: 산림청 산불 발생 공공데이터 및 관련 기상/지형 데이터 활용
- 데이터 출처:

---------------------
### 기술 스택

| 분류 | 기술/도구 |
| :--- | :--- |
| **언어** | ![Python](https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white) |
| **협업 툴** | ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white) 
| **데이터 처리** | ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
| **데이터 시각화** | ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) ![Seaborn](https://img.shields.io/badge/Seaborn-%234470AD.svg?style=for-the-badge&logo=python&logoColor=white)

-----

## **전처리 과정**: 

-EDA 단계(Before):
결측치/이상치 탐색, 기상 변수 분포·계절성 파악, 산불 발생 시기·지역 히트맵 등 현상 이해 중심의 분석 수행.

-ML 단계(After):
날짜·행정구역 기준으로 모든 데이터셋을 통합하고, 파생 변수 (실효습도, 농지비율, 도시산림 인접지수) 생성, 결측치 보간·평균 대체, SMOTE로 클래스 불균형을 보정해 모델 학습에 최적화된 형태의 피처 세트 구축


### 📋 Preprocessing Pipeline

| 번호 | 처리 내용 | 사용 데이터 | 처리 목적 | 세부 설명 |
| :--- | :--- | :--- | :--- | :--- |
| 1 | 산불 데이터 로드 | sanbul.xlsx | 산불 발생 정보 확보 | 산림청 산불 발생 원자료 로드 |
| 2 | 시도 컬럼명 통일 | 산불 데이터 | 데이터 결합 준비 | 기상 데이터와 공간 단위 통일 |
| 3 | 발생일시 생성 | 산불 데이터 | 시간 단위 정규화 | 연·월·일 컬럼 결합 |
| 4 | 산불 발생 여부 변수 생성 | 산불 데이터 | 종속변수(Y) 정의 | 발생 시 1 |
| 5 | 기상 데이터 로드 | weather CSV | 기상 변수 확보 | 기온·습도·강수·풍속 load |
| 6 | 강수량, 최심적설 결측치 처리 | 기상데이터 | 통계 신뢰성 확보 | 결측치 0으로 처리 |
| 7 | 기온, 풍속 결측치 처리 | 기상데이터 | 통계 신뢰성 확보 | 결측치 지점, 일시별 평균으로 처리 |
| 8 | 습도 결측치 처리 | 기상데이터 | 통계 신뢰성 확보 | 주변 날짜 평균으로 보간 |
| 9 | 초기 기간 데이터 보완 | 2015년 기상 | 실효습도 안정화 | 과거 습도 부족 문제 보완 |
| 10 | 공통 컬럼 추출 | 기상 데이터 | 컬럼 불일치 방지 | 공통 변수만 선택 |
| 11 | 지점·날짜 정렬 | 기상 데이터 | 시계열 정확성 | shift 계산 오류 방지 |
| 12 | 실효습도 계산 | 기상 데이터 | 파생변수 생성 | 지수 가중 이동 평균 적용 |
| 13 | 분석 기간 제한 | 기상 데이터 | 초기 결측 제거 | 2016년 이후 데이터 사용 |
| 14 | 관측소–시도 매핑 | 기상 데이터 | 공간 단위 통합 | 관측소를 시도로 변환 |
| 15 | 시도·일자별 집계 | 기상 데이터 | 대표값 생성 | 기상데이터의 평균·최대·최소 집계 |
| 16 | 산불 발생 일 집계 | 산불 데이터 | 발생 여부 정리 | 시도–일 단위 정리 |
| 17 | 시도×전체 날짜 생성 | 통합 데이터 | 패널 데이터 구축 | 산불 미발생일(0) 포함 |
| 18 | 산불 발생 여부 병합 | 통합 데이터 | 종속변수 결합 | fire=0 처리 |
| 19 | 기상 변수 병합 | 통합 데이터 | 설명변수 결합 | 시도–일 기준 병합 |
| 20 | 결측치 제거 | 통합 데이터 | 학습 데이터 정제 | 기상 결측 행 제거 |
| 21 | 지역별 논 비율 및 밭 비율 생성 | 전국(도별) 논밭별 경지면적 | 파생변수 생성 | 전국 면적으로 지역별 계산 |
| 22 | 지역별 (산림면적 / 지역면적) 계산 | 산림면적 | 파생변수 생성 | 전국 면적으로 지역별 계산 |
| 23 | ((산림면적 / 지역면적) * 인구밀도) 추가 | 인구밀도 - 시도 | 파생변수 생성 | 비율에 인구밀도 곱함 |
| 24 | 최종 데이터 저장 | CSV 파일 | 모델 입력 | 머신러닝 학습용 데이터 생성 |


----------------
## EDA
(그래프 삽입 및 해석 추가)


---------------------

## 3. 모델링 및 성능 평가 (TBD)
- **사용한 모델**: Decision Tree, Logistic Regression, XGBoost 등
- **성능 향상을 위한 노력**: (하이퍼파라미터 튜닝, 특성 공학 등)
- **최종 모델 및 성능 결과**: (정확도, F1-score 등)

---

## 4. 실제 예측 결과 및 기대 효과
- **예측 결과**:

- **기대 효과**: <br/>

(1) 선제적 대응: 산불 발생 위험도가 높은 시기를 사전에 파악하여 예방 순찰 및 인력 배치 최적화<br/>

 - 산불 예방 측면:
시·군·구별 산불 발생 확률을 사전에 제공함으로써, 고위험 지역 중심의 입산 통제·쓰레기 소각 단속·계도 활동을 효율적으로 집중할 수 있어 예방 인력·예산의 기회비용을 절감할 수 있다.

(2) 피해 감소: 데이터 기반의 경보 시스템 구축을 통해 초기 진화 성공률을 높이고 산림 자원 손실 최소화<br/>

- 초기 대응·자원 배치 측면:
소방·산림청이 고위험 지역에 인력·장비·헬기 등을 선제적으로 배치하도록 지원해, 초기 진화 성공률을 높이고 대형 산불로 확산되기 전 대응할 수 있는 기반을 제공한다.

(3) 확장성: 구축된 모델을 타 지역이나 유사 기상 재난(가뭄 등) 예측 모델로 응용 가능<br/>
- 정책·연구 확장:
본 모델 구조는 기상청 실시간 예보·위성/리모트 센싱 데이터와 결합해 실시간 산불 위험지도 서비스로 확장 가능하며, 향후 읍·면·동 단위로 해상도를 높인 고도화 모델 개발의 기초 자료로 활용될 수 있다.<br/><br/>


​

 
---

## 한계점

---

<br/>
<br/>

## 💭한 줄 회고
```
고아라
```
Keep
문서화역량: README 작성 및 발표
협업 워크플로우 준수 - Github flow 활용
Problem
데이터 정합성 검증 미흡 : 전처리 과정에서 누락된 로직을 사전에 인지하지 못한채 공유하여 데이터 파이프라인 상의 재작업 공수를 발생 시킴
에러 인지 및 디버깅 숙련도 부족: 발생한 오류의 원인을 스스로 파악하고 수정하는 단계에서 병목현상 발생
리스크 관리 부족: 초기단계에서 예견되었던 기술적 이슈에 대해 선제적으로 대응하지 못하고 반복적인 시행착오겪음
Try
전처리 검증 및 체크리스트 ( 셀프리뷰) - 데이터 전달 전 스키마 일치 여부와 결측치 확인할 수 있는 검증 스크립트나 체크리스트를 필수적으로 활용하겠음
협업 소통방식의 구체화
오류대응 프로세스 정립 - 스스로 해결할수 없는 기술적 난관에 부딪혔을때, 공식문서 확인 및 질문 가이드를 활용해 해결시간 단축 및 기술로그로 기록할 예정
```
정재훈
```
comment 작성
```
김은우
```
comment 작성
```
나혜린
```
comment 작성
```
박수영
```
comment 작성
```
<br/><br/>

---

### 📂 폴더 구조 안내
- **data/**: 데이터셋 파일 (raw, processed)
- **notebooks/**: EDA 및 실험용 주피터 노트북
- **src/**: 실제 실행용 파이썬 코드
- **models/**: 학습된 모델 저장 (.pkl, .h5 등)
