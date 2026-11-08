# Portfolio

## Core Competency

### LLM 엔지니어링
- 비용/성능을 고려한 프롬프트와 출력 스키마, 제약 조건 설계 경험.
- 캐싱 적용과 토큰 사용량 추적을 통한 LLM 비용 관리 경험 (토큰 비용 70% 절감).
- LLM으로 학습 콘텐츠(커리큘럼, 문제)를 생성하는 파이프라인과 비동기 작업 처리 설계 경험.
- AI 에이전트를 위한 동적 함수 호출 아키텍처 구현 경험.

### EDA, 데이터 분석, ML/DL 모델링
- 석사 논문의 문제 해결 과정에서 EDA, 데이터 수집, 정제, 모델링, 문제 해결 방안 도출 과정 경험.
- Tableau, Matplotlib 등의 시각화 도구로 분석 결과 시각화 경험.
- 주요 CNN/LLM 논문들의 [PyTorch 코드 구현](https://github.com/2p990i9hpral/pytorch_paper_implementation) 경험.
- DB 설계, SQL을 통한 데이터 처리 경험.

### 프로그래밍, 데이터 수집, ML 모델 배포
- AWS상 머신러닝 API 서버 구축 경험.
- Python, Selenium을 통해 웹상 정형/비정형 데이터 수집, 정제 경험.
- 브라우저 확장 프로그램(Manifest V3), Userscript 개발 경험.
- Docker, Git 등 프로그래밍 관련 기반기술 사용 경험.

## Projects

### [LLM 기반 학습 콘텐츠 생성 설계와 언어 학습 서비스 기능 개발](https://github.com/2p990i9hpral/Portfolio/blob/main/projects/language_platform.md)
- 학습 커리큘럼과 문제를 LLM이 생성할 수 있도록 프롬프트, 출력 스키마, 제약 조건 설계.
- 커리큘럼 생성 방식 2가지(한 번에 생성 / 단계별 생성)를 응답 시간과 단어 중복 방지 측면에서 비교, 한 번에 생성 방식 채택.
- 비동기 LLM 작업의 응답 시간 분포를 고려해 상태 조회 주기(적응형 폴링) 설계.
- Anki 스타일 SRS 스케줄링, 학습 통계 대시보드, 학습 서비스 보조 도구(Lesson Importer, Navigator) 구현.

### [LLM 기반 언어 학습 도구 개발](https://github.com/2p990i9hpral/LingQ_Add-On)
- LLM을 활용해 AI 단어 사전, CEFR 난이도별 레슨 요약, 채팅 위젯 구현.
- 최근 학습한 단어를 LLM으로 분석해 난이도, 주제 흐름, 표현 패턴을 정리하는 AI 학습 리포트 구현.
- 토큰 종류별 사용량과 비용 추적 구현. 효율적인 캐싱 구현으로 토큰 비용 70% 절감.
- AI 플래시카드 생성, 저장과 Anki 동기화 구현.

### [LLM 기반 AI 에이전트 개발](https://github.com/2p990i9hpral/Portfolio/blob/main/projects/llm_powered_ai_agent.md)
- 자연어 이해, 추론 및 응답 생성을 위해 OpenAI 호환 LLM API 활용.
- LLM이 사용자 요청에 필요한 외부 API를 호출하는 동적 함수 호출 아키텍처 구현.
- 로컬 데이터베이스를 사용하여 대화 기록, 사용자 통계, 내부 로깅, LLM 토큰/비용 추적과 관리.

### [NLP 기반 언어 학습 데이터 분석 및 시각화, 개인화된 학습 추천](https://forum.lingq.com/t/lingq-data-analysis-visualizing-patterns-in-my-known-words/1410961?u=vet8t6z79pc4)
- NLP 기법을 통해 대규모 개인 언어 학습 데이터 전처리, 품사 빈도 분석.
- 데이터를 기반으로 학습 패턴 통계 도출, 미지 단어 식별을 통한 학습 우선순위 도출.
- 단어 임베딩 시각화, 어휘 토픽 맵 구축, 학습자 맞춤형 토픽 기반 어휘 학습 추천 시스템 프로토타입 설계.

### [영상 내 개인정보 비식별화 서비스 개발](https://github.com/2p990i9hpral/Portfolio/blob/main/projects/personal_info_making.md)
- 자체 데이터셋을 사용하여 영상 내 얼굴, 차량 번호판 등 개인정보 인식 모델 학습.
- 추론 프로세스를 Docker 이미지화, AWS ECS/Batch를 활용한 API 서버 구축, 웹 기반 사용자 UI 개발.

### [통합 OTT 콘텐츠 순위 제작](https://github.com/2p990i9hpral/Portfolio/blob/main/projects/ott_ranking.md)
- Netflix, TVING, Wavve, Disney+의 콘텐츠 일간 순위 수집.
- 수집된 순위 데이터와 인터넷 언급량 데이터를 기반으로 통합 콘텐츠 순위 제작.

### [스마트폰 발주 추천모델 구축](https://github.com/2p990i9hpral/Portfolio/blob/main/projects/phone_recommendation.md)
- 핸드폰 커뮤니티들의 게시물 실시간 수집.
- 수집된 게시물 전처리, 주요 키워드 추출 후 시각화 대시보드 제작.
- 주요 키워드를 바탕으로 제품, 개통유형별 선호도 분석, 모델 발주 추천.

## Research

### [혈액 수요/공급 구조 분석](https://github.com/2p990i9hpral/Factors_Dominating_Blood_Supply_Dynamics) (석사 학위논문)
- 시계열 분석 방법론 기반 위기 상황 시 혈액 수요/공급량 모델링.
- 헌혈 참여자 특성에 따른 프로모션의 정량적 효과 측정.
- 분석 결과 시각화, 효율적인 프로모션 수행 방안 제시.

---

- [Tech Blog](https://obsidian-79x.pages.dev/)
- [Google Scholar](https://scholar.google.com/citations?user=iXWBhc0AAAAJ)
