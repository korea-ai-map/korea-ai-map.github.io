# 변경 이력 (Changelog)

이 파일은 **스키마·정책·구조**의 변경을 기록합니다.
개별 데이터 항목의 변경 이력은 Git 커밋 히스토리로 보존됩니다.

형식은 [Keep a Changelog](https://keepachangelog.com/), 버전은 데이터 스냅샷 기준 `YYYY.MM`을 사용합니다.

## [2026.08]

### Added
- **Kanana-2 SLM 공개 모델**: 3B·1.3B의 Base/Instruct 모델 4종을 공식 기술 블로그와 Hugging Face 모델 카드 기준으로 추가.
- **BC Card 금융 AI 자산**: 금융 LLM 800문항 벤치마크·회귀 테스트 골든셋·한영 금융 개인정보 탐지 데이터셋을 추가.
- **최신 국내 기반모델**: Solar Pro 4, A.X K2·ALM·VE, A.X K2 Raon-Speech, K-EXAONE 2.0, Motif-3 Beta·Vision Encoder·Audio를 공식 문서와 모델 카드 기준으로 추가.
- **신규 기술보고서**: A.X K2, A.X K2 ALM, K-EXAONE 2.0 기술보고서를 모델·개발 조직과 연결.
- **Motif 3 정식 공개**: 정식 포스트트레이닝 모델과 Base 체크포인트, 기술보고서를 추가하고 Beta를 보관 상태로 전환.
- **NOLLI 평가 자산**: 영어-한국어 추론 격차를 진단하는 벤치마크·데이터셋·평가 코드·논문을 연결해 추가.
- **NAVER AI Lab OPD²**: 다국어 수학 추론 델타 증류 논문과 Apache-2.0 공식 구현을 추가.
- **체화형 AI 안전 평가**: AIM Intelligence·서울대의 EgoSafetyBench 벤치마크·영상 데이터·평가 코드·논문을 연결해 추가.
- **신규 국내 연구**: KAIST DISLab의 스트리밍 대화 요약 메모리 ReMEMBER 논문을 추가하고 Motif 3 기술보고서의 arXiv 정식 공개를 반영.
- **산업 특화·음성 모델**: EXAONE Tabular·Forecast, Solar Embedding 2, Raon-OpenTTS-1B과 학습 데이터 풀을 공식 문서 기준으로 추가.
- **한국어 특화 후속학습**: 비씨카드 MoAI-Privacy-Filter와 유니바 Qwen3-ASR 한국어 Beta를 학습 기여·공개 가중치 근거와 함께 추가.
- **신규 도구·제품**: Nari Qwen3-TTS 실시간 추론 도구와 코난테크놀로지 Agent-X 엔터프라이즈 플랫폼을 추가.
- **최신 국내 연구**: MoE 학습률 전이 연구, PolicyGuide, SafeBranch, ReWEIGH, LT-Mem, GraniKV, TRACER 논문 7건을 국내 기관 소속과 arXiv 원문 기준으로 추가.
- **한국어 평가 자산**: 래블업의 RouterBench·τ²-bench 한국어 번역판과 써로마인드의 한국어 RAG QA를 데이터셋·벤치마크로 연결하고 두 개발사를 추가.
- **시각 문서 검색 자산**: KoViDoRe 벤치마크와 Ko-VDR Train Public 학습 데이터를 논문과 함께 연결.
- **오픈소스 갱신**: AutoRAG 2.3의 피드백 학습·클라우드 연결·중복 관리 기능을 반영하고 메타데이터를 TypeScript·MIT 기준으로 정정. ReCurveflow와 LG AI연구원의 GBDT 유도 조각별 선형 임베딩 공식 구현을 추가.
- **신규 국내 연구**: 개인화 프라이버시, 사회공학 공격 탐지, 화학 전이상태 예측, 시각 문서 검색, LLM 추천, 단백질 결합체 선별, 영상 이상 탐지, 얼굴인식 보안, 다중시점 깊이, GNN 불확실성 논문 10건을 국내 기관 소속과 원문 기준으로 추가.
- **데이터 확충**: 조직 145 · 모델 175 · 제품 78 · 오픈소스 56 · 데이터셋 124 · 벤치마크 26 · 논문 261 (합계 865).

## [2026.07]

### Added
- **`papers` 컬렉션 신설** (7번째 컬렉션): 한국 기관 주도 논문. `title`, `authors_org`, `venue`, `year`, `arxiv_id`, `related_ids`(조직/모델 참조) 등. arXiv 실존 검증 기반.
- **models 스키마 확장**: `base_model`(파생 관계), `benchmark_results[]`(`{benchmark, score, metric?, source?}`).
- **웹 기능**: 홈 통합검색, 다차원 필터·정렬, 4개 항목 비교, 검증 상태 배지 툴팁, 최근 업데이트 일시 표기.
- **조직 페이지**: 상세에 개발 모델·제품·오픈소스·관련 논문 섹션. 목록에 모델/오픈소스/논문 보유 필터 + 연결 개수 칩.
- **SEO**: 사이트맵, JSON-LD, OG/Twitter, canonical, robots.txt, llms.txt.
- **데이터 확충**: 조직 140 · 모델 130 · 제품 71 · 오픈소스 50 · 데이터셋 114 · 벤치마크 19 · 논문 236 (합계 760).
- **AI Hub 세분화**: 한국어 카탈로그의 공식 상세 항목 68건을 `dataSetSn`별 데이터셋으로 추가하고, KsponSpeech를 상세 페이지와 연결.
- **신규 생태계 항목**: K-EXAONE·Solar Pro 3·Solar Open 2·KRAFTON Raon 모델군, KoBALT·KRETA·KVoiceBench 계열, Nota AI·Liner와 제품·논문을 공식 출처로 추가.
- **2026년 공개 자산 보강**: K-BrowseComp·KoALa-Bench와 데이터·평가 코드·논문, TeamSparta AX의 K-AX Spartan OSS 27B, BC Card의 MoAI 임베딩 모델·금융 검색 데이터를 공식 출처로 추가.

### Changed
- `models.organization_id`를 필수로 강제 (org 없는 모델은 개발사 조직을 먼저 등재).
- 출처 유형을 enum으로 제한하고, 조직의 모델·제품 역참조를 자식 `organization_id` 기준으로 동기화.
- 링크 점검을 URL 단위로 중복 제거하고 병렬화해 전체 검증 시간을 단축.
- 생태계 지도·타임라인 페이지 제거 (실효성 낮음).

### Fixed
- Astro glob 로더의 id 점(`.`) 제거로 인한 파일명/URL/참조 불일치 → 모델 id에서 점 제거로 통일.
- 내부 `id`보다 파일명을 정규 ID로 사용하고, AI Hub `dataSetSn` 중복과 조직 역참조 불일치를 자동 검출.
- 빈 모델 라이선스명과 잘못 분류된 출처 유형·신뢰도 표기를 교정.
- 이전·합병·경로 변경으로 끊긴 N.THING·SAPEON·Vrew·Bllossom·KcBERT 링크를 현재 공식 출처로 교체.
- 필터가 카드를 숨기지 못하던 문제 → 전역 `[hidden]{display:none!important}`.
- 전역 ID 충돌 해소 규칙(컬렉션 간 유일성) 적용: `ko-reranker-bge`, `klue-project`.

## [Phase 0]

### Added
- Phase 0 리포 뼈대: 디렉터리 구조, zod 스키마 6종, 검증/빌드 스크립트, Issue Form, 자동화 워크플로우
- 문서: README, METHODOLOGY, CONTRIBUTING, GOVERNANCE, DATA_LICENSE, CODE_OF_CONDUCT
- 샘플 데이터: 조직 1건, 모델 1건
