# git 사용법 익히기

## 사전지식

### 1. 로컬 저장소(local)와 원격 저장소(remote)
- 로컬 저장소(local repository): 개발자의 컴퓨터에 위치한 프로젝트의 버전을 관리하는 저장소 (내 컴퓨터)
- 원격 저장소(remote repository): 네트워크 상의 다른 위치에 있는 저장소로 여러 개발자가 협업하며 프로젝트의 변경 이력을 공유하는 곳 (서버)
- local에서 작업한 것을 remote로 공유하기 위해 `git push` 명령어를 사용해야 변경사항이 서버에 반영된다. remote에서의 변경사항은 `git pull` 명령어를 사용하여 local로 가져올 수 있다. 이를 통해 여러 개발자가 효과적으로 협업할 수 있다.

<br>

### 2. branch란?
- 여러 개발자들이 동시에 다양한 작업을 할 수 있게 만들어주는 기능
- 독립적으로 어떤 작업을 진행하기 위한 개념
- 하나의 프로젝트에 두 명의 개발자가 동시에 작업하는 경우,
    - 개발자 A가 작업을 완료한 뒤, B가 이어서 작업하는 것은 많은 시간이 소요
    - 브랜치는 여러 작업을 각각 독립된 공간에서 진행할 수 있도록 하는 기능 (하나의 프로젝트에서 여러 사람이 동시에 본인의 작업을 진행할 수 있다.)

<br>

### 3. 기본 명령어
1. `git add`
    - 변경된 파일들을 스테이징 영역에 추가
    - git add [파일명/폴더명]

2. `git commit`
    - 스테이징 영역에 추가된 변경 사항을 로컬 저장소에 커밋
    - git commit -m "커밋 메시지"

3. `git push`
    - 로컬 저장소의 변경 사항을 원격 저장소에 업로드
    - git push origin main

4. `git pull`
    - 원격 저장소의 변경 사항을 로컬 저장소로 가져옴
    - git pull [원격저장소 이름] [브랜치 이름]

5. `git branch`
    - 브랜치를 생성하거나 현재 브랜치를 확인
    - 브랜치 생성: git branch [새로운 브랜치 이름]
    - 현재 브랜치 확인: git branch