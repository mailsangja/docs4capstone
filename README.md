# 메일상자 팀 (2026-1학기 캡스톤디자인 2조)


## 🔥 서비스 소개

> 메일상자는 AI 기술을 활용하여 이메일과 관련된 문제를 해결하는 팀입니다.

## 🌱 팀 소개

| 이름 | 학과 | 이메일 | 역할 |
| --- | --- | --- | --- |
| 곽민서([@mkms8436](https://github.com/mkms8436)) | 소프트웨어학과 | mkms0222@ajou.ac.kr | FrontEnd Developer |
| 김휘래([@rlagnlfo1004](https://github.com/rlagnlfo1004)) | 소프트웨어학과 | hrkim2001@ajou.ac.kr | BackEnd Developer |
| 천진강([@jjjjjk12](https://github.com/jjjjjk12)) | 소프트웨어학과 | jjjjjk12@ajou.ac.kr | BackEnd Developer |
| 한동현([@asitisdev](https://github.com/asitisdev)) | 소프트웨어학과 | hando1220@ajou.ac.kr | FrontEnd / Infra Developer |

## ✅ 협업 방식

> 효율적인 협업을 위해 GitHub을 활용한 명확한 컨벤션을 수립하여 진행했습니다.

<details>
<summary><b>1. Issue 규칙</b></summary>

**컨벤션**

| 구분       | 규칙                                                |
| -------- | ------------------------------------------------- |
| Issue 유형 | `feature`, `bug`, `refactor` 등 라벨 지정           |
| Title 형식 | `[Feat] 한 일`, `[Bug] 어떤 문제`, `[Refactor] 리팩토링 내용` |
| Template | 각 유형(feature / bug / refactor)에 맞는 템플릿 형식 유지      |
| Task 작성  | 작업 상세 내용은 체크박스로 작성하여 추적 가능하게 유지                   |

<br></br>

**예시**
- Feature Issue 예시
    ```
    Title: [Feat] 영상 업로드 API 구현
    
    ## 💡 설명
    > 추가하려는 기능에 대해 간결하게 설명해주세요
    
    ## ✅ 작업 상세 내용
    - [ ] presigned URL 발급 API 구현
    - [ ] 업로드 검증 로직 추가
    - [ ] 파일 확장자 필터링 추가
    
    ## 📝 추가 설명
    없음
    
    ## 📚 참고 자료
    없음
    ```
- Bug Issue 예시
    ```
    Title: [Bug] 키스톤 토큰 관련 버그 발견
    
    ## 💡 설명
    > 어떤 버그인지 간단하게 설명해주세요
    
    ## 🚨 상황
    로그인 후 토큰이 정상적으로 발급되지 않음
    
    ## 💥 실제 결과
    서버에서 401 Unauthorized 반환
    
    ## 🖥️ 예상 결과
    정상적으로 토큰 발급 및 인증 가능해야 함
    
    ## 📚 참고 자료
    없음
    
    ```

</details>

<details>
<summary><b>2. Branch 규칙</b></summary>

**컨벤션**

| 구분       | 규칙                                                  |
| -------- | --------------------------------------------------- |
| 브랜치 구조   | `feat/#이슈번호/작업내용`                                   |
| Prefix   | `feat`, `fix`, `refactor`, `docs` 등 issue type과 일치 |
| Issue 연동 | 브랜치명에 GitLab issue number 반드시 포함                    |


<br></br>

**예시**

```
feat/#75/createProjectForm
fix/#102/loginFailure
refactor/#88/encodingServiceLogic

```

</details>

<details>
<summary><b>3. Commit 규칙</b></summary>

**컨벤션**

| 구분           | 규칙                                                            |
| ------------ | ------------------------------------------------------------- |
| 형식           | `{type}: {message}`                            |
| Type         | `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`, `design` |
| Message      | 한글로 작성, 파일명/디렉토리명 명시 금지                                       |
| 공백 규칙        | `:` 뒤에만 공백 존재                                                 |


<br></br>

**예시**

```
feat: 예약 기능 validation 추가
fix: 로그인 실패 처리 로직 수정
refactor: 인코딩 서비스 코드 구조 재정비
docs: README API 문서 업데이트

```

</details>

<details>
<summary><b>4. Merge Request 규칙</b></summary>

**컨벤션**

| 구분          | 규칙                   |
| ----------- | -------------------- |
| Title       | `[Feat] 작업 내용 #이슈번호` |
| MR Template | default 템플릿 형식 유지    |
| 관련 이슈       | `#이슈번호` 반드시 연결       |
| 설명          | 작업 요약 + 변경 사항 명확히 기재 |


<br></br>

**예시**

```
Title: [Feat] Vercel 배포 스크립트 및 Git Action 추가 #64

## 🔗 관련 이슈
> #64

## 💡 작업 내용
- Vercel 배포 스크립트 추가
- main 브랜치 push 시 자동 배포되는 GitHub Action 설정

## 📝 추가 설명
없음

## 📚 참고 자료
없음

```

</details>

