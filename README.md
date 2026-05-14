# 생성형 AI 기반 PCB 초정밀 불량 탐지

## 프로젝트 개요
- **참여 형태**: 학부연구생
- **프로젝트 기간**: 2024년 겨울방학 ~
- **목표**: 생성형 AI를 활용한 PCB 불량 이미지 생성 및 이상 탐지 성능 향상

## 문제 정의
> 여기에 작성: PCB 불량 탐지에서 왜 생성형 AI가 필요한지,
> 기존 이상 탐지 방법의 한계가 무엇인지 2~3줄로 작성

---

## 실험 과정

### Stage 1 — SeaS 적용 (미채택)
> 여기에 작성: SeaS를 선택한 이유 한 줄

- 논문: [SeaS: Few-shot Industrial Anomaly Image Generation with Separation and Sharing Fine-tuning](논문 링크)
- 코드 참고: [https://github.com/HUST-SLOW/SeaS](https://github.com/HUST-SLOW/SeaS)

**실험 결과**
| 지표 | 수치 |
|------|------|
| (지표명) | (수치) |

![SeaS 결과 시각화](이미지경로)

**결론**: VisA PCB 데이터에 적용 시 성능이 불충분하여 미채택
> 여기에 작성: 왜 성능이 안 좋았는지 원인 분석 1~2줄

---

### Stage 2 — CDAD 원본 적용
> 여기에 작성: SeaS 실패 후 CDAD를 선택한 이유 한 줄

- 논문: [One-for-More: Continual Diffusion Model for Anomaly Detection](논문 링크)
- 코드 참고: [https://github.com/FuNz-0/One-for-More](https://github.com/FuNz-0/One-for-More)

**실험 결과**
| 지표 | 수치 |
|------|------|
| (지표명) | (수치) |

![CDAD 원본 결과](이미지경로)

📄 [상세 결과 보기 (PDF)](PDF파일경로)

---

### Stage 3 — CDAD 변형 (결함 이미지 생성)
> 여기에 작성: 원본 CDAD를 변형하게 된 이유 한 줄
> (원본은 정상+결함 → 정상 생성, 변형은 정상+결함 → 결함 생성으로 수정)

- 베이스 코드: [https://github.com/FuNz-0/One-for-More](https://github.com/FuNz-0/One-for-More)

**변형한 부분**
> 여기에 작성: 구조에서 어떤 부분을 어떻게 수정했는지 2~3줄

**실험 결과**
| 모델 | 지표 | 수치 |
|------|------|------|
| CDAD 원본 | (지표명) | (수치) |
| CDAD 변형 | (지표명) | (수치) |

![CDAD 변형 결과](이미지경로)

📄 [발표자료 보기 (PDF)](PDF파일경로)

---

## 실험 결과 요약
| 단계 | 모델 | 결과 | 채택 여부 |
|------|------|------|----------|
| Stage 1 | SeaS | (수치) | ❌ 미채택 |
| Stage 2 | CDAD 원본 | (수치) | ✅ 채택 |
| Stage 3 | CDAD 변형 | (수치) | ✅ 최종 적용 |

🏆 경진대회 제출 완료 (결과 업데이트 예정)

---

## 한계 및 개선 방향
**한계**
- 여기에 작성: 현재 결과의 한계점 2~3가지

**개선 방향**
- 여기에 작성: 향후 개선하고 싶은 방향 2~3가지

---

## 환경
- OS: Windows / Linux (GPU 서버)
- 주요 라이브러리: (사용한 것들 작성)

---

## 참고 자료

### SeaS
- 논문: [SeaS: Few-shot Industrial Anomaly Image Generation with Separation and Sharing Fine-tuning](논문 링크)
- 코드: [https://github.com/HUST-SLOW/SeaS](https://github.com/HUST-SLOW/SeaS)

### CDAD
- 논문: [One-for-More: Continual Diffusion Model for Anomaly Detection](논문 링크)
- 코드: [https://github.com/FuNz-0/One-for-More](https://github.com/FuNz-0/One-for-More)
