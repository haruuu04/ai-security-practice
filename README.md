# AI-based Phishing Message Detection

## 1. Project Overview

본 프로젝트는 AI 기반 텍스트 분류 모델을 활용하여 피싱 메시지를 자동으로 탐지하는 시스템 구현을 목표로 한다.
TensorFlow 기반의 간단한 신경망 모델을 사용하여 정상 메시지와 스팸 메시지를 분류하였으며, 위험도를 확률 형태로 출력하도록 구현하였다.

---

## 2. System Architecture

텍스트 입력
→ 데이터 전처리
→ 텍스트 벡터화
→ TensorFlow 기반 분류 모델
→ 정상 / 피싱 분류 결과 출력
→ 위험도 확률 출력

---

## 3. AI Tool Usage Strategy (Prompting Log)

### 사용한 AI 도구

* ChatGPT

### 주요 활용 내용

* TensorFlow 텍스트 분류 코드 생성 및 구조 이해
* 학습 횟수(Epoch) 변경 실험 설계
* 위험도 확률 출력 기능 구현
* 오류 분석 및 디버깅
* 발표 자료 및 문서화 지원

### 주요 프롬프트 예시

* “학습 횟수를 변경했을 때 성능 차이를 비교하는 코드를 작성해줘.”
* “모델 출력값을 활용하여 위험도를 확률 형태로 출력하는 방법을 알려줘.”
* “최종 발표용 README 구조를 작성해줘.”

---

## 4. Experimental Results

| Epoch | Accuracy |
| ----- | -------- |
| 3     | 0.90     |
| 5     | 0.98     |

학습 횟수를 증가시킴에 따라 모델 정확도가 향상되는 경향을 확인하였다.

---

## 5. How to Run

1. Google Colab에서 ipynb 파일 실행
2. TensorFlow 및 pandas 라이브러리 설치 확인
3. 전체 코드 셀 순차 실행
4. 모델 학습 및 결과 확인

---

## 6. Troubleshooting

### 문제점

* TensorFlow 및 Colab 환경 사용 경험 부족
* 코드 구조와 실행 흐름 이해의 어려움
* 단순 모델 사용만으로는 차별성이 부족하다는 문제

### 해결 과정

* AI 도구를 활용하여 코드 흐름을 단계별로 분석
* 학습 횟수 비교 실험 추가
* 위험도 확률 출력 기능 구현

---

## 7. Future Work

* 추가 데이터셋 활용
* Precision 및 Recall 기반 성능 분석
* 다양한 모델 구조 비교 실험
* Git 기반 프로젝트 관리 강화
