# AI-based Phishing Message Detection System

## 1. Project Overview

본 프로젝트는 인공지능 기반 텍스트 분류 모델을 활용하여 피싱 메시지를 탐지하는 시스템 구현을 목표로 한다.

최근 피싱 및 스팸 메시지는 실제 사용자 메시지와 유사한 형태로 진화하고 있으며, 단순 키워드 기반 필터링만으로는 탐지에 한계가 존재한다. 이를 해결하기 위해 TensorFlow 기반 딥러닝 모델을 활용하여 메시지 데이터를 학습하고, 피싱 여부를 자동으로 분류하는 시스템을 구현하였다.

또한 단순 분류 결과뿐만 아니라 위험도를 확률 형태로 출력하여 메시지의 위험 가능성을 보다 직관적으로 분석할 수 있도록 구성하였다.

---

# 2. System Architecture

텍스트 입력
→ 데이터 전처리
→ 텍스트 벡터화(Vectorization)
→ TensorFlow 기반 분류 모델 학습
→ 피싱 여부 예측
→ 위험도 출력
→ 성능 평가 및 시각화

본 프로젝트에서는 TensorFlow 기반 텍스트 분류 모델을 활용하였으며, Epoch 변화에 따른 성능 비교 실험과 Accuracy 그래프, Confusion Matrix를 통한 모델 평가를 함께 진행하였다.

---

# 3. AI Tool Usage Strategy (Prompting Log)

## 사용한 AI 도구

* ChatGPT
* GitHub

## AI 활용 전략

AI 도구를 단순 코드 자동 생성기로 사용하는 것이 아니라, 프로젝트 진행 과정에서의 가상 협업 도구 형태로 활용하였다.

특히 TensorFlow 코드 구조 이해, 실험 설계, 오류 수정, 성능 비교 및 시각화 과정에서 AI 도구를 활용하였으며, 결과를 직접 비교 및 수정하며 프로젝트를 진행하였다.

## 주요 활용 내용

* TensorFlow 텍스트 분류 코드 구조 분석
* Epoch 변화에 따른 성능 비교 실험 설계
* Accuracy 시각화 그래프 구현
* Confusion Matrix 기반 모델 평가 분석
* 위험도 확률 출력 기능 구현
* README 및 발표 자료 정리

## 주요 프롬프트 예시

* "학습 횟수(Epoch)를 변경했을 때 성능 차이를 비교하는 코드를 작성해줘."
* "Accuracy 그래프를 시각화하는 방법을 알려줘."
* "Confusion Matrix를 활용한 모델 평가 코드를 작성해줘."
* "위험도를 확률 형태로 출력하는 방법을 알려줘."

---

# 4. Experimental Results

## Accuracy Comparison

| Epoch | Accuracy |
| ----- | -------- |
| 3     | 0.90     |
| 5     | 0.98     |

Epoch 값을 증가시킴에 따라 모델 정확도가 향상되는 경향을 확인할 수 있었다.

## Model Evaluation

* Accuracy 그래프를 활용하여 Epoch별 성능 변화를 시각적으로 비교하였다.
* Confusion Matrix를 활용하여 모델의 분류 성능을 추가적으로 분석하였다.
* 위험도 확률 출력 기능을 통해 메시지별 위험 가능성을 수치 형태로 표현하였다.

---

# 5. How to Run

1. Google Colab에서 ipynb 파일 실행
2. TensorFlow, pandas, matplotlib, sklearn 라이브러리 설치 확인
3. 코드 셀을 위에서부터 순차적으로 실행
4. 모델 학습 및 결과 출력 확인
5. Accuracy 그래프 및 Confusion Matrix 결과 확인

---

# 6. Troubleshooting

## 문제점

* TensorFlow 및 Colab 환경 사용 경험 부족
* 코드 실행 구조와 데이터 흐름 이해의 어려움
* 단순 모델 사용만으로는 프로젝트 차별성이 부족하다는 문제

## 해결 과정

* AI 도구를 활용하여 코드 구조를 단계별로 분석
* Epoch 비교 실험 추가
* Accuracy 그래프 및 Confusion Matrix 기반 평가 기능 추가
* 위험도 확률 출력 기능 구현

---

# 7. Limitations and Future Work

본 프로젝트는 공개 데이터셋 기반으로 진행되었기 때문에 실제 피싱 환경의 다양한 패턴을 완벽히 반영하지는 못한다.

향후에는 실제 피싱 데이터 기반 실험, 다양한 딥러닝 모델 비교, Precision 및 Recall 기반 성능 분석 등을 추가적으로 진행할 예정이다.

또한 실제 서비스 환경에 적용 가능한 형태의 실시간 탐지 시스템으로 확장하는 방향을 고려하고 있다.
