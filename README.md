# 전동환 · LETUED

데이터를 모으고, 가설을 세우고, 통계로 검증한다. 안 되는 것은 안 된다고 기록한다.
*Collect data, form hypotheses, verify with statistics — and when the answer is no, write that down too.*

## 대표 프로젝트

### [coinrandom](https://github.com/LETUED/coinrandom) — 시장 데이터 기반 난수 라이브러리
암호화폐 시장의 예측 불가능성을 엔트로피 소스로 쓰는 Python 라이브러리. PyPI 배포·유지보수 중.
*A verifiable random-number library seeded by live crypto-market entropy. Published on PyPI.*

- `pip install coinrandom` — v2.0.1, 엔트로피 소스 7종 (거래소 3 + ETH/BTC/SOL 블록 + Uniswap V3)
- 병렬 I/O로 수집 지연 ~17초 → ~2초, 커넥션 풀링으로 반복 호출 처리량 ~44% 개선
- 오프라인 pytest 매트릭스(Python 3.10–3.13) CI + 태그 푸시 시 OIDC로 PyPI 자동 배포

### [Entropy_Crypto](https://github.com/LETUED/Entropy_Crypto) — 엔트로피 트레이딩 정량 연구
순열 엔트로피(MPE)로 시장의 "질서 구간"을 찾는 전략을 실험 35개로 검증하고, 우위가 통계적으로 성립하지 않음을 확인해 실거래 투입 직전 스스로 종결한 연구.
*A 35-experiment quantitative study that falsified its own edge before real capital was deployed.*

- Walk-forward 6구간, 순열검정 10,000회, 블록 부트스트랩 5,000회, LightGBM+SHAP 피처 분석
- 초기 Sharpe +1.391이 측정 인플레이션임을 거래단위 재측정으로 자가 규명 — 반증 과정 전체가 [RESEARCH_LOG](https://github.com/LETUED/Entropy_Crypto/blob/main/docs/RESEARCH_LOG.md)에 기록돼 있음

### [LETRADE_V1](https://github.com/LETUED/LETRADE_V1) — 마이크로서비스 트레이딩 시스템
기존 프레임워크 없이 메시지버스 기반으로 밑바닥부터 설계한 자동거래 인프라.
*A from-scratch microservice trading system — RabbitMQ, PostgreSQL, CCXT, FastAPI.*

- 거래 실행 경로 0.86ms 실측, 메시지 처리량 15,000 msg/s, 24시간 연속 테스트 가용성 99.9%
- 서비스 6종 (Core Engine / Strategy Worker / Capital Manager / Exchange Connector 외), 테스트 232케이스

## 프로젝트 인덱스

| 시기 | 프로젝트 | 한 줄 |
|---|---|---|
| 2026 | [Thesis](https://github.com/LETUED/Thesis) | 투자판단 SaaS — FastAPI + Supabase + Stripe (개발 중) |
| 2026 | [polymarket-bot](https://github.com/LETUED/polymarket-bot) | 예측시장 엣지 검증 드라이런 프레임워크 — 프랙셔널 켈리, Brier 판정 |
| 2026 | [D_QR](https://github.com/LETUED/D_QR) | 다차원 QR 코드 연구 — 육각 격자, RS 소거정정, 점진 공개 |
| 2026 | [Entropy_Crypto](https://github.com/LETUED/Entropy_Crypto) ★ | 엔트로피 트레이딩 정량 연구 (위) |
| 2026 | [coinrandom](https://github.com/LETUED/coinrandom) ★ | 시장 데이터 기반 난수 라이브러리, PyPI (위) |
| 2025 | [LETRADE_V1](https://github.com/LETUED/LETRADE_V1) ★ | 마이크로서비스 트레이딩 시스템 (위) |
| 2025 | [crypto-trader-bot](https://github.com/LETUED/crypto-trader-bot) | Freqtrade 듀얼 전략 봇 — 48조합 백테스트, Docker/Telegram |
| 2024 | [CCProject](https://github.com/LETUED/CCProject) | CI/CD 자동화 CLI — PyPI `ci-cd-tool`, 캡스톤 |
| 2024 | [PCBS](https://github.com/LETUED/PCBS) | 코인 백테스트 시스템 — backtrader 백엔드 + React 대시보드 |
| 2023 | [thefish_src](https://github.com/LETUED/thefish_src) | AI 어종 분류 데스크톱 앱 — ResNet50 전이학습 + PyQt5 + SQLite 백과사전 |

## 연락처

woo9910203626@gmail.com,dglsts5387@naver.com
