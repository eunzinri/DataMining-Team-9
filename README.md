# DataMining_Team_9

# 📊 산업공학과 졸업 후 취업 및 연봉 예측 프로젝트

데이터마이닝 과목의 팀 프로젝트로, 대학생의 다양한 개인/학업/생활 데이터를 바탕으로 **졸업 후 정규직 합격 여부 및 연봉 수준 예측**을 수행합니다.

---

## 📁 프로젝트 구성

- `DMT_Final.ipynb` - 전체 분석 및 예측을 수행한 메인 코드
- `DM2015.csv` ~ `DM2019.csv` - 연도별 설문에서 사용할 항목들을 추출한 데이터 
- `전공코드맵.csv`, `자격증코드맵.csv` - 전처리용 매핑 테이블

---

## 🔍 주요 내용

### 1. 데이터 전처리
- 전공/자격증 등의 코드 매핑
- 연도별 데이터를 통합하고, 주요 변수들을 정제/통일
- 결측치 처리 및 파생 변수 생성

### 2. 분석 주제 1: 졸업 후 정규직 합격 여부 예측
- 🎯 타겟 변수: `합격여부` (0: 미합격, 1: 합격)
- 사용 알고리즘:
  - Decision Tree
  - Random Forest (GridSearch를 통한 하이퍼파라미터 튜닝)
- 모델 성능 평가:
  - Accuracy, Classification Report
  - Feature Importance 시각화 및 SHAP 해석

### 3. 분석 주제 2: 연봉 수준 분류 (추정)
- 🎯 타겟 변수: `월 소득`으로부터 파생된 고연봉여부 (월 소득 >= 300만원)
- 분석 목적: 정규직 취업자들을 대상으로 어떤 요인이 고연봉과 관련 있는지 탐색
- 분류 방식 및 시각화 (예: 점수 구간, 수면시간, 부모 자산 등과의 관계 분석)

---

## 📌 주요 인사이트

- 졸업평점, 전공 일치도, 자격증 보유 여부 등이 취업 여부에 유의미한 영향을 미침
- 특정 학습 습관이나 생활 패턴이 결과에 긍정적으로 작용하는 경향 확인

---

## 🛠 재현 방법
- csv 파일 모두 다운로드 받은 후
- 주석에 따라 ipynb 파일 실행
