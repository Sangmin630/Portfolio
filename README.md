# 이상민 Portfolio

# Personal Info
- Email: lsm5877@gmail.com

---

# Introduction
Python과 SQL 기반 데이터 분석 역량을 바탕으로, GIS 공간 분석부터 머신러닝 모델 학습까지 다양한 프로젝트를 수행해 왔습니다.  
특히 위치 데이터와 모빌리티 서비스 품질 개선에 관심이 많으며, 데이터 기반으로 사용자 경험을 개선하는 Data Scientist로 성장하는 것을 목표로 하고 있습니다.

---

# Projects

| # | 프로젝트명 | 유형 | 주요 기술 |
|---|---|---|---|
| 1 | Seattle EV Charging Station Web GIS | 팀(4인) | Mapbox GL JS, Turf.js, GeoJSON, JavaScript |
| 2 | Mobility Infrastructure Imbalance Analysis | 팀(5인) | Python, Pandas, Streamlit, Folium, MySQL, Selenium |
| 3 | OULAD Dropout Prediction & Clustering | 팀(5인) | Python, Scikit-learn, MLflow, MySQL, Docker, Streamlit |

---

## 1. Seattle EV Charging Station Web GIS
**프로젝트 개요**  
시애틀 전기차 충전소 데이터를 시각화하고, 사용자가 원하는 조건에 따라 충전소를 탐색할 수 있도록 제작한 Web GIS 프로젝트입니다.

**주요 목표**
- 충전소 위치를 지도에서 직관적으로 확인
- 충전기 유형, 사용 가능 여부, 가격, 거리 기준 필터링 제공
- 사용자 위치 기반으로 가까운 충전소 탐색 지원

**역할**
- 충전소 데이터 수집 및 전처리
- GeoJSON 기반 데이터 구성
- 사용자 위치 기반 근접 충전소 탐색 기능 구현
- UI/UX 설계 참여 및 필터링 기능 정의

**문제 해결 경험**  
가격 정보가 비어 있거나 불명확한 데이터가 많아 단순 결측치로 제거할 경우 정보 손실이 커질 수 있었습니다. 이를 해결하기 위해 해당 값을 `unknown`으로 분류하고, 사용자가 직접 확인할 수 있도록 전화번호 조회 기능을 함께 제공했습니다.

**사용 기술**
- Mapbox GL JS
- Turf.js
- GeoJSON
- JavaScript
- GitHub Pages

**배운 점**
- 위치 데이터의 정확성이 사용자 의사결정에 미치는 영향을 체감
- 데이터 품질과 서비스 연결 구조의 중요성을 이해
- 모빌리티 데이터를 실제 서비스로 구현하는 과정을 경험

**링크**
- GitHub: https://github.com/slee0630-uw/Seattle_EV_Charging_Stations

---

## 2. Mobility Infrastructure Imbalance Analysis
**프로젝트 개요**  
차량 등록 데이터와 정비소 데이터를 결합하여 지역별 정비 인프라 불균형을 분석하고 시각화한 프로젝트입니다.

**주요 목표**
- 차량 대비 정비소 부족 지역 파악
- 지역별 인프라 불균형을 정량적으로 비교
- 정책적·서비스적 시사점을 도출할 수 있는 시각화 제공

**역할**
- FAQ 페이지 구현
- FAQ 크롤링
- 공통 레이아웃 컴포넌트 제작

**문제 해결 경험**  
차량 등록 데이터와 정비소 데이터의 공간 단위가 달라 바로 결합하기 어려웠고, 팀원들 사이에서도 17개 시도 단위로 단순화할지 시군구 단위까지 반영할지를 두고 의견이 갈렸습니다. 17개 시도 단위만 사용할 경우 실제 지도 시각화에서 지역 왜곡이 커질 수 있다고 판단했고, 시군구 단위까지 반영하는 방향으로 의견을 조율했습니다. 이를 통해 프로젝트의 분석 방향을 더 세밀하게 정리할 수 있었습니다.

**사용 기술**
- Python
- Pandas
- Streamlit
- Folium
- MySQL
- Selenium

**배운 점**
- 지표와 공간 단위 기준이 분석 결과 해석에 미치는 영향을 이해
- 프로젝트 방향성을 맞추는 커뮤니케이션의 중요성을 체감
- 데이터 기반 문제 정의와 시각화 설계 역량을 강화

**링크**
- GitHub: https://github.com/SKNETWORKS-FAMILY-AICAMP/sk25-1st-5team

---

## 3. OULAD Dropout Prediction & Clustering
**프로젝트 개요**  
OULAD(Open University Learning Analytics Dataset)를 기반으로 학습자 이탈을 예측하고 군집 분석을 수행한 머신러닝 팀 프로젝트입니다.

**주요 목표**
- 학습자 이탈 여부를 머신러닝 모델로 예측
- 여러 모델의 성능을 정량적으로 비교하여 최적 모델 선정
- 학습자 군집 분석으로 이탈 위험 그룹 프로파일 도출

**역할**
- 팀 전체 데이터 정의 및 전처리 기준 논의·결정 참여
- Random Forest 모델 담당 및 하이퍼파라미터 튜닝 수행
- MLflow 기반 실험 추적
- 모델별 성능(Accuracy, F1-score) 정량 비교 및 결과 분석

**문제 해결 경험**  
팀원마다 로컬 환경이 달라 같은 코드를 실행해도 결과가 달라지는 문제가 발생했습니다. 이를 해결하기 위해 Docker Compose로 MySQL, MLflow, Jupyter, Streamlit을 하나의 환경으로 묶어 팀 전체가 동일한 환경에서 분석을 수행할 수 있도록 구성했습니다. 이 경험을 통해 분석 재현성과 협업 환경 구축의 중요성을 직접 체감했습니다.

**사용 기술**
- Python
- Scikit-learn
- Random Forest
- XGBoost
- MLflow
- MySQL
- Docker Compose
- Streamlit

**배운 점**
- 모델 학습부터 실험 추적과 배포까지 이어지는 전체 파이프라인을 경험
- 데이터 전처리 기준이 모델 성능에 미치는 영향을 확인
- Docker 기반 협업 환경과 분석 재현성의 중요성을 체감

**링크**
- GitHub: https://github.com/SKNETWORKS-FAMILY-AICAMP/SKN25-2nd-3Team

---