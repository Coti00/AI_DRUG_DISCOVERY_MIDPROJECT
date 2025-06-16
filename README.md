##📘 AI-Based Drug Discovery: EGFR Inhibitor for Lung Cancer
###🧬 프로젝트 개요
이 프로젝트는 인공지능(AI) 기반 신약개발 기법을 활용하여 폐암 치료 타깃인 EGFR (Epidermal Growth Factor Receptor) 억제제를 발굴하는 데 목적이 있습니다. EGFR은 비소세포폐암(NSCLC) 환자에게서 높은 발현율을 보이며, 이를 타깃으로 한 약물 개발이 활발히 이루어지고 있습니다.

###🔬 연구 배경
EGFR의 역할: 세포 성장, 생존, 분화를 조절하는 수용체로, EGFR의 변이는 폐암 발생과 밀접한 연관.

역학: 폐암은 전 세계 암 발병률 및 사망률 1위이며, EGFR 돌연변이는 특히 아시아인에게서 40~60% 유병률을 보임.

기존 치료제의 한계: 1~3세대 EGFR-TKI가 개발되었으나, 내성 돌연변이(T790M 등)로 인해 약효 지속에 한계가 있음.

###🧪 사용 기술 및 도구
Python

DeepChem: 분자 구조 분석 및 featurization

RDKit: 화학 분자 시각화 및 변환

Scikit-learn: 기계 학습 모델 학습 및 평가

Graph Neural Network (GCN): 분자 특성 기반 예측

AUC/ROC 등 성능 평가 지표

###📊 모델링 및 실험
데이터셋 구성: SMILES 구조를 가진 화합물과 그에 대한 EGFR 억제 활성을 라벨링한 데이터셋 사용.

Featurization 기법: GraphConvFeaturizer, Circular Fingerprint 등 다양한 분자 표현 방법 활용.

모델: GCN, Random Forest, MLP 등 비교 실험 진행.

평가지표: Accuracy, AUC, ROC Curve를 활용하여 모델 성능 평가.

###✅ 주요 결과
GCN 모델이 가장 높은 정확도 및 AUC 성능을 보임

EGFR 활성이 높은 약물 후보군을 시각적으로 분석하고, 분자 구조적 특성을 도출함

SHAP 값을 통해 주요 feature에 대한 모델 해석 가능

###📝 향후 계획
EGFR 이외의 다른 타깃에 대해서도 pipeline 적용

분자 생성 모델 (e.g., generative models) 활용하여 novel inhibitor 후보 도출

실제 wet-lab validation 가능성을 고려한 후보 약물 선정

