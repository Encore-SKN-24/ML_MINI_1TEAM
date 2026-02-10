📑Table of Contents
1. 프로젝트 소개 
2. 팀원 소개
3. 프로젝트 개요
4. 데이터셋 정보
5. 데이터 전처리 과정
6. EDA
7. 모델링 및 성능평가
8. Conclusion & Discussion
9. 회고



# 1. **프로젝트 소개 (Title)**

###  **주제:🌲기상 데이터를 활용한 ML 기반 산불 발생 예측 및 예방 솔루션(Meteorological Data-Driven ML Model for Forest Fire Prediction and Prevention)**
### **기간: 2026년 2월 4일 ~ 2026년 2월 11일**
### **팀명: 🏆 ML 미니 프로젝트 1팀**

---

### 🛠 Tech Stack

#### 📚 Languages & Data Analysis
<img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white"> <img src="https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white"> <img src="https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white">

#### 🤖 Machine Learning
<img src="https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white"> <img src="https://img.shields.io/badge/XGBoost-blue?style=for-the-badge"> <img src="https://img.shields.io/badge/LightGBM-green?style=for-the-badge"> 
> **Models Used:** Decision Tree, Random Forest, Gradient Boosting, XGBoost, LightGBM

#### 📊 Visualization
<img src="https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black"> <img src="https://img.shields.io/badge/Seaborn-blue?style=for-the-badge">

#### 🤝 Collaboration
<img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white">


---
 
# 2. 👥 **팀원 소개**
 
| <img src="https://github.com/user-attachments/assets/192cc577-c7ac-49a9-9855-2230cd1cc55c" width="150" height="150"> | <img src="https://github.com/user-attachments/assets/3cb641b2-cfc5-4c3a-a10a-e0222ef9c673" width="150" height="150"> | <img src="https://github.com/user-attachments/assets/a60d634f-6fba-4cfb-b74e-b56d6be3f358" width="150" height="150"> | <img src="https://github.com/user-attachments/assets/a32be587-2de6-4884-8f66-0a4b303dfe53" width="150" height="150"> | <img src="https://github.com/user-attachments/assets/a367b378-429e-4117-85fa-bd968867ee28" width="150" height="150"> |
|:---:|:---:|:---:|:---:|:---:|
| **고아라** | **정재훈** | **김은우** | **나혜린** | **박수영** |
|  [![github - Akoh-0909](https://img.shields.io/badge/Akoh--0909-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Akoh-0909) | [![github - JeaHoon-J](https://img.shields.io/badge/JeaHoon--J-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/JeaHoon-J) | [![github - whitehole17](https://img.shields.io/badge/whitehole17-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/whitehole17) | [![github - ](https://img.shields.io/badge/nngpfls-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/nngpfls) | [![github - suyoung6279](https://img.shields.io/badge/suyoung6279-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/suyoung6279) |
| | | | | |



---



# 3. 🎯 **프로젝트 개요 (Overview)**

### 주제 선정 배경: 
본 프로젝트는 데이터 기반의 의사결정을 통해 사회적 난제를 해결하고자 하는 고민에서 시작되었다.

**1. 데이터 분석의 실전적 확장**

이전 EDA과정에서 다루었던 기상데이터를 보다 실질적인 사회적 이슈에 연결해보고자 했다. 단순 상관분석을 넘어, 머신러닝 모델링을 통해 실제 현장에서 활용 가능한 '예측 시스템'으로 확장하는 것을 목표로 삼았다.

**2. 산불 위기 대응을 위한 예방 체계의 필요성**

최근 기후변화로 인한 건조지수 상승과 강풍, 그리고 인위적 요인으로 인해 발생한 대형 산불은 더이상 특정 지역의 사고가 아닌 국가적인 구조적 재난이 되었다. 산불로 인한 인명, 재산, 환경피해가 반복적으로 언론에 보도되고 있는 현재, 산불 피해 규모와 회복 비용, 그리고 그 여파가 지역사회와 생태계에 미치는 장기적 영향에 주목하게 되었고, 데이터 분석 역량을 활용해 이 문제에 기여할 수 있는 방법을 고민하게 되었다.

-> **산불 위기대응**: 대형 산불에 대한 원인 데이터 기반의 예방 및 경보 체계 필요성 증대

**3. 실용적 가치 창출: 기술에서 솔루션으로**

이에 본 프로젝트는 과거 기상 및 산림 정보를 통합 분석하여 산불 발생 가능성을 사전에 예측하였다. <br/>
이를 통해:

- **행정 현장의 자원 최적화**: 인력과 장비를 고위험 지역에 선제적으로 배치할 수 있도록 지원
  
- **피해 최소화**: 데이터에 기반한 정밀한 경보 시스템을 구축하여 초기 진화 성공률을 높이고, 산림 자원 및 인명 손실을 막는 유의미한 솔루션을 제공하고자 함


<br/>


### 🔗 뉴스 및 자료 출처 (References)

##### 📰 관련 뉴스 보도
* [[뉴시스] "산불 막아라"…강원, 대형산불 대비 선제적 대응 체계 가동](https://www.newsis.com/view/NISX20260209_0003508833)
* [[연합뉴스] 동해안 대형산불 방지대책 마련…진화 헬기·인력 집중 배치](https://www.yna.co.kr/view/AKR20260209006000053?input=1195m)
* [[강원도민일보] 기후변화가 부른 재난…이제 산불은 사계절 구조적 위험](https://www.kado.net/news/articleView.html?idxno=2033140)
* [[위키백과] 2022년 울진-삼척 산불 정보 (역대 최대 규모)](https://ko.wikipedia.org/wiki/2022%EB%85%84_%EC%9A%B8%EC%A7%84-%EC%82%BC%EC%B2%99_%EC%82%B0%EB%B6%88)
* [[YTN 뉴스] 역대 최악 산불...실화자, 처벌 물론 배상책임 (YouTube)](https://www.youtube.com/watch?v=sbZC2LiKeaE)

<br/>
<br/>

---

# 4.📂 **데이터 출처 및 참고 문헌**

### 📊 분석 데이터셋 (Datasets)
* **산불 발생 데이터**: [산림청 산불정책기술플랫폼 실시간 산불 정보](https://fd.forest.go.kr/ffas/)
* **기상 데이터**: [기상청 공공데이터포털 ASOS/AWS 관측 데이터](https://data.kma.go.kr/)
* **지역별 경지면적**: [KOSIS 국가통계포털 - 전국(도별) 논밭별 경지면적](https://kosis.kr/statHtml/statHtml.do?orgId=101&tblId=DT_1EB001)
* **산림 면적 정보**: [KOSIS 국가통계포털 - 산림면적 통계](https://kosis.kr/statHtml/statHtml.do?orgId=110&tblId=DT_11001N_2013_A022)
* **인구 밀도 데이터**: [KOSIS 국가통계포털 - 인구밀도(시도별)](https://kosis.kr/statHtml/statHtml.do?orgId=101&tblId=DT_1B08024)

### 📖 참고 문헌 및 연구 자료
* **분석 논리**: 국립산림과학원(NIFoS), *2025년 산불 제대로 알기*
* **지리 데이터 기준**: 통계청 시도별 행정구역 및 지목별 면적 통계 기준 적용
---
  

# 5.📋**데이터 전처리 (Preprocessing Pipeline)**

- EDA 단계(Before):
결측치/이상치 탐색, 기상 변수 분포·계절성 파악, 산불 발생 시기·지역 히트맵 등 현상 이해 중심의 분석 수행.

- ML 단계(After):
날짜·행정구역 기준으로 모든 데이터셋을 통합하고, 파생 변수 (실효습도, 농지비율, 도시산림 인접지수) 생성, 결측치 보간·평균 대체, SMOTE로 클래스 불균형을 보정해 모델 학습에 최적화된 형태의 피처 세트 구축


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
<br/><br/>

## **변수 정리**

## 💡 주요 파생 변수 및 생성 근거

산불 발생의 주요 원인이 **인적 실화와 소각 행위**라는 통계적 근거에 기반하여, 정적 데이터(Static Data)를 활용한 3가지 핵심 변수를 추가하였음.


### 1. 도시 산림 인접 비율 (WUI, Wildland-Urban Interface)

**산출 방식**
```
WUI = (지역별 산림 면적 / 지역 전체 면적) × 인구 밀도
```

**설명**  
지역의 산림(연료) 비율과 인구 밀도를 결합하여 **사람이 산림 연료와 접하는 잠재적 강도**를 연속형 지표로 나타냄. 값이 클수록 지역 면적 대비 산림 비중이 높고 인구가 밀집한 지역으로, 산불 발생 위험이 상대적으로 높을 수 있음을 의미.

**근거**  
Stewart et al.(2007)은 WUI를 다음과 같이 정의함:
- **혼합형 WUI**: 40에이커당 택지 1개 이상이고, 야생 식생이 전체 면적의 50% 이상인 지역
- **접경형 WUI**: 40에이커당 택지 1개 이상이고, 1.5마일 이내에 야생 식생 75% 이상으로 덮인 1,235에이커 이상의 대규모 지역이 인접한 경우

본 프로젝트에서는 WUI 개념을 적용하여 **지역 단위에서 산림 비중과 인구밀도를 결합한 연속형 지표**를 사용하였음.

> **출처**: 안현진·정도채·김동욱·정호근. (2024.12). *산림 인접지역의 효과적 산불 관리를 위한 개선과제*(연구보고서 R 2024-19). [한국농촌경제연구원]

---

### 2. 논밭 비율 (Agricultural Ratio)

**산출 방식**
```
논(밭) 비율 = 지역별 논(밭) 면적 / 전국 논(밭) 총 면적
```

**설명**  
지역의 농지(논/밭) 면적 비율

**근거**  
최근 10년간 산불 원인 통계에 따르면 **논·밭두렁 소각(11.0%)** 및 쓰레기 소각(12.4%) 등 소각 행위가 전체 산불 원인의 23.4%를 차지함. 

> **출처**: 산림청. (2025). [*2025년 산불 제대로 알기*]


### 3. 실효습도 (Effective Humidity)

산불 예측의 정확도를 높이기 위해 당일의 습도뿐만 아니라 과거의 습도가 누적되어 지표면의 건조 상태에 영향을 미치는 **'실효습도'**를 파생변수로 생성하였음.

**산출 방식**
실효습도($H_e$)는 다음과 같은 수식으로 계산됨.
$$H_e = (1 - r)(h_0 + r^1h_1 + r^2h_2 + r^3h_3 + r^4h_4 + r^5h_5)$$
* $r$: 연소율 (일반적으로 0.7 사용)
* $h_n$: n일 전의 평균 상대습도

#### 🧐 실효습도란?
> 화재 예방의 목적으로 사용되는 지수로, 당일의 상대습도뿐만 아니라 **전날부터 과거 수일간의 습도에 경과시간에 따른 가중치를 주어 산출한 지수**.
> 목재 등의 건조도를 나타내며 산불 발생 위험도를 판단하는 중요한 지표가 됨.


### 3-1. 변수 산출 로직 및 근거
모델의 예측력을 높이기 위해 산불 확산의 물리적 메커니즘을 분석하고, 이를 코드로 구현하였음.

#### **[산불 확산 영향 요인 분석]**
![산불확산에 영향 미치는 요인](./img/산불확산에 영향 미치는 요인.png)
> **인사이트:** 산불은 단순히 발생 여부를 넘어 기온, 풍속, 습도 및 지형적 특성이 복합적으로 작용하여 확산됨. 본 모델은 이러한 요인들을 독립 변수로 채택하여 학습을 진행하였음.

#### **[핵심 파생변수: 실효습도(Effective Humidity)]**
단기 습도가 아닌, 수일간의 누적 건조 상태를 반영하기 위해 **실효습도**를 산출하여 변수로 활용함.

<p align="center">
  <img src="https://github.com/user-attachments/assets/bd200d12-7b3c-41ac-9837-c93977de0f5f" width="48%" />
  <img src="https://github.com/user-attachments/assets/b6032a95-7b9d-4744-81dd-787f8d1cacb0" width="48%" />
</p>

> **💡 Note**: 신설된 관측소(세종, 북부산 등)의 경우 초기 과거 데이터 부재로 발생하는 결측치는 모델의 신뢰성을 위해 제거 후 분석을 진행하였습니다.
> *(참고: 국립산림과학원 산불지식정보, 기상청 기상지상관측지침)*

---



# 6. 📊**EDA**

## 6.1. 산불 데이터 (Forest Fire Data)
산불 발생 지점, 시간, 원인(피해 규모 포함) 데이터를 기반으로 주요 발생 패턴 파악하였음.


### 6.1.1. 지역별 산불 발생 현황
<img src="https://github.com/user-attachments/assets/ab7ce9f6-46a4-4691-82dc-a4fe3ed1c830" width="600">
 
 > **분석 요약:** 시도별 발생 횟수 시각화 결과, 특정 지역에 산불이 집중되는 경향을 확인하였는데, 이는 지역별 지형 및 산림 밀도 등 공간적 특성이 산불 발생의 주요 변수임을 시사하며, 모델링 시 지역별 가중치 설정의 기초가 되었음.


### 6.1.2. 산불 발생 원인 분석
<img src="https://github.com/user-attachments/assets/3dae1119-27bd-41eb-a3d6-b729352dadcf" width="600">

> **분석 요약:** 분석 결과, 자연적 요인보다 입산자 실화 및 부주의 등 인위적 요인이 압도적인 비중을 차지함. 이는 기상 데이터뿐만 아니라 인적 활동을 수치화한 파생 변수(WUI 등)의 도입 필요성을 뒷받침함.

### 6.1.3. 기타 원인 상세 분석
<img src="https://github.com/user-attachments/assets/6c6810cf-8f61-44b7-a81a-ec782cd11a0b" width="600">

> **분석 요약:** 위 원인 분석 중 '기타'로 분류된 항목들을 세분화하여 분한 그래프. 이를 통해 쓰레기 소각, 건축물 화재 전이 등 모델이 학습해야 할 미세한 위험 요인들을 파악하고 데이터 라벨링의 정확도를 개선하였음.

### 6.1.4. 산불 발생 원인 통계 (Reference)

국립산림과학원 자료에 따르면 전체 산불의 절반 이상이 실화·소각 등 인적 요인으로 발생하며, 본 모델은 이러한 인적 요인을 정량화하여 예측에 반영하고 데이터 정합성을 확인하였음.

<div align="center"> <img src="https://github.com/user-attachments/assets/d375fe72-0f3c-4652-819a-386fb33750c1" alt="월별 원인별 산불발생 현황" width="600"> <p><i>출처: [국립산림과학원] 2025년 산불 제대로 알기</i></p> </div>


| 컬럼명 | 설명 | 비고 |
| :--- | :--- | :--- |
| `발생일시_년/월/일/시간/요일` | 산불 발생 시점의 상세 일시 정보 | - |
| `진화종료시간_년/월/일/시간` | 산불 진화가 완료된 시점 | 지속시간 계산 가능 |
| `발생장소_관서/시도/시군구/읍면/동리` | 산불 발생 행정 구역 정보 | 공간 분석용 |
| `발생원인_구분/세부원인/기타` | 산불 발생 사유 (실화, 소각 등) | 원인 분석용 |
| `피해면적_합계` | 산불로 인한 총 소실 면적 | - |

### 6.1.5. 변수 간 상관관계 분석 (Correlation Analysis)

산불 발생 여부와 주요 기상 및 지표 데이터 간의 상관성 분석 및 변수의 유효성 검증.

<p align="center">
  <img src="https://github.com/user-attachments/assets/8653d96c-532a-49f1-93e3-1e12b59efb41" width="80%">
</p>

* **실효습도**: 산불 발생과 음의 상관관계를 가짐 -> 실효습도가 낮을수록(나무나 풀이 바짝 마를수록) 산불은 더 자주 발생
* **인적 요인(밭 비율)**: 약한 양의 상관관계를 보여, 농지 소각 행위가 실제 산불의 주요 원인=사람이 있는 곳에 불이 난다라는 통계를 입증함.
* **평균기온, 강수량, 풍속과는 낮은 상관관계**:실효습도 같은 복합 변수가 더 유의미함을 확인하였음.

  
---

## 6.2. 날씨 데이터 (Weather Data)
전국 기상 관측 정보

| 컬럼명 | 설명 | 단위 |
| :--- | :--- | :--- |
| `지점 / 지점명` | 관측소 코드 및 지역 이름 | 지역 매칭용 |
| `일시` | 데이터 측정 날짜 | 시간 매칭용 |
| `평균/최저/최고기온` | 당일 온도 정보 | °C |
| `일강수량` | 하루 동안 내린 비의 양 | mm |
| `최대/평균 풍속` | 바람의 세기 | m/s |
| `최소/평균 상대습도` | 대기 중 습도 상태 | % |
| `일 최심적설` | 쌓인 눈의 최대 깊이 | cm |

---

## 6.3. 최종 분석용 데이터셋 (Final Feature Set)
모델 학습을 위해 전처리가 완료된 핵심 변수 리스트 (62,018 X 9)

| 컬럼명 | 설명 | 중요도 및 역할 |
| :--- | :--- | :--- |
| **평균기온(°C)** | 당일 평균 기온 | 기온 상승 시 산림 내 가연물 건조 가속화 |
| **일강수량(mm)** | 당일 총 강우량 | 직접적인 산불 발생 억제 요인 |
| **최대/평균 풍속(m/s)** | 바람의 세기 | 산불의 확산 속도 및 대형산불 전이 판단 |
| **최소/평균 상대습도(%)** | 대기 중 습도 | 발화 가능성을 측정하는 기초 지표 |
| **일 최심적설(cm)** | 쌓인 눈의 깊이 | 동절기 산불 억제 및 수분 공급 요인 |
| **실효습도** | 수일간의 습도를 가중치로 계산 | **핵심 지표:** 목재의 건조 상태를 나타냄 (30% 이하 시 위험) |
| **논/밭_비율** | 주변 토지 이용 형태 | 농작물 폐기물 소각으로 인한 산불 전이 분석 |
| **도시_산림_인접지수** | 도시와 산림의 경계 밀접도 | 인위적 실화 가능성 및 인명 피해 위험도 산출 |
| **산불 유무** | 산불 발생 여부 (0/1) | **Target 변수:** 분류(Classification) 모델의 목적값 |



---------------------

# 7. 📊 **모델링 및 성능 평가 (Modeling & Evaluation)**

## 7.1. 모델별 주요 결과 요약

| 순서 | Model | Key Insights & Performance | Optimization |
| :---: | :--- | :--- | :--- |
| 01 | **Decision Tree** | 직관적인 규칙 기반 분석을 통해 **실효습도** 등 초기 주요 변수 파악. (Recall 85% 확보) | Max Depth 제한으로 과적합 방지 |
| 02 | **Random Forest** | 여러 트리를 결합해 안정성 확보. **정확도(91%)**와 **AUC(0.91)**에서 최상위 성능 기록. | Bagging 및 특성 선택 최적화 |
| 03 | **Gradient Boosting** | 오차를 순차적으로 보정하여 **AUC 0.88**의 높은 판별력 확보. | Optuna 하이퍼파라미터 최적화 |
| 04 | **XGBoost** | 대규모 데이터 처리에 최적화. `Scale_pos_weight` 적용으로 **클래스 불균형** 해소. | 정밀 파라미터 튜닝 |
| 05 | **LightGBM** | 학습 속도가 가장 빠르며 리소스 효율성이 높은 최신 부스팅 기법 활용. | Optuna 자동 튜닝 |

> **📊 분석 요약:** 모든 모델에서 '실효습도'가 산불 발생의 핵심 지표임을 재확인하였으며, 실무 배포 시 성능과 속도 면에서 **LightGBM**과 **Random Forest**의 활용 가치가 가장 높음을 입증하였음.



## 7.2. 모델링 전략 및 워크플로우

#### 목표 지표: 산불은 발생 징후를 놓치지 않는 것이 최우선이므로, **재현율(Recall)**과 AUC-ROC를 핵심 평가지표로 설정함.

#### 데이터 불균형 대응: 산불 미발생 데이터가 압도적으로 많은 특성을 고려하여 SMOTE(Over-sampling) 및 scale_pos_weight 파라미터를 적용해 학습 편향을 방지함.

#### 최적화: Optuna를 활용한 하이퍼파라미터 자동 튜닝으로 모델별 최적의 성능 도출.
<br/>
<br/>

- **(1) 사용한 모델: Decision Tree & Random Forest**

#### [하이퍼 파라미터 튜닝 결과]

<table style="width: 100%; border-collapse: collapse;">
  <tr>
    <td style="width: 50%; text-align: center; vertical-align: top;">
      <img src="https://github.com/user-attachments/assets/e55a8538-64c1-46de-bf60-008c6c8ad921" height="400px">
      <p><b>Decision Tree 파라미터</b></p>
    </td>
    <td style="width: 50%; text-align: center; vertical-align: top;">
      <img src="https://github.com/user-attachments/assets/1cb19cab-a647-4b9e-96b4-3042159adf40" height="400px">
      <p><b>Random Forest 파라미터</b></p>
    </td>
  </tr>
</table>


모델 성능 극대화를 위해 **Optuna**를 활용하여 하이퍼파라미터 튜닝을 수행하였음.
* **Decision Tree**: 과적합 방지를 위해 **최대 깊이(max_depth)를 5**로 제한함.
* **Random Forest**: **265개의 결정 트리**와 **'log2' 특성 선택 방식**을 통해 예측 안정성을 확보한 최적의 조합을 도출하였음.



#### [두 모델 성능 비교]

!<img width="493" height="253" alt="Image" src="https://github.com/user-attachments/assets/467b77f6-081d-4439-ba45-9401c9f34078" />



#### [Classification Report]
<table style="width: 100%; border-collapse: collapse;">
  <tr>
    <td style="width: 50%; text-align: center; vertical-align: top;">
      <img src="https://github.com/user-attachments/assets/40f438cc-099f-4bf4-a020-5c0c1b9c0b43" height="250px">
      <p><b>모델 성능 분석 1</b></p>
    </td>
    <td style="width: 50%; text-align: center; vertical-align: top;">
      <img src="https://github.com/user-attachments/assets/7f9be420-bf78-4354-9acf-59bbcd393927" height="250px">
      <p><b>모델 성능 분석 2</b></p>
    </td>
  </tr>
</table>

> **Decision Tree**는 **85%의 높은 재현율(Recall)**로 산불 발생 징후를 민감하게 포착하지만, 낮은 정밀도로 인해 오탐지가 발생하는 한계가 있었음. 이를 개선한 **Random Forest**는 **정밀도를 46%까지** 끌어올리고 **전체 정확도를 91%로 향상**시켜, 모델의 안정성과 예측 신뢰도를 동시에 확보하였음.



#### [특성 중요도 (Feature Importance)]
<table style="width: 100%; border-collapse: collapse;">
  <tr>
    <td style="width: 50%; text-align: center; vertical-align: top;">
      <img src="https://github.com/user-attachments/assets/1ba44a0e-692a-46ce-9dc7-1ec4032ca0dc" style="width: 100%;">
      <p><b></b></p>
    </td>
    <td style="width: 50%; text-align: center; vertical-align: top;">
      <img src="https://github.com/user-attachments/assets/c57fd532-b6e5-44f0-9a42-f3190163244f" style="width: 100%;">
      <p><b></b></p>
    </td>
  </tr>
</table>

두 모델 모두 '**실효습도**'를 산불 발생의 가장 결정적인 요인으로 판단하였음.
* **Decision Tree**: 실효습도와 토지 피복도(논 비율) 등 **특정 상위 변수**에 의존도가 높음.
* **Random Forest**: 실효습도 외에도 상대습도, 기온, 풍속 등 **기상 변수들을 고르게 반영**하여 예측의 다각화를 이루었으며, 기상 데이터의 복합적인 상호작용을 더 잘 학습함.



#### [ROC Curve & AUC]
<table style="width: 100%; border-collapse: collapse;">
  <tr>
    <td style="width: 50%; text-align: center; vertical-align: top;">
      <img src="https://github.com/user-attachments/assets/152f8a5c-b129-48d1-92d2-a69c8b938df4" style="width: 100%;">
      <p><b></b></p>
    </td>
    <td style="width: 50%; text-align: center; vertical-align: top;">
      <img src="https://github.com/user-attachments/assets/a0d74db7-737a-4ae8-b9a0-458bda583034" style="width: 100%;">
      <p><b></b></p>
    </td>
  </tr>
</table>

ROC Curve 분석 결과, **Random Forest(AUC = 0.91)**가 Decision Tree보다 높은 수치를 기록하며 전반적인 예측 판별력이 우수함을 입증함. 두 모델 모두 좌상단으로 치우친 **이상적인 곡선 형태**를 보여 유효성을 확보하였으나, **Random Forest가 AUC에서 0.02 가량 앞서며** 미세한 성능 우위를 점했음.


---

- **(2) 사용한 모델: Gradient Boosting (앙상블)**
  
- **성능향상을 위한 노력**:
  - Hyperparameter Tuning - Optuna 라이브러리 활용하여 최적의 하이퍼파라미터 조합을 탐색.
  - 학습률(learning_rate), 트리의 개수(n_estimators), 트리의 깊이(max_depth)등을 세밀하게 조정하여 과적합을 방지하고 일반화 성능을 높임
- **성능결과 및 해석**:
  - ROC Curve: AUC 수치가 0.88로 측정됨. 이는 모델이 산불 발생 여부(Class 0, 1)를 매우 높은 확률로 정확하게 판별하고 있음을 의미.

  - Feature Importance: 모델이 예측 시 가장 중요하게 참고한 변수는 **'실효습도'**와 **'평균 상대습도'**였음. 이는 산불 예측에 있어 대기의 건조 상태가 결정적인 역할을 한다는 데이터적 근거가 됨. (대기 건조도의 누적치가 산불 위험을 결정짓는 중요한 물리적 요인임을 입증)
    
<table style="width: 100%; border-collapse: collapse;">
  <tr>
    <td colspan="2" style="text-align: center; vertical-align: top;">
      <img src="https://github.com/user-attachments/assets/35231abd-31c1-4755-a780-99cda409cbcc" width="80%">
      <p><b>Gradient Boosting 하이퍼파라미터 튜닝 과정 (Optuna)</b></p>
    </td>
  </tr>
  <tr>
    <td style="width: 50%; text-align: center; vertical-align: top;">
      <img src="https://github.com/user-attachments/assets/0b495d3b-caf3-45f4-ae82-658aa3140046" style="width: 100%;">
      <p><b>ROC Curve (AUC = 0.88)</b></p>
    </td>
    <td style="width: 50%; text-align: center; vertical-align: top;">
      <img src="https://github.com/user-attachments/assets/6e919e0c-06e4-46f4-ac75-ffcad7c6f02b" style="width: 100%;">
      <p><b>Feature Importance</b></p>
    </td>
  </tr>
</table>


---

- **(3) 사용한 모델: XGBoost**

<div align="left">
  <img src="https://github.com/user-attachments/assets/d2d78eb1-1929-4914-86b3-a8f2cae54881" alt="auc-roc와 혼동행렬" width="600">
  <p><i>auc-roc 곡선</i></p>
</div>

<div align="left">
  <img src="https://github.com/user-attachments/assets/1e122378-2e9c-4186-859e-1ed9abbe4705" alt="auc-roc와 혼동행렬" width="600">
  <p><i>혼동행렬</i></p>
</div>

- **성능 향상을 위한 노력**: 

smote로 산불이 1이 되는 값을 임의로 늘렸다. 그러나 precision이 낮게 나왔음
<div align="left">
  <img src="https://github.com/user-attachments/assets/fcf20cc6-a62b-4794-b0ec-820573ccff57" width="600">
</div>

<div align="left">
  <img src="https://github.com/user-attachments/assets/8e39b9cc-9f40-4169-a954-0a50d33a7555" width="600">
</div>

이후에 scale_pos_weight를 사용하여 하이퍼 파라미터 탐색

<div align="left">
  <img src="https://github.com/user-attachments/assets/e0366e0f-4229-44b1-8e7a-e2aa06fb9dea" width="600">
</div>

<div align="left">
  <img src="https://github.com/user-attachments/assets/fa7aa882-c974-4148-8e47-9307bf11cd20" width="600">
</div>

---

- **(4) 사용한 모델: LightGBM**
- **성능 향상을 위한 노력**: optuna 활용 최적의 하이퍼파라미터 활용
<img width="726" height="425" alt="1  lightGBM 하이퍼파라미터" src="https://github.com/user-attachments/assets/57d3c10a-1f44-4179-82d1-90ed6d306d89" /><br/>

<table style="width: 100%; border-collapse: collapse;">
  <tr>
    <td style="width: 50%; text-align: center; vertical-align: top;">
      <img src="https://github.com/user-attachments/assets/f5da1754-31cf-434a-abf0-b1e738107358" style="width: 100%;">
      <p><b>⭐ Model 별 ROC Curve 비교</b></p>
    </td>
    <td style="width: 50%; text-align: center; vertical-align: top;">
      <img src="https://github.com/user-attachments/assets/3d6db174-5d8a-46a3-b08e-3905ab9af392" style="width: 100%;">
      <p><b>⭐ Feature Importances (LightGBM)</b></p>
    </td>
  </tr>
</table>



---


​
## 7.3. 종합성능 분석 및 시각화

[모델 성능 비교 및 평가]
Random Forest는 Decision Tree의 한계인 낮은 정밀도를 46%까지 끌어올리며 전체 정확도를 91%로 향상시켰음. 반면 부스팅 계열 모델들은 AUC 0.88~0.91의 이상적인 곡선을 그리며 산불 발생 여부에 대한 강력한 판별력을 입증할 수 있었음.

<table style="width: 100%; border-collapse: collapse;"> <tr> <td style="width: 50%; text-align: center;"> <img src="https://github.com/user-attachments/assets/152f8a5c-b129-48d1-92d2-a69c8b938df4" style="width: 100%;"> <p><b>ROC Curve (Random Forest)</b></p> </td> <td style="width: 50%; text-align: center;"> <img src="https://github.com/user-attachments/assets/f5da1754-31cf-434a-abf0-b1e738107358" style="width: 100%;"> <p><b>Model 별 ROC Curve 비교</b></p> </td> </tr> </table>

[특성 중요도 (Feature Importance)]
모든 모델이 공통적으로 **'실효습도'**를 산불 발생의 가장 결정적인 요인으로 판단함. 이는 단기 습도보다 수일간 누적된 건조 상태가 발화에 더 직접적인 영향을 미친다는 도메인 지식과 일치하는 결과임.

<div align="center"> <img src="https://github.com/user-attachments/assets/3d6db174-5d8a-46a3-b08e-3905ab9af392" width="80%"> <p><i>최종 모델(LightGBM) 특성 중요도 분석 결과</i></p> </div>


---



# 8. **Conclusion & Discussion**

## **8.1. 최종 모델 예측 결과 요약**

본 프로젝트는 Random Forest, Gradient Boosting, XGBoost, LightGBM, Decision Tree 총 5가지 모델을 비교 분석하였음.

- **성능 우수성**: 전반적으로 모든 모델에서 AUC 0.88 ~ 0.91의 높은 수치를 기록하며 산불 발생에 대한 우수한 판별력을 보였음.특히 Random Forest와 LightGBM이 정확도(91%)와 재현율(Recall) 측면에서 안정적인 성능을 보였음.

- **핵심 변수**: 모든 모델에서 **'실효습도'**가 가장 중요한 변수로 도출되었음. 이는 단발성 기상 현상보다 누적된 건조 상태가 산불의 결정적 원인임을 시사하는 바임. 또한, **'논밭 비율'**과 'WUI' 지표가 주요 변수로 작용하여 인적 요인에 의한 산불 발생 가능성을 모델이 잘 학습했음을 확인하였음.

## **8.2. 프로젝트 기대효과**

1. **데이터 기반 선제적 행정**: 감에 의존한 순찰이 아닌, 모델이 제시하는 고위험 지역(시·군·구 단위)에 예방 인력과 진화 헬기를 선제적으로 배치하여 골든타임을 확보할 수 있음.
   -> 자원 배치의 '선택과 집중' (Efficiency)<br/>
   : 현실적으로 모든 산에 산불 감시원을 배치하거나 24시간 헬기를 띄우는 것은 얘산과 인력이 부족하기 때문에 불가할 것으로 예상된다. 따라서 기존에 봄/가을철 조심 기간에 모든 산림 지역에 일괄적으로 인력을 배치하였던 방식을 본 모델을 적용한 후 실효습도가 30% 이하이면서 농지 비율이 높은 지역을 위주로 해당 지역 순찰 횟수를 1일 5회, 소방 헬기 전진 배치 거점을 모델이 찍어준 고위험군 군락 근처로 이동시켜 한정된 예산으로 방어력을 높이는 효과를 볼 수 있다고 예상됨.

2. **대국민 맞춤형 경보**: 단순 '산불 조심' 재난 문자가 아닌, 지역별 농지 소각 위험도 등을 반영한 정밀 경보 서비스 시스템의 기초 자료로 활용 가능.
   -> 핀포인트(Pin-point) 재난 문자 및 계도(Targeting)<br/>
   : 모두에게 보내는 재난 문자는 사람들이 무시하기 쉬움. 하지만 모델은 '누가' 불을 낼 가능성이 높은지 알려줄 수 있음. 기존에 전 국민에게 건조하니 산불조심하세요 라는 문자를 보냈었지만, 모델 적용 후, 농번기에 실효습도가 임계치 이하로 떨어지면, 농지비율이 높은 마을의 이장님들에게 전용 알림을 보내어 구체적인 가이드가 가능해짐.
    
3. **경제적 손실 최소화**: 초기 진화 성공률을 높임으로써 연간 수천억 원에 달하는 산림 복구 비용 및 탄소 흡수원 소실에 따른 간접적 경제 피해를 줄일 수 있음.
   -> 'WUI(도시 산림 인접지)' 관리 정책 수립 (Infrastructure)<br/>
   : WUI 지수가 높다는 것은 산불이 났을 때 인명 피해로 직결될 위험이 크다는 뜻. 기존에는 산불이 난 뒤에야 민가 피해를 수습하였다면, 모델 적용 후에는 모델이 지목한 WUI 고위험 지역을 대상으로 '산불 완충 지대'를 우선 설치, 고위험군으로 분류된 마을 주변의 잡목을 우선 제거하거나, 방화수림을 조성하고, 비상 소화전 설치 우선순위를 결정하는 등 도시 계획의 근거 데이터가 되며, 이는 사후 수습 비용(수천억 원)을 사전 예방 비용 (수억원)으로 대체하는 엄청난 경제적 이득을 가져다 줄 것으로 예상함.

## **8.3. 산불 발생 예측 시스템으로서의 배포 가능성**
-> 실시간 연동: 기상청 ASOS/AWS API를 연동하여 매일 업데이트되는 기상 정보를 모델에 입력하면, 일 단위 산불 위험도 예측 서버로 즉시 배포가 가능할 것으로 예상

## **8.4. 프로젝트의 한계점 및 향후 과제**

본 프로젝트는 기상 데이터와 인적 요인을 결합하여 유의미한 예측 성과를 거두었으나, 다음과 같은 기술적 한계와 향후 개선 과제를 확인하였음:

### - 공간 해상도 및 지형 데이터의 부재

현재 시·도/시·군·구 단위의 광역 데이터를 사용하고 있어, 실제 산불 확산에 결정적인 영향을 미치는 **국지적 지형(경사도, 산의 방향, 계곡 지형)**의 특성을 세밀하게 반영하지 못하였음. 향후 GIS(지리정보시스템) 데이터 결합이 필요.

### - 인적 활동 추정의 간접성

도시 산림 인접 비율(WUI)은 인구 밀도가 높은 도심지의 특성을 과하게 반영할 위험이 있음. 또한 실제 등산객 수나 실시간 소각 신고 등 직접적인 인적 활동 데이터를 확보하지 못해 밭 비율 등으로 간접 추정한 점이 한계로 남아있음.

### - 희소 사건(Rare Event)에 따른 데이터 불균형

산불은 미발생일이 압도적으로 많은 불균형 데이터로, SMOTE와 scale_pos_weight로 보정했음에도 불구하고, 높은 재현율(Recall) 대비 낮은 정밀도(Precision, 오탐지) 문제가 발생하였음. 실무 적용을 위해서는 오탐율을 낮추는 모델 고도화가 추가적으로 필요.

---

<br/>
<br/>

# 9.💭한 줄 회고

**고아라**
```
Keep (좋았던 점)
- 프로젝트 스토리텔링 완성: 5가지 모델링 결과를 관통하는 핵심 변수(실효습도, WUI 등)를 추출하여 프로젝트의 논리적 흐름을 구축하고, 이를 가독성 높은 README로 문서화함.
- 전략적 발표 준비: 기술적인 분석 내용을 비전공자도 이해하기 쉬운 기대 효과와 솔루션 중심으로 재구성하여 프로젝트의 실무적 가치를 강조함.

Problem (아쉬운 점)
- 초기 기획 단계의 리스크 관리: 주제 선정과 문제 정의 단계에서 더 구체적인 가이드라인을 세웠다면 팀원들의 작업 효율을 더 높였을 것이라는 아쉬움이 남음.
- 기술적 숙련도: 취합 과정에서 모델별 특성을 깊이 있게 다루기에는 스스로의 ML 숙련도가 부족함을 느껴 보완의 필요성을 체감함.

Try (시도할 점)
- 체계적인 프로젝트 매니징: 다음 프로젝트에서는 문제 정의 체크리스트를 미리 도입해 기획 단계를 더 탄탄하게 다질 예정임.
- 도메인 융합 역량 강화: 기상 및 산림 데이터 외에도 GIS 등 다양한 도메인 지식을 학습하여 더 정교한 분석 설계가 가능하도록 노력할 것임.
```

**정재훈**
```
comment 작성
```

**김은우**
```
comment 작성
```

**나혜린**
```
이번 프로젝트를 진행하며 가장 먼저 어려움을 느낀 부분은 주제 선정이었습니다. 머신러닝까지 적용해야 하는 프로젝트이다 보니, 분석 가치가 있는 주제인지 그리고 실제로 모델까지 연결할 수 있을지에 대한 고민이 컸습니다. 아이디어를 떠올리는 것보다 현실적으로 활용 가능한 데이터가 존재하는지를 판단하는 과정이 더 어려웠습니다. 주제를 정한 이후에도 데이터 전처리 단계에서 데이터 불균형 문제가 있었습니다. 산불 발생이라는 희귀 이벤트를 모델이 학습하도록 만드는 과정에서, 단순히 모델을 적용하는 것보다 데이터의 특성과 문제 구조를 이해하는 것이 훨씬 중요하다는 것을 깨달았습니다. 향후 프로젝트에서는 주제 선정 단계부터 데이터 구조와 분석 방향을 더 명확히 설정해야겠다는 기준을 갖게 되었습니다.
```

**박수영**
```
모델 학습을 하면서, 일차적으로 회귀인가 분류인가 하는 문제에 직면했고, 모델을 선택한 이후에도 하이퍼 파라미터를 조정하는 과정이 어려웠다. 특히 모델을 만들고 내가 예측하려는 산불이 
정확도보다는 재현율이 중요하기 때문에, recall을 높여야 한다는 것, 점수가 높지 않게 나와 GridSearchCV를 사용했는데, 너무 오래 걸려서 결국에 RandomizedSearchCV를 사용해서 최적의 파라미터를 찾았다.
상황에 따라, 또 목적에 따라서 모델 이외에 부수적인 것들의 선택지가 다양하다는 것을 이론 이외에 실제로 느꼈다.
```
<br/><br/>

---

### 📂 폴더 구조 안내
- **data/**: 데이터셋 파일 (raw, processed)
- **notebooks/**: EDA 및 실험용 주피터 노트북
- **src/**: 실제 실행용 파이썬 코드
- **models/**: 학습된 모델 저장 (.pkl, .h5 등)
