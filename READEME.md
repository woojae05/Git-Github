# Git&GitHub 익히기

## git
깃은 컴퓨터 파일의 변경사항을 추적하고 여러 명의 사용자들 간에 해당 파일들의 작업을 조율하기 위한 분산 버전 관리 시스템이다

git init - .git 파일을 생성한다.

## 첫 번째 버전
- 커밋(Commit) - 하나의 버전 (git commit -m "설명")
- 애드(Add) - 커밋을 으로 만들고 싶은 파일을 선택 (git add .)

## 만든 버전 GitHub에 올리기
- git remote add origin https://github.com/아이디/이름.git
내 컴퓨터에 있는 폴더에 GitHub 저장소 주소 알려주기
- git push origin master
로컬 저장소에서 원격 저장소로 커밋 푸쉬

## 다른 사람이 만든 저장소 불러오기
- 클론(Clone) - 원격 저장소의 코드를 내 컴퓨터로 받아 온다. (git clone https://github.com/아이디/이름.git)
- 풀(Pull) - 원격 저장소 데이터을 가져온다. (git pull origin master)


## GitHub에 버전 올리는 순서 
1. 커밋(Commit)하고 싶은 파일 선택해서 애드(Add)하기
2. 커밋(Commit)하기
3. GitHub에 커밋(Commit) 푸쉬(Push)하기

## 평행세계 나누기
- 브랜치(Branch - 가지) - 표지판 개념
- git push orgin master - master 브랜치(기본적으로 만들어져 있음)에 커밋을 푸쉬해라 라는 뜻
- git branch test - test라는 브랜치를 현재 시점에 만들어라
- git checkout test - test 브랜치로 이동해라

## 두 버전 합치기
- 머지(Merge) - 브랜치를 병합
- git merge branch_name - 헤드와 branch_name을 병합

## 병합하다 충돌
- 컴플릭트(Conflict) -머지 할 때 두 버전이 같은 곳을 수정
- 수동으로 해결해야 함

## 저장소 통쨰로 복제하기
- 포크(Fork) - 저장소를 통째로 복사

## 내 코드를 머지(Merge)해주면 안되겠니?
- 풀 리퀘스트 - 커밋(Commit)과 커밋(Commit)을 합치는걸 허락 하도록 요청

## 많이 사용되는 Git 키워드
1. rebase: 묵은 커밋을 새 커밋처럼 조작하고 싶어요
2. amend: 깜빡하고 수정 못 한 파일이 있어요, 방금 만든 커밋을 살짝 추가할래요
3. cherry-pick: 저 커밋 하나만 떼서 지금 브랜치에 붙이고 싶어요 
4. reset: 옛날 커밋으로 시간을 돌리고 싶어요
5. reverse: 이 커밋의 변경사항을 되돌리고 싶어요
6. stach: 변경사항을 잠시 킵해두고 싶어요. 아직 커밋은 안 만들래요
