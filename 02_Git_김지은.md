# Git이란?

(**버전**을 통해) 코드 관리 도구



# SCM & VCS

- SCM : Source Code Management (소스 코드 관리)
- VCS : Version Control System (버전 관리 시스템)
- DVDS : 분산형 



# Git 을 왜 사용하는가?

> 1. 버전관리 (히스토리 파악 및 이전버전으로 회귀 가능)
> 2. 백업 (지역저장소push< -->pull 원격저장소, 여러대의 컴퓨터 동기화 가능)
> 3. 협업 (같은 파일을 수정하여도 섞이는 것을 방지 가능)



# Git 종류

- Github
- Git (Original)
- Tortoise Git (only Windows)
- ScourceTree (강력한 자유로움 but 복잡성)



## Git 버전 관리

> 중요 : Git은 **폴더 단위**로 코드를 관리 -> 폴더 위치 중요! 항상 먼저 폴더 위치 지정

- 커밋 == 버전 생성  == 스냅샷 촬영 == 현재 상태 저장

## pwd

현재 위치 확인

## cd ~ or cd [폴더명]

홈으로 가기, 혹은 해당 폴더로 들어가기

## rm -r .git

git 폴더 지우기

## cd ..

상위 폴더로 돌아가기

## cat

출력

## mkdir

폴더 만들기



## ls -a

숨김 폴더 보기



## esc 3번 , :q!

VI 탈출법



### `git init`

특정 폴더를 git으로 관리 시작

- `(master)` 가 생성, 프롬포트에 표시됨
- `.git` 폴더 생성
  - `.git` 폴더 삭제 시 git 관리 중지

```
Initialized empty Git repository in C:/Users/govlh/recap/.git/
```



### `Git status`

git에게 상태 확인 -> **가장 많이 활용**

- `git init` 직후

```
On branch master : master 라는 브랜치에 있고

No commits yet : 아직 commit 없어

nothing to commit (create/copy files and use "git add" to track)
: commit 할게 없어 (트래킹 하고 싶으면 'git add'명령어 사용해)
```

- `a.txt`파일 생성 직후

````
Untracked files: 
  (use "git add <file>..." to include in what will be committed)
        a.txt (빨강)

nothing added to commit but untracked files present (use "git add" to track)
````

- `git add a.txt` 직후

```
Changes to be committed: comit될 변경사항이 있어
  (use "git rm --cached <file>..." to unstage)
        new file:   a.txt (초록)
```



### `git add [파일명]`

**Staging Area(스냅샷 무대)에 파일 추가**



### `git commit -m "커밋 메시지"`

버전을 생성

- 커밋(버전) 구성 요소
  - 해시(hash)
  - 작성자
  - 날짜
  - 커밋메시지 : 버전에 대한 설명

```
$ git commit -m "First commit"

[master (root-commit) cbafabd] First commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 a.txt
```



### `git log`

버전(커밋)들의 히스토리(로그)

- `git log --oneline` : 한눈에 로그 보기

### git diff [파일명]

변경사항 확인

### `git config`

설정

- `git config [설정할내용] [설정할값]`
  - `git config user.name 'Jieun Kim'`
  - `git config user.email 'govlhao13@gmail.com'`
  - `git config --global` : 전역 설정

```
Author identity unknown

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

```



# Git 관련 학습 사이트

- [연습해보기](https://learngitbranching.js.org/?locale=ko)
- [코드아카데미 GIT 강의](https://opentutorials.org/course/3837)
- [강동주 강사_실습파일](http://bit.do/kdt-dse-0715)







