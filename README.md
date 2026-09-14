# 제조 AI 실제 (Manufacturing AI Practical)

대학원 2학기 **제조 AI 실제** 과목의 주차별 실습 과제를 정리한 저장소입니다.
CWRU(Case Western Reserve University) 모터 베어링 진동 실데이터를 활용해 패턴인식과 특징 추출 개념을 실습합니다.

## 폴더 구조

```
manufacturing-ai-practical/
├── README.md
└── 2주차/
    ├── manufacturing_ai_lab2_1.ipynb   # 실습 2-1: 좋은 특징(Good Feature)과 클래스 분리성
    ├── manufacturing_ai_lab2_2.ipynb   # 실습 2-2: 제약 조건(Constraints)과 일반화
    ├── cwru_normal.mat                 # CWRU 정상(Normal) 베어링 진동 데이터
    └── cwru_fault.mat                  # CWRU 결함(Inner Race Fault) 베어링 진동 데이터
```

## 주차별 실습 내용

| 주차 | 파일 | 주제 | 핵심 개념 |
| :---: | --- | --- | --- |
| 2주차 | `manufacturing_ai_lab2_1.ipynb` | 좋은 특징(Good Feature)의 정의와 클래스 분리성(Separability) 체감 | 패턴/특징의 정의, 나쁜 특징(Mean, 순간값) vs 좋은 특징(RMS, 고주파 스펙트럼 비율), Fisher 분리도 지수, Logistic Regression 분류 성능 비교 |
| 2주차 | `manufacturing_ai_lab2_2.ipynb` | 제약 조건(Constraints)에 따른 일반화(Generalization)와 문제 난이도 비교 | 데이터/환경 제약(노이즈 제거), 모델 제약(선형 구조·L2 정규화·가우시안 가정), 작업 제약(회귀 → 2진 분류 단순화) |

## 데이터

- **CWRU Bearing Dataset**: Case Western Reserve University에서 공개한 모터 베어링 진동 데이터셋
- `cwru_normal.mat` — 정상 상태 진동 신호
- `cwru_fault.mat` — 내륜 결함(Inner Race Fault) 진동 신호
- 노트북과 같은 폴더에 두고 상대 경로로 불러옵니다.

## 실행 방법

1. 저장소를 클론합니다.
   ```bash
   git clone https://github.com/gukim1991/manufacturing-ai-practical.git
   cd manufacturing-ai-practical
   ```
2. 필요한 패키지를 설치합니다.
   ```bash
   pip install numpy scipy matplotlib scikit-learn jupyter
   ```
3. 해당 주차 폴더의 노트북을 Jupyter Notebook 또는 Google Colab에서 열어 실행합니다.
   - Colab에서 실행할 경우 `.mat` 파일을 함께 업로드하세요.

## 진행 현황

- [x] 2주차 — 좋은 특징과 분리성 / 제약 조건과 일반화
- [ ] 3주차
- [ ] 4주차
