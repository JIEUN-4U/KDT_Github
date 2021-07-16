# 들어가기. git 백업

- 지역 저장소 내용을 복제(clone)하여 또 다른 저장소에 넣는(push) 작업
- 원격저장소 내용을 당겨오면(pull), 내 컴퓨터와 원격저장소가 동기화됨
- `push` 와 `pull` 의 연속
- `pull` -> 작업 -> `commit` -> `push`


## git 백업의 효과

- 안전성
- 작업 이동성 극대화



## git hosting

- 깃허브(github)

- 깃랩(gitlab)

- etc

  

# 1. 원격저장소 연결

> github -> new repository 생성-> code확인(HTTPS) -> git bash 통해 연결하기
>


## 1)명령어

## `git remote`

원격 저장소 정보 출력

- git remote -v



추가하기

- git remote add
  - git remote add [저장소별명] [저장소주소]

- git remote add origin https://github.com/JIEUN-4U/first.git



## `git push`

원격저장소에 코드 백업

- `git push [저장소 별명] [브랜치이름]`
  - `git push origin master`



## 1-2)복제 clone

>  이미 있는 것을 복제함

### `git clone [주소]`



## 1-3)당겨오기 Pull

> 원격 저장소 내용을 지역 저장소로 당겨오는 것

### `git pull`



# 마치며

>  백업 과정을 통해 오픈소스를 자유롭게 이동, 동기화 가능
>
> > +)이슈트래커 이용: 발생 문제 기록 및 처리상태 체계적 관리 가능
> >
> > > 추후 협업 이용 시 이 이슈트래커를 통해 업무분담 처리 가능



# 다음차시 예고

> git 협업

- 충돌(conflict) 발생 시 `협업`을 통해 해결할 수 있는 방법 학습

