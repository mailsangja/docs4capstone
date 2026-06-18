<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=200&section=header&text=메일상자&fontSize=80&fontColor=ffffff&animation=twinkling&fontAlignY=38&desc=AI%20기반%20다중%20계정%20메일%20인박스%20자동화%20서비스&descAlignY=62&descSize=20&descColor=d0e8ff" />

<br/>

[![GitHub org](https://img.shields.io/badge/GitHub-mailsangja-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/mailsangja)
&nbsp;
[![AJOU](https://img.shields.io/badge/AJOU%20SOFTCON-2026--1-0057A8?style=flat-square&logo=academia&logoColor=white)](https://softcon.ajou.ac.kr/works/works.asp?uid=2298)
&nbsp;
![MAU](https://img.shields.io/badge/MAU-200%2B-brightgreen?style=flat-square&logo=googlegmail&logoColor=white)
&nbsp;
![Service](https://img.shields.io/badge/Service-Live-success?style=flat-square&logo=vercel&logoColor=white)
&nbsp;

<br/>

> **여러 Gmail 계정, 이제 하나로 관리하세요.**  
> AI가 라벨을 분류하고, RAG가 맞춤 답장 초안을 작성해드립니다.

<br/>

[![Service](https://img.shields.io/badge/🌐%20서비스%20바로가기-mail.ajou.app-4A90E2?style=for-the-badge)](https://mail.ajou.app/)

</div>

---

## 🏆 수상 내역

<div align="center">

| 시상식 | 수상 | 날짜 |
|:---:|:---:|:---:|
| 🥉 아주대학교 **SOFTCON 2026-1** | **장려상 (3등)** | 2026.06.11 |
| 🌟 아주대학교 **SOFTCON 2026-1** | **인기상** | 2026.06.11 |

> **SOFTCON** — 아주대학교 소프트웨어학과 졸업작품 전시회  
> [SOFTCON 2026-1 작품 페이지](https://softcon.ajou.ac.kr/works/works.asp?uid=2298)

</div>

---

## 🔥 서비스 개요

메일상자는 여러 Gmail 계정을 하나의 인박스에서 통합 관리하고, AI 기반 자동 라벨링과 RAG 기반 답장 초안 생성을 제공하는 메일 관리 자동화 서비스입니다.

사용자는 여러 계정을 오가며 메일을 확인할 필요 없이 하나의 화면에서 메일을 조회할 수 있으며, AI가 메일의 성격을 분석해 라벨을 제안하고 중요 메일 관리, 필터링, 알림 설정, 민감정보 관리까지 연결할 수 있습니다.

<table>
  <tr>
    <th align="center" width="100">구분</th>
    <th>내용</th>
  </tr>
  <tr>
    <td align="center">🎯 <b>Target</b></td>
    <td>여러 Gmail 계정을 동시에 관리해야 하는 사용자</td>
  </tr>
  <tr>
    <td align="center">😣 <b>Problem</b></td>
    <td>빠른 인박스 전환의 어려움 &nbsp;·&nbsp; 중요 메일 누락 &nbsp;·&nbsp; AI 환경설정 비용 부담 &nbsp;·&nbsp; 메일 관리 효율성 저하</td>
  </tr>
  <tr>
    <td align="center">✅ <b>Solution</b></td>
    <td><b>다중 계정 인박스</b> + <b>AI 자동 라벨링</b> + <b>AI 자동 답장</b></td>
  </tr>
  <tr>
    <td align="center">💡 <b>POD</b></td>
    <td>다중 계정·벤더 통합 인박스, RAG·LLM 기반 개인화 메일 분류·작성 자동화</td>
  </tr>
</table>

---

## 🚀 핵심 기능 (서비스 상세 소개)

### 📥 다중 Gmail 계정 통합 인박스

여러 Gmail 계정을 하나의 화면에서 조회할 수 있는 통합 인박스를 제공합니다.  
사용자는 계정을 반복해서 전환하지 않아도 전체 메일 흐름을 한 번에 확인할 수 있습니다.

- Gmail OAuth 기반 계정 연동 (서비스 로그인과 별도로 인박스 접근 권한 확보)
- 계정별 메일 동기화 및 통합 조회
- 메일 계정 단위 필터링 및 검색 지원
- Thread 단위 메일 묶음 보기

### 🏷️ AI 기반 자동 라벨링

메일 제목, 본문, 발신자 정보를 기반으로 AI가 적절한 라벨을 자동 제안합니다.  
제안된 라벨은 필터링, 알림 설정, 민감정보 관리 정책과 연결하여 메일 관리 자동화의 기준으로 활용할 수 있습니다.

- LLM 기반 메일 내용 분석 후 라벨 자동 추천
- 사용자 정의 라벨 + 라벨 그룹 관리
- 라벨 기반 필터링 및 실시간 알림 정책 연동
- 과거 메일 일괄 재분류 (Debounce + Rate Limit 제어)

### ✉️ RAG 기반 맞춤 답장 초안 생성

사용자의 기존 메일 작성 패턴을 벡터화하고, 유사한 메일 맥락을 검색하여 개인화된 답장 초안을 생성합니다.

- 사용자 메일 패턴 기반 임베딩 → pgvector 저장
- 유사 메일 검색 기반 RAG 구성
- 대화 맥락을 반영한 답장 초안 생성 및 검토
- 2~3개 답장 옵션 제안 → 편집기에서 자유 수정 후 발송

### ✍️ AI 보조 메일 작성

- 프롬프트 입력 → AI가 메일 제목·본문 초안 생성
- 전송 전 AI 자동 리뷰: 오타, 첨부 누락, 맥락 적절성 팝업 알림

### ⚡ 실시간 메일 동기화 및 비동기 처리

Google Pub/Sub과 Gmail API를 통해 신규 메일 이벤트를 수신하고, RabbitMQ 기반 비동기 처리 구조로 메일 저장, 라벨링, 알림 작업을 안정적으로 분리했습니다.

- Google Pub/Sub 기반 Gmail 변경 이벤트 수신
- RabbitMQ 기반 비동기 메일 처리 (Direct Exchange + DLX)
- Backpressure 적용을 통한 트래픽 급증 대응
- DLQ 및 Dead Letter Alert 기반 실패 메시지 추적
- FCM(Firebase Cloud Messaging) 기반 실시간 Push 알림

### 💳 구독 및 결제

- Portone 연동 결제 시스템
- 플랜별 AI 기능 사용 제한 및 Rate Limit 관리

---

## 📖 매뉴얼 / 튜토리얼

### 1. 시작하기 — Gmail 계정 연동

```
1. mail.ajou.app 에서 서비스 회원가입 / 로그인
2. 사이드바 → [계정 추가] 클릭
3. Gmail OAuth 팝업에서 연동할 Google 계정 선택 및 권한 허용
4. 통합 인박스에서 해당 계정의 메일 자동 수신 확인
```

> Gmail OAuth는 서비스 로그인과 별개입니다. 로그인된 서비스 계정에 여러 Gmail 주소를 연결할 수 있습니다.

### 2. 라벨 자동 분류 설정

```
1. 설정 → [라벨 관리]
2. [라벨 추가] → 라벨 이름 및 분류 규칙 입력
3. [AI 제안 받기] → AI가 현재 수신 메일 기반 라벨 규칙 추천
4. 규칙 확인 후 저장 → 이후 수신 메일에 자동 적용
5. 과거 메일 재분류: [전체 재분류] 버튼 클릭 (Rate Limit 적용)
```

### 3. AI 답장 초안 생성

```
1. 메일 Thread 열기
2. [AI 답장 초안 보기] 클릭
3. AI가 제안하는 2~3개 답장 옵션 중 선택
4. 편집기에서 자유롭게 수정
5. [전송] 클릭
```

### 4. 알림 설정

```
1. 설정 → [알림]
2. 라벨별 알림 ON/OFF 설정
3. FCM 기반 실시간 Push 알림 수신 (브라우저 권한 허용 필요)
```

---

## 🏗️ 설계 및 구현

### 소프트웨어 아키텍처

```
┌─────────────────────────────────────────────────────────────────┐
│                         클라이언트                               │
│    React 19 + TypeScript + TanStack Router/Query + shadcn/ui    │
│    PWA (Service Worker) · Amplitude · Firebase(FCM)             │
└────────────────────────┬────────────────────────────────────────┘
                         │ HTTPS
┌────────────────────────▼────────────────────────────────────────┐
│                      Core (HTTP API 서버)                        │
│   Spring Boot 4 · Java 21 · Spring Security · Spring MVC       │
│                                                                  │
│  Gmail OAuth 연동  ──→  Pub/Sub 수신  ──→  MQ 발행              │
│  Controller → Facade → Classifier → Publisher                   │
└──────────┬──────────────────────────────────────────────────────┘
           │ RabbitMQ (DirectExchange + DLX)
┌──────────▼──────────────────────────────────────────────────────┐
│                     Worker (비동기 처리)                          │
│   Spring Boot 4 · Java 21                                       │
│                                                                  │
│  Listener (Facade 역할) → Handler → ApiService/CommandService   │
│  Gmail 동기화 · 라벨 분류 · 벡터 임베딩 · FCM Push 발송          │
└──────────┬──────────────────────────────────────────────────────┘
           │
┌──────────▼──────────────────────────────────────────────────────┐
│                       데이터 레이어                               │
│   PostgreSQL (pgvector 확장)  ·  Redis  ·  RabbitMQ            │
└─────────────────────────────────────────────────────────────────┘
           │
┌──────────▼──────────────────────────────────────────────────────┐
│                     외부 서비스                                   │
│   Gmail API  ·  Google Pub/Sub  ·  LLM API  ·  Portone(결제)   │
└─────────────────────────────────────────────────────────────────┘
```

#### 메시지 처리 흐름 (비동기)

```
[Google Pub/Sub]
      │  Gmail 변경 이벤트 (Webhook)
      ▼
[Core — Facade]
  Classifier → 이벤트 타입 분류
  Publisher  → RabbitMQ 발행 (mail.message-added / mail.label-sync 등)
      │  즉시 응답 (DB Write 없음)
      ▼
[RabbitMQ — DirectExchange]
      │  큐: mailsangja.{taskName}
      ▼
[Worker — Listener (비즈니스 Facade 역할)]
  Handler → Gmail API 조회 → CommandService → PostgreSQL 저장
  Handler → LLM API → 라벨 추천 / 임베딩 생성
  Handler → FCM → Push 알림 발송
      │  실패 시 → DLQ → Dead Letter Alert
```

#### 레이어 의존성 (단방향)

```
Controller → Facade → CommandService / QueryService → Repository (Port)
                   ↘ ApiService (외부 API 호출)
```

---

### Repository 구조

| 레포지토리 | 역할 | 기술 |
|:---|:---|:---|
| [`mailsangja/docs4capstone`](https://github.com/mailsangja/docs4capstone) | User Story 이슈 관리, 기획 문서 | GitHub Projects |
| [`mailsangja/mailsangja-server`](https://github.com/mailsangja/mailsangja-server) | 백엔드 서버 (core + worker + db 멀티모듈) | Spring Boot 4 / Java 21 |
| [`mailsangja/mailsangja-frontend`](https://github.com/mailsangja/mailsangja-frontend) | 프론트엔드 웹 앱 | React 19 / TypeScript / Vite |

#### `mailsangja-server` 모듈 구조

```
mailsangja_server/
├── db/                          # JPA Entity, Repository Port/Adapter
│   └── src/main/java/com/mailsangja/db/
│       ├── entity/              # User, MailAccount, Thread, Message, Label, ...
│       └── port/                # Repository Port 인터페이스
├── core/                        # HTTP API 서버 (port: 8080)
│   └── src/main/java/com/mailsangja/core/
│       ├── controller/          # REST API 엔드포인트
│       ├── facade/              # 비즈니스 흐름 조율
│       ├── handler/             # Classifier + Handler (이벤트 분류·처리)
│       ├── service/             # CommandService / QueryService
│       ├── config/              # Security, RabbitMQ, Async 설정
│       └── common/              # 인증(AuthUser/AuthAdmin), DTO, 예외 처리
├── worker/                      # MQ Consumer (port: 8081)
│   └── src/main/java/com/mailsangja/worker/
│       ├── messaging/
│       │   ├── listener/        # RabbitMQ Listener (비즈니스 Facade)
│       │   └── publisher/       # MQ 발행 전용
│       ├── handler/             # 이벤트 핸들러 (전략 패턴)
│       ├── service/             # ApiService / CommandService / QueryService
│       └── scheduler/           # Cron 트리거 (Watch 갱신 등)
├── docker/                      # 관측성 스택 설정 (Loki, Tempo, Alloy, Grafana)
├── compose.yaml                 # 개발 환경 Docker Compose
└── compose.production.yaml      # 운영 환경 Docker Compose
```

#### `mailsangja-frontend` 구조

```
mailsangja-frontend/
└── src/
    ├── routes/
    │   ├── _authenticated/      # 로그인 필요 라우트
    │   │   ├── mail/            # 인박스, Thread 뷰
    │   │   └── settings/        # 계정·라벨·알림 설정
    │   └── _guest/              # 로그인 전 페이지
    ├── components/
    │   ├── compose/             # 메일 작성기 (Tiptap 에디터)
    │   ├── thread/              # Thread 뷰 컴포넌트
    │   ├── label/               # 라벨 관리
    │   ├── sidebar/             # 사이드바 내비게이션
    │   └── ui/                  # shadcn/ui 기반 공통 컴포넌트
    ├── queries/                 # TanStack Query — 서버 상태 관리
    ├── mutations/               # TanStack Query — 서버 상태 변경
    ├── api/                     # API 클라이언트
    └── paraglide/               # i18n (ko / en)
```

---

### 핵심 기술 스택

<div align="center">

**Backend**

![Spring](https://img.shields.io/badge/Spring_Boot_4-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Java](https://img.shields.io/badge/Java_21-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL_+_pgvector-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React_19-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Shadcn/ui](https://img.shields.io/badge/shadcn/ui-000000?style=for-the-badge&logo=shadcnui&logoColor=white)
![TanStack Query](https://img.shields.io/badge/TanStack_Query-FF4154?style=for-the-badge&logo=reactquery&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)

**Infra / DevOps**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)
![Loki](https://img.shields.io/badge/Grafana_Loki-F46800?style=for-the-badge&logo=grafana&logoColor=white)
![Tempo](https://img.shields.io/badge/Grafana_Tempo-F46800?style=for-the-badge&logo=grafana&logoColor=white)

**AI / External API**

![Gmail API](https://img.shields.io/badge/Gmail%20API-EA4335?style=for-the-badge&logo=gmail&logoColor=white)
![Google PubSub](https://img.shields.io/badge/Google%20Pub%2FSub-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![FCM](https://img.shields.io/badge/FCM-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![Portone](https://img.shields.io/badge/Portone-00B3E3?style=for-the-badge&logo=iota&logoColor=white)
![RAG](https://img.shields.io/badge/RAG%20AI%20Draft-8A2BE2?style=for-the-badge&logo=openai&logoColor=white)

</div>

#### 기술 선택 근거

| 기술 | 선택 이유 |
|:---|:---|
| **RabbitMQ (DirectExchange + DLX)** | Gmail 이벤트 처리를 Core에서 분리하여 비동기화. DLQ로 실패 메시지 추적. Backpressure 적용으로 트래픽 급증 대응 |
| **pgvector** | PostgreSQL 확장으로 별도 Vector DB 없이 임베딩 저장·유사 검색 구현 (RAG 파이프라인) |
| **Redis** | 라벨 Debounce/Rate Limit 상태 관리, AI API Rate Limit 캐시, Gmail Thread 분산 락 |
| **Google Pub/Sub** | Gmail 변경 이벤트를 Webhook 방식으로 수신 (폴링 대비 지연 최소화) |
| **TanStack Router/Query** | 타입 안전한 라우팅과 서버 상태 관리. 캐시·재검증·낙관적 업데이트 지원 |
| **Tiptap** | 리치 텍스트 에디터 (Markdown / HTML 메일 작성) |
| **Paraglide JS** | 트리쉐이킹 지원 i18n (한국어/영어). 번들 크기 최소화 |
| **PWA + FCM** | 브라우저 Push 알림 + 오프라인 캐시 지원 |

#### RAG 알고리듬 개요

```
[임베딩 생성]
  사용자 전송 메일 → 텍스트 정제 → LLM Embedding API
  → pgvector (PostgreSQL) 저장

[답장 초안 생성 — RAG Pipeline]
  수신 메일 → 임베딩 변환
  → pgvector ANN 검색 (코사인 유사도) → 유사 과거 메일 K개 검색
  → 검색 결과 + 현재 메일 → LLM 프롬프트 구성
  → LLM API → 답장 초안 2~3개 생성
```

---

### DevSecOps / 배포

#### CI/CD 파이프라인

```
PR 생성 (→ main)
  └─▶ [CI: Validate]
        ├─ PostgreSQL 18 + Redis 8 서비스 컨테이너 기동
        ├─ JUnit5 테스트 실행 (core + worker)
        └─ JaCoCo 커버리지 → Codecov 업로드

main 브랜치 병합
  └─▶ [Build Docker Image]
        ├─ Gradle bootJar 빌드 (core / worker)
        ├─ Docker Buildx (linux/amd64 + linux/arm64 멀티플랫폼)
        └─ GHCR(GitHub Container Registry) Push

이미지 빌드 완료
  └─▶ [Deploy]
        ├─ SSH → 운영 서버 접속
        ├─ compose.production.yaml Pull & Up (postgres / core / worker)
        └─ 수동 배포: workflow_dispatch로 이미지 태그 지정 가능 (롤백 지원)
```

#### 관측성 스택 (Observability)

| 구성 요소 | 역할 |
|:---|:---|
| **Grafana Alloy** | 로그 수집 에이전트 (파일 → Loki), OTLP 트레이스 수신 (→ Tempo) |
| **Grafana Loki** | 로그 집계 및 조회 |
| **Grafana Tempo** | 분산 트레이싱 (OpenTelemetry) |
| **Grafana** | 통합 모니터링 대시보드 |
| **RabbitMQ DLQ + Discord Alert** | 실패 메시지 추적 및 이상 탐지 알림 |
| **Amplitude** | 사용자 행동 분석, Session Replay, 히트맵 |

#### 보안

- Spring Security 기반 인증·인가 (`@AuthUser` / `@AuthAdmin` 어노테이션)
- Gmail OAuth — 서비스 로그인과 분리된 별도 인박스 연동 흐름
- 환경 변수로 민감 정보 관리 (하드코딩 금지, `@ConfigurationProperties` 사용)
- GitHub Secrets — API Key, SSH Key, Codecov Token 관리

#### 로컬 개발 환경 실행

```bash
# 전체 인프라 기동 (PostgreSQL, Redis, RabbitMQ, 관측성 스택)
docker compose up -d

# 각 모듈 빌드 및 실행
./gradlew :core:bootRun
./gradlew :worker:bootRun

# 테스트 실행
./gradlew :core:test :worker:test --no-daemon
```

```bash
# 프론트엔드 개발 서버
npm install
npm run dev
```

---

## 📊 운영 성과

<div align="center">

| 구분 | 성과 |
|:---:|:---|
| 🧑‍💻 사용자 지표 | 실제 서비스 운영을 통해 MAU 200명 이상 확보 |
| 🧪 테스트 품질 | JUnit5 기반 Service Layer 테스트를 작성하여 테스트 커버리지 52% 달성 |
| 🔒 테스트 케이스 | 핵심 비즈니스 로직에 대해 80개 이상 Unit / 통합 테스트 작성 |
| 📈 UX 분석 | Amplitude Session Replay와 히트맵 분석을 활용해 계정 연동 및 라벨 관리 플로우 개선 |
| 🚨 장애 대응 | RabbitMQ DLQ와 Dead Letter Alert를 통해 실패 메시지 추적 및 이상 상황 탐지 |
| ⚙️ 처리 안정성 | Pub/Sub 수신 이후 메일 저장·분류·알림 작업을 비동기화하여 Backpressure 기반 처리 구조 |

</div>

---

## 🌱 팀 소개

<div align="center">

| 이름 | 학과 | 이메일 | 역할 |
|:---:|:---:|:---:|:---:|
| 김휘래 ([@rlagnlfo1004](https://github.com/rlagnlfo1004)) | 소프트웨어학과 | hrkim2001@ajou.ac.kr | **팀장** / 백엔드 개발 |
| 천진강 ([@jjjjjk12](https://github.com/jjjjjk12)) | 소프트웨어학과 | jjjjjk12@ajou.ac.kr | 인프라 / 백엔드 개발 |
| 곽민서 ([@mkms8436](https://github.com/mkms8436)) | 소프트웨어학과 | mkms0222@ajou.ac.kr | 디자인 / 프론트엔드 개발 |
| 한동현 ([@asitisdev](https://github.com/asitisdev)) | 소프트웨어학과 | hando1220@ajou.ac.kr | 인프라 / 프론트엔드 개발 |

</div>

---

## ✅ GitHub Projects 기반 애자일 협업

[![Projects](https://img.shields.io/badge/GitHub%20Projects-mailsangja%2F1-238636?style=flat-square&logo=github&logoColor=white)](https://github.com/orgs/mailsangja/projects/1)

Sprint 단위로 작업 목표를 설정하고, **STORY → TASK** 두 단계로 이슈를 분리하여 관리했습니다.

- **STORY** (`docs4capstone`): 사용자 관점의 기능 요구사항 정의
- **TASK** (`mailsangja-server`): STORY를 기반으로 한 실제 구현 단위 작업

각 TASK는 GitHub Projects Board에서 `Backlog → Ready → In Progress → Review → Done` 단계로 진행 상태를 추적하며, PR에서 `Closes #이슈번호`로 자동 종료됩니다.

<details>
<summary><b>📖 1. STORY Issue — 사용자 관점의 기능 요구사항</b></summary>
<br>

> 레포: [`mailsangja/docs4capstone`](https://github.com/mailsangja/docs4capstone)

**컨벤션**

| 구분 | 규칙 |
|:---:|:---|
| Title 형식 | `[STORY-XXX] 제목` |
| 타입 | `Story` |
| 작성 방식 | As a / I want to / so that 형식으로 사용자 요구사항 기술 |

**예시**

```
Title: [STORY-427] 메일 라벨 자동 분류

👤 As a (사용자 유형): 서비스 사용자
🎯 I want to (원하는 기능): 메일을 자동으로 라벨링 하고 싶다
💡 so that (기대 효과): 중요한 메일을 빠르게 찾을 수 있도록
```

</details>

<details>
<summary><b>📋 2. TASK Issue — 실제 구현 단위 작업</b></summary>
<br>

> 레포: [`mailsangja/mailsangja-server`](https://github.com/mailsangja/mailsangja-server) &nbsp;/&nbsp; [`mailsangja/mailsangja-frontend`](https://github.com/mailsangja/mailsangja-frontend)

**컨벤션**

| 구분 | 규칙 |
|:---:|:---|
| Title 형식 | `[TASK-XXX] 제목` |
| 타입 | `Task-BE` / `Task-FE` / `Task-OPS` |
| STORY 연결 | 상위 STORY Issue 번호를 기준으로 앞 세 자리 공유 |

**예시 — BE Task**

```
Title: [TASK-427] 민감 라벨 추가 및 처리 로직

## 🛠️ 목적
무엇을 위한 작업인지 설명

## 📝 작업 내용
- 해야 할 일 1
- 해야 할 일 2

## ✅ 완료 조건
- [x] 어떤 상태가 되면 Done인가?
- [x] 확인 기준은 무엇인가?

## 📚 참고 자료 (선택)
- 관련 API / 참고자료 문서 링크
```

**예시 — FE Task**

```
Title: [TASK-919] 중요 메일 기능 및 인박스 구현

## 🛠️ 목적
무엇을 위한 작업인지 설명

## 📝 작업 내용
- 해야 할 일 1
- 해야 할 일 2

## ✅ 완료 조건
- [x] 어떤 상태가 되면 Done인가?
- [x] 확인 기준은 무엇인가?

## 📚 참고 자료 (선택)
- 관련 문서 링크
```

</details>

<details>
<summary><b>🌿 3. Branch 규칙</b></summary>
<br>

**컨벤션**

| 구분 | 규칙 |
|:---:|:---|
| 브랜치 구조 | `{이슈번호}-{작업내용}` |
| 이슈번호 | TASK Issue 번호 기준 |
| 작업내용 | 영문 소문자, `-` 구분 |

**예시**

```
803-admin-user
201-thread-count
901-start-thread-api
616-refactor-ai
```

</details>

<details>
<summary><b>💬 4. Commit 규칙</b></summary>
<br>

**컨벤션**

| 구분 | 규칙 |
|:---:|:---|
| 형식 | `{type}: {내용} (#{TASK 이슈번호})` |
| Type | `feat`, `fix`, `refactor`, `docs`, `test`, `chore` |
| 내용 | 한글 작성, 변경 목적 중심으로 기술 |
| 이슈번호 | 관련 TASK Issue 번호 괄호로 명시 |

**예시**

```
feat: 별표 편지함 안읽은 수 반영 (#146)
fix: Inline/Attachment 구분 로직 강화 (#43)
refactor: 응답 DTO 및 Entity star 필드 추가 (#146)
test: star 토글 조회 구현 및 테스트 (#146)
```

</details>

<details>
<summary><b>🔀 5. Pull Request 규칙</b></summary>
<br>

**컨벤션**

| 구분 | 규칙 |
|:---:|:---|
| Title | `[STORY-XXX] 작업 내용` |
| User Story | `docs4capstone` STORY Issue 번호 연결 |
| Task | `Closes #이슈번호` 로 TASK Issue 자동 종료 |
| Test 결과 | API 기능별 HTTP Method · 경로 · 결과 이미지 첨부 |

**PR 템플릿**

```
## 🔗 관련 작업

### 👤 User Story
- mailsangja/docs4capstone#n

### 📌 Task
- Closes #
- Closes #


## 💡 작업 내용

-
-


## 📝 추가 설명

### 1.
-

### 2.
-


## ⚡️ Test 결과

| 기능 1     | 기능 2     |
| ---------- | ---------- |
| HTTP Method | HTTP Method |
| /api/v1/example | /api/v1/example |
| 이미지 태그 | 이미지 태그 |
```

</details>

---

<div align="center">

**아주대학교 소프트웨어학과 &nbsp;·&nbsp; 2026-1 SW캡스톤디자인 2조**

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/mailsangja)
&nbsp;
[![Service](https://img.shields.io/badge/Service-mail.ajou.app-4A90E2?style=for-the-badge&logo=googlechrome&logoColor=white)](https://mail.ajou.app/)
&nbsp;
[![SOFTCON](https://img.shields.io/badge/SOFTCON-2026--1-0057A8?style=for-the-badge&logo=academia&logoColor=white)](https://softcon.ajou.ac.kr/works/works.asp?uid=2298)

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=120&section=footer" />

</div>
