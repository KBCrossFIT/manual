# Git 브랜치
- 모든 작업은 자신의 이름으로 생성된 브랜치에서 한다.
	
    - `git checkout 이름` 이후 작업
- `main` 브랜치는 항상 배포가 가능한 상태의 브랜치
- `dev` 브랜치에 모든 협업들을 Pull Request 하고 Merge한다.
- `자신의 이름 브랜치`를 생성하여 작업한다.

# Git Commit Convention
##### 커밋 메시지 구조
`subject`, `body`, `footer`
```
type : subject
// 줄바꿈 두번
body(생략가능) : 본문

footer(생략가능) : 꼬리말
```
**subject** : 작업 타입과 작업 내용을 작성합니다.
**body** : 작업 내용에 관해 설명이 필요한 경우 무엇을 했는지 작성합니다.
**footer** : 꼬리말을 해당 커밋과 연관된 이슈 트래킹 번호를 입력합니다.

##### 커밋 메시지 예시
```
feat: 로그인 기능 추가

부연설명(생략가능)

Resolves: #이슈번호
```

|Type|설명|
|---|---|
|feat|새로운 기능 추가|
|fix|버그 수정|
|refactor|리팩토링|
|design|CSS등 사용자 UI 디자인 변경|
|comment|필요한 주석 추가 및 변경|
|style|코드 포맷팅, 세미콜론 누락, 코드 변경이 없는 경우|
|test|테스트(테스트 코드 추가, 수정, 삭제)|
|init|프로젝트 초기 생성|
|rename|파일 혹은 폴더명 수정하거나 옮기는 경우|
|remove|파일을 삭제하는 작업만 수행하는 경우|

##### Commit 예시
```
git add .
git commit -m"fix: 결제 페이지 오류 수정"
git push origin mincheol
```
