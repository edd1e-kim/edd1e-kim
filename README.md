<div align="center">

# Kim Jaehoon

### Software Science @ Dankook University

### Software Engineering · Backend · Cloud / Infrastructure Fundamentals

특정 분야를 일찍 좁히기보다,  
**소프트웨어 공학의 기초와 실제 서비스 개발 경험을 폭넓게 쌓아가고 있습니다.**

현재는 일본에서의 취업을 목표로  
**CS 기초 · Java/Python · Backend · Cloud/Container · Team Project** 역량을 함께 준비하고 있습니다.

</div>

---

## About Me

- 단국대학교 소프트웨어학과 재학
- 아직 하나의 세부 직무로 진로를 고정하기보다 다양한 소프트웨어 개발 경험을 쌓는 중
- Java와 Python을 활용한 애플리케이션 및 백엔드 개발 경험
- 팀 프로젝트에서 **기획 → 설계 → 구현 → 테스트 → 문서화**까지 전체 개발 흐름 경험
- 새로운 기술을 단순히 사용하는 데 그치지 않고, 실제 서비스 흐름 안에서 어떻게 연결되는지 이해하는 것을 중요하게 생각
- 일본 취업을 목표로 기술 역량과 커뮤니케이션 역량을 함께 준비 중

---

## Currently Building

일본 IT 취업을 준비하면서 다음 영역을 균형 있게 강화하고 있습니다.

- **Computer Science Fundamentals** — 자료구조, 알고리즘, 운영체제, 데이터베이스, 네트워크
- **Programming** — Java, Python
- **Backend Development** — REST API, FastAPI, 데이터 처리 및 외부 서비스 연동
- **Cloud & Infrastructure** — Docker 및 클라우드 환경에 대한 이해
- **Team Development** — Git/GitHub 기반 협업, 문서화, 역할 분담
- **Technical Communication** — 프로젝트를 코드뿐 아니라 README, 설계 문서, 발표를 통해 설명하는 능력

---

## Tech Stack

### Languages

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)

### Backend & Application

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![REST API](https://img.shields.io/badge/REST_API-005571?style=flat-square)
![OpenAI](https://img.shields.io/badge/OpenAI_API-412991?style=flat-square&logo=openai&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)

### Development Environment

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)

---

# Featured Project

## ReSee — AI Smart Archive

> 저장하고 잊어버리는 SNS·웹 콘텐츠를 AI로 분석하고 다시 활용할 수 있도록 만드는 스마트 아카이브

**Dankook University Capstone Design · Team Re:Mind · 2인 팀**  
**2026.03 ~ 2026.05**

[View Repository](https://github.com/jimin-21/DKU-2026-REMIND)

### My Role — AI Backend & Data Pipeline

Python/FastAPI 기반의 AI 분석 서버와 콘텐츠 수집·전처리 파이프라인을 담당했습니다.

- GPT-4o Vision 기반 OCR과 논리적 요약을 분리한 **Dual-Pass AI Pipeline**
- `title`, `summary`, `shortSummary`, `category`, `tags` 형태의 구조화 JSON 생성
- `asyncio.Semaphore`, `asyncio.gather`를 이용한 다중 이미지 병렬 처리
- 여러 스크린샷을 게시물 단위로 묶는 **Smart Grouping**
- Naver Blog / Instagram 콘텐츠 수집 및 전처리
- 장문 콘텐츠 Chunking 및 재통합 요약
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
FastAPI
        ↓
Flutter Client
        ↓
User-specific Firestore Archive
```

---

# Projects

## MSG Foundation System

**Java · OOAD · UML · Software Architecture**

[View Repository](https://github.com/edd1e-kim/MSG-Foundation-System)

Schach와 Larman의 객체지향 소프트웨어 공학 방법론을 기반으로 설계한 Java 파일럿 시스템입니다.

- Use Case, Domain Model, Sequence Diagram 기반 분석 및 설계
- `model / service / view` 구조로 관심사 분리
- 투자 수익, 운영 비용, 모기지 상환 등을 반영한 비즈니스 로직 구현
- 객체지향 분석·설계 결과를 실제 Java 코드 구조로 연결

---

## Java Philosophy Dictionary

**Java · OOP · File I/O · CRUD**

[View Repository](https://github.com/edd1e-kim/Java-Philosophy-Dictionary)

동양 철학 용어와 한자를 관리하고 학습하기 위한 Java 애플리케이션입니다.

- 철학 용어 등록·조회·수정·삭제 CRUD
- File I/O 기반 데이터 저장 및 불러오기
- 무작위 용어를 이용한 퀴즈 기능
- Java 객체지향 구조를 활용한 데이터 관리

---

## Docker Analysis Team Project

**Docker · Open Source Software · Technical Research**

[View Repository](https://github.com/edd1e-kim/25-2-Team-Project-of-Docker-analysis)

Docker의 실질적인 가치와 확장 가능성을 분석한 오픈소스 소프트웨어 팀 프로젝트입니다.

- Docker 도입 배경과 필요성 조사
- 실제 활용 사례와 도입 효과 분석
- 관련 기술 및 사례 비교
- 컨테이너 기반 개발 환경의 장점과 활용 가능성 정리


---

## What I Value

```text
Strong Fundamentals
        +
Practical Development Experience
        +
Clear Communication
        +
Continuous Learning
        =
A Better Software Engineer
```

아직 특정 분야 하나로 진로를 한정하기보다,  
**탄탄한 CS 기초와 다양한 프로젝트 경험을 바탕으로 문제를 해결할 수 있는 사람**로 성장하는 것을 목표로 하고 있습니다.

---

<div align="center">

### 방문해주셔서 감사합니다!
### ご覧いただきありがとうございます!
### Thanks for visiting!


[![GitHub](https://img.shields.io/badge/GitHub-edd1e--kim-181717?style=flat-square&logo=github)](https://github.com/edd1e-kim)

</div>
