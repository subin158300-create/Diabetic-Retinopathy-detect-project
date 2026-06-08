# DR Module (Diabetic Retinopathy EDA & Modeling)

## 1) 개요
본 분석 코드들은 프로젝트 DR(당뇨망막병증) 파트입니다.  
안저 이미지 데이터 기반으로 EDA, 라벨/품질 점검, 분류 모델 학습 및 외부 검증까지의 흐름으로 구성되어 있습니다.

## 2) 파일 구성
1. `EDA/DR_EDA_1.ipynb`  
   DR 데이터셋 탐색 분석 및 기본 통계 확인
2. `EDA/DR_DataSet_QC.ipynb`  
   데이터 품질 점검(QC)
3. `EDA/DR_Image-Label.ipynb`  
   이미지-라벨 매칭 및 샘플 확인
4. `EDA/DR_DataSet_Lable_basic_analysis(EDA).json`  
   EDA 결과 산출 JSON
5. `Modeling/DR_Modeling_RN50_baseline.ipynb`  
   ResNet50 베이스라인 모델 학습
6. `Modeling/DR_Modeling_RN50(bestmodel)_.ipynb`  
   ResNet50 성능 개선 실험
7. `Modeling/DR_Modeling_ENB3_baseline.ipynb`  
   EfficientNet-B3 베이스라인 학습
8. `Modeling/DR_Modeling_external_validation_APTOS2019.ipynb`  
   외부 데이터셋(APTOS2019) 검증

## 3) 분석/모델링 파이프라인 요약
- 이미지 데이터 품질 점검 및 라벨 일치성 확인
- 클래스 분포/샘플 특성 분석
- CNN 계열(ResNet50, EfficientNet-B3) 분류 모델 실험
- 실험 모델 간 성능 비교 후 외부 검증 수행

## 4) 모델링 메모
- 하이퍼파라미터/실험 로그는 각 노트북 내에 기록되어 있습니다.
- 최종 서비스 연동용 산출물은 웹서비스 저장소에서 관리합니다.

## 5) 수행 내용
- DR 데이터셋 구조 및 품질 진단
- 모델 아키텍처별 성능 비교 실험
- 외부 데이터 기반 일반화 성능 확인

## 6) 기술 스택
- Python
- Jupyter Notebook
- PyTorch / torchvision
- Pandas / NumPy / Scikit-learn

## 7) 참고
- 웹 연동 및 추론 서비스 구현은 별도 저장소 `Diabetic-Retinopathy-detect-project_Web-service`에서 관리합니다.
