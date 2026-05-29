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

## 🔥 서비스 소개

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
</table>

---

## 🚀 핵심 기능

### 📥 다중 Gmail 계정 통합 인박스

여러 Gmail 계정을 하나의 화면에서 조회할 수 있는 통합 인박스를 제공합니다.  
사용자는 계정을 반복해서 전환하지 않아도 전체 메일 흐름을 한 번에 확인할 수 있습니다.

- Gmail OAuth 기반 계정 연동
- 계정별 메일 동기화 및 통합 조회
- 메일 계정 단위 필터링 및 검색 지원

### 🏷️ AI 기반 자동 라벨링

메일 제목, 본문, 발신자 정보를 기반으로 AI가 적절한 라벨을 자동 제안합니다.  
제안된 라벨은 필터링, 알림 설정, 민감정보 관리 정책과 연결하여 메일 관리 자동화의 기준으로 활용할 수 있습니다.

- 메일 내용 기반 라벨 추천
- 사용자 정의 라벨 관리
- 라벨 기반 필터링 및 알림 정책 연동

### ✉️ RAG 기반 맞춤 답장 초안 생성

사용자의 기존 메일 작성 패턴을 벡터화하고, 유사한 메일 맥락을 검색하여 개인화된 답장 초안을 생성합니다.

- 사용자 메일 패턴 기반 임베딩 생성
- 유사 메일 검색 기반 RAG 구성
- 대화 맥락을 반영한 답장 초안 생성 및 검토

### ⚡ 실시간 메일 동기화 및 비동기 처리

Google Pub/Sub과 Gmail API를 통해 신규 메일 이벤트를 수신하고, RabbitMQ 기반 비동기 처리 구조로 메일 저장, 라벨링, 알림 작업을 안정적으로 분리했습니다.

- Google Pub/Sub 기반 Gmail 변경 이벤트 수신
- RabbitMQ 기반 비동기 메일 처리
- Backpressure 적용을 통한 트래픽 급증 대응
- DLQ 및 Dead Letter Alert 기반 실패 메시지 추적

---

## 🛠️ 기술 스택

<div align="center">

**Backend**

![Spring](https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Shadcn/ui](https://img.shields.io/badge/shadcn/ui-000000?style=for-the-badge&logo=shadcnui&logoColor=white)
![TanStack Query](https://img.shields.io/badge/TanStack_Query-FF4154?style=for-the-badge&logo=reactquery&logoColor=white)

**Infra / DevOps**

![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![ArgoCD](https://img.shields.io/badge/ArgoCD-EF7B4D?style=for-the-badge&logo=argo&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
![Loki](https://img.shields.io/badge/Grafana%20Loki-F46800?style=for-the-badge&logo=grafana&logoColor=white)

**AI / External API**

![Gmail API](https://img.shields.io/badge/Gmail%20API-EA4335?style=for-the-badge&logo=gmail&logoColor=white)
![Google PubSub](https://img.shields.io/badge/Google%20Pub%2FSub-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![FCM](https://img.shields.io/badge/FCM-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![Portone](https://img.shields.io/badge/Portone-00B3E3?style=for-the-badge&logo=iota&logoColor=white)
![RAG](https://img.shields.io/badge/RAG%20AI%20Draft-8A2BE2?style=for-the-badge&logo=openai&logoColor=white)

</div>

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
| ⚙️ 처리 안정성 | Pub/Sub 수신 이후 메일 저장·분류·알림 작업을 비동기화하여 Backpressure 기반 처리 구조

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
