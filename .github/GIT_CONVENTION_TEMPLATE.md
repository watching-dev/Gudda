#### `git convention`

#### 규칙 설명

* 일반적인 경우: **이슈먼저 등록 -> 작업 -> push**
* **리팩토링 처럼 특별한 경우: 이슈먼저 등록 -> 브랜치 생성 -> 작업 -> Pull Request -> Merge**
*
* **배포의 경우: Top 브랜치에서 release 0.0.1 브랜치 생성 -> 확인 작업 -> Pull Request -> Merge -> tag 설정( 배포 브랜치는 삭제x )**

***

#### `git branch convention`

#### 규칙 설명

* Git-Flow 와 GitHub-Flow 를 조금씩 섞어(?) 사용
* Main 브랜치는 배포만 담당
* Main 브랜치에서 나온 Top 브랜치는 Develop / Topic 과 같은 역할(준 배포 브랜치)
* Top 브랜치에서 Feature / HotFix 브랜치를 만들어 Pull Request를 이용하여 Merge
* 
* 브랜치를 만들때는 commit convention을 prefix로 작성하고 이슈넘버, 이름 작성
* 아래 prefix 예시는 commit convention에 따라 추가 될 수 있음
* (23.09.12)
* #### `예) [feat/#12] 로그인 기능 추가 | [refactor/#12] 로그인 리팩토링 | [fix/#12] 로그인 에러 수정`
* #### `예) [test/#12] ui test 추가 | [style/#12] swift convention 추가`
*
* #### `예) [init/#12] 프로젝트 생성 | [chore/#12] 폴더 구조 수정 | [docs/#12] README.md 수정`
* #### `예) [add/#12] 이슈 템플릿 추가 | [del/#12] 이슈 템플릿 삭제`
* #### `예) [rename/#12] ViewController 이름 수정 | [design/#12] 첨부 이미지 디자인 어떤지 아이디어 요청(PR)`
* #### `예) [build/#12] 빌드 버전 수정 | [ci/#12] ci 관련 수정 | [release 0.0.1] 배포`