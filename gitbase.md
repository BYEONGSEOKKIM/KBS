# Git 총정리



## Git 

> 버전을 통한 코드관리 도구

## SCM & VCS

- SCM: Source Code Management (소스 코드 관리)
- VCS: Version Control System (버전 관리 시스템)

## Git 도구

- 기초명령어

- 버전 관리 도구
  - 변경 이력 트래킹
  - 언제든 특정 시점으로 이동 가능
- 백업 도구
- 협업 도구

### 1. Git 기초명령어



#### (1) `pwd` 

- `pwd` (print working directory): 현재 폴더의 경로
- `~` (home directory): 홈디렉토리 (git bash 처음 열면 나오는 기본폴더)



#### (2) `ls`  

- `ls` (list): 내용물을 출력

Git (버전을 통해) 코드 관리 도구 SCM & VCS SCM: Source Code Management (소스 코드 관리) VCS: Version Control System (버전 관리 시스템) Git? 버전 관리 도구 변경 이력 트래킹 언제든 특정 시점으로 이동 가능 백업 도구 협업 도구

#### (2) `cd [폴더명]`  

- `cd` (change directory): 폴더를 변경
- `cd..` : 상위 폴더로 이동
- `cd.` : 현재 폴더로 이동



#### (2) `mkdir [폴더명]` 

- `mkdir` (make directory): 폴더를 생성



#### (2) `rm [파일명]`  

- `rm` (remove): 파일을 삭제



#### (2) `rm -r [폴더명]`  

- `-r` : recursively(재귀적으로) 폴더를 삭제



#### (2) `touch [파일명]`  

- `touch `: 파일생성



#### (2) `cp [파일명] [위치]`  

- `cp`(copy): 파일 복사



#### (2) `cp -r [폴더명] [위치]`  

- 폴더를 복사

#### (2) `mv [파일/폴더명] [바꿀파일/폴더명]`  

- `mv`(move): 파일 /폴더명 변경
- `mv [파일/폴더명] [위치]` : 파일 또는 폴더를 이동



### 2. Git 버전관리

 #### (1) `git init` 

>  특정 폴더를 git으로 관리 시작

- `(master)` 프롬프트에 표시
- `.git` 폴더 생성
  - `.git` 폴더 삭제 시 git 관리 중지



#### (2) `git status` 

>  git 에게 상태 확인



#### (3) `git add` [파일명]

> Staging Area에 파일 추가



#### (4) `git commit -m "커밋 메시지"` 

>  버전을 생성

- 커밋(버전)구성 요소
  - 해시(Hash)
  - 작성자
  - 날짜
  - 커밋메시지: 버전에 대한 설명



#### (5) `git log` 

>  버전(커밋)들의 히스토리(로그)



#### (6) `git config` 

> 설정

- `git config [설정할내용] [설정값]` 
  - `git config user.name 'KBS'`
  - `git config user.email 'kqw38598@gmail.com'` 
  - `git config --global` : 전역 설정

`

### 3. Git 백업

- Git 백업: 지역저장소(ex: 개인컴퓨터) 와 원격저장소(ex: github)간의 상호 통신

- github New repository 생성하여 주소복사하기



#### (1)`git remote` 

> 원격 저장소 연결

- `git remote add` : 저장소 별명과 github에서 생성한 저장소 주소 입력
  - ex) `git remote add origin http://~`



#### (2)`git push `

>  원격 저장소에 백업 

- ```
  git push [저장소 별명] [브랜치 이름]
  ```

  - ex `git push origin master`



### 4. Git 협업



#### (1) Git clone

>  협업시 같은 저장소 공유

- `git clone` 원격저장소 URL



#### (2) Git pull

>  원격저장소에서 로컬저장소로 내보내기

- `git pull origin master` 

