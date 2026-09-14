<div align="center">

# Kim Jaehoon

### Software Science @ Dankook University  

</div>

---

## About Me

- 단국대학교 소프트웨어학과 재학
- AI 기능을 실제 애플리케이션에 연결하는 **Backend / Data Pipeline**에 관심
- LLM 단순 호출보다 **입력 수집, 전처리, 구조화, 예외 처리, API 연동**까지 포함한 전체 시스템 흐름을 중요하게 생각
- Java 객체지향 설계, 운영체제, 데이터베이스/스토리지 실험 등 다양한 소프트웨어 프로젝트 경험 보유

---

## Tech Stack

### Languages

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)

### Backend & AI

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI_API-412991?style=flat-square&logo=openai&logoColor=white)
![REST API](https://img.shields.io/badge/REST_API-005571?style=flat-square)
![AsyncIO](https://img.shields.io/badge/AsyncIO-3776AB?style=flat-square&logo=python&logoColor=white)

### Data & Platform

![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![JSON](https://img.shields.io/badge/JSON-000000?style=flat-square&logo=json&logoColor=white)

### Tools

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

---

# Featured Project

## ReSee — AI Smart Archive

> 저장하고 잊어버리는 SNS·웹 콘텐츠를 AI로 분석하고 다시 활용할 수 있도록 만드는 스마트 아카이브

**Dankook University Capstone Design · Team Re:Mind · 2인 팀**  
**2026.03 ~ 2026.05**

[Repository](https://github.com/jimin-21/DKU-2026-REMIND)

### My Role — AI Backend & Data Pipeline

Python/FastAPI 기반의 AI 분석 서버와 콘텐츠 수집·전처리 파이프라인을 담당했습니다.

#### Dual-Pass AI Pipeline
- GPT-4o Vision 기반 OCR/메타데이터 추출과 논리적 요약 단계를 분리
- `title`, `summary`, `shortSummary`, `category`, `tags` 형태의 구조화 JSON 생성
- 원문에 없는 정보 생성을 줄이고 콘텐츠 구조를 최대한 보존하도록 프롬프트 설계

#### Async Multi-Image Processing
- `asyncio.Semaphore`, `asyncio.gather`, `asyncio.to_thread()` 기반 병렬 OCR 처리
- 최대 8개 이미지 동시 분석
- 처리 완료 순서와 관계없이 원본 이미지 순서 복원

#### Smart Grouping
- `sourceAccount`, `captionSnippet`, `carouselInfo`를 기준으로 동일 게시물 이미지 자동 그룹화
- `imageIndexes`로 원본 이미지와 분석 결과 연결
- 누락 이미지 인덱스 탐지 및 보정 로직 구현

#### Robust Data Pipeline
- Naver Blog 본문 파싱 및 Instagram RapidAPI 연동
- 장문 입력을 청크 단위로 분할 → 부분 요약 → 재통합
- SNS 행동 유도 문구 제거 및 번호형 목록·체크리스트 구조 보존
- URL / 이미지 / URL+이미지 입력을 처리하는 FastAPI API 설계

### Service Flow

```text
Link / Screenshots
        ↓
Web Parsing / Vision OCR
        ↓
Preprocessing & Smart Grouping
        ↓
Structured AI Summarization
        ↓
FastAPI JSON Response
        ↓
Flutter Client
        ↓
User-specific Firestore Archive
```

---

# Projects

## MSG Foundation System

**Java · OOAD · UML · Software Architecture**

[Repository](https://github.com/edd1e-kim/MSG-Foundation-System)

Schach의 객체지향 소프트웨어 공학과 Larman의 UML/Pattern 방법론을 기반으로 설계한 **재단 자금 운영 파일럿 시스템**입니다.

- Use Case Diagram, Domain Model, Sequence Diagram 기반 분석 및 설계
- `model / service / view` 계층으로 관심사 분리
- 투자 수익, 운영 비용, 모기지 상환액, 보조금을 반영한 주간 자금 계산 로직 구현
- 7단계 자금 운영 알고리즘 및 주택 구입/재투자 시뮬레이션 구현
- 객체지향 설계 원칙을 실제 Java 코드 구조에 적용

---

## Java Philosophy Dictionary

**Java · OOP · File I/O · CRUD**

[Repository](https://github.com/edd1e-kim/Java-Philosophy-Dictionary)

동양 철학 용어와 한자를 체계적으로 정리하고 학습하기 위해 개발한 Java 애플리케이션입니다.

- 철학 용어 등록·조회·수정·삭제 CRUD
- File I/O 기반 데이터 저장 및 불러오기
- 무작위 용어 추출을 활용한 퀴즈 기능
- 객체지향 구조를 활용한 데이터 관리
- Java 기반 애플리케이션 설계 및 상태 관리 경험

---

## Docker Analysis Team Project

**Docker · Open Source Software · Technical Research**

[Repository](https://github.com/edd1e-kim/25-2-Team-Project-of-Docker-analysis)

오픈소스 소프트웨어 Docker의 **실질적인 가치와 확장 가능성**을 분석한 팀 프로젝트입니다.

- Docker 도입 배경과 필요성 조사
- 실제 활용 사례 및 도입 성과 분석
- 유사 기술/사례 비교
- 컨테이너 기반 개발 환경의 장점과 활용 가능성 정리

> This repository is a fork of the original team repository.

---

# Additional Technical Work

## Operating System Scheduler Simulator

**C++ · Scheduling Algorithms · Systems Programming**

운영체제 스케줄링 알고리즘을 직접 구현하고 테스트한 시뮬레이터입니다.

- Round Robin
- Multi-Level Feedback Queue
- Lottery Scheduling
- Stride Scheduling
- 프로세스별 response time / completion time 비교
- GoogleTest 기반 테스트 환경에서 알고리즘 검증

---

## Flash Translation Layer & Garbage Collection

**C++ · Storage Systems · FTL · Garbage Collection**

SSD의 논리-물리 주소 변환과 Garbage Collection 동작을 구현하고 Write Amplification을 분석했습니다.

- Greedy FTL
- Cost-Benefit FTL
- Logical Page → Physical Page Mapping
- Garbage Collection 및 Block 상태 관리
- Workload별 Write Amplification 비교

---

## RocksDB Performance Experiments

**RocksDB · Benchmarking · Storage Engine**

RocksDB 내부 자료구조와 필터 설정에 따른 성능 차이를 실험했습니다.

- Bloom Filter ON/OFF 비교
- Prefix 기반 False Positive 분석
- SkipList / HashSkipList MemTable 성능 비교
- Zipfian workload 기반 throughput / latency 측정
- 메모리 사용량 및 tail latency 분석

---

## Data Analysis Projects

**Python · Pandas · Matplotlib · Statistical Analysis**

실제 CSV 데이터셋을 기반으로 데이터 전처리와 시각화 실습을 수행했습니다.

- 사용자 행동 데이터 분석
- 만족도 데이터 분석
- 산점도, 히스토그램, 박스플롯, 선 그래프 시각화
- Python 기반 데이터 탐색 및 기초 통계 분석

---

## What I Focus On

```text
Reliable Data Collection
        +
Clear API Design
        +
Structured AI Output
        +
Robust Error Handling
        +
System-level Understanding
        =
Software that can actually be used
```

LLM을 사용하는 것 자체보다,  
**불완전한 입력을 어떻게 수집하고 정제하며 안정적인 결과로 만들어 실제 서비스에 전달할지**에 관심을 두고 개발하고 있습니다.

---

<div align="center">

### Thanks for visiting!

[![GitHub](https://img.shields.io/badge/GitHub-edd1e--kim-181717?style=flat-square&logo=github)](https://github.com/edd1e-kim)

</div>
