## Git&GitHub 익히기

# git
깃은 컴퓨터 파일의 변경사항을 추적하고 여러 명의 사용자들 간에 해당 파일들의 작업을 조율하기 위한 분산 버전 관리 시스템이다

git init - .git 파일을 생성한다.

# 첫 번째 버전
커밋(Commit) - 하나의 버전 (git commit -m "설명")
애드(Add) - 커밋을 으로 만들고 싶은 파일을 선택 (git add .)

# 만든 버전 GitHub에 올리기
- git remote add origin https://github.com/아이디/이름.git
내 컴퓨터에 있는 폴더에 GitHub 저장소 주소 알려주기
- git push origin master
로컬 저장소에서 원격 저장소로 커밋 푸쉬

# 다른 사람이 만든 저장소 불러오기
클론(clone) - 원격 저장소의 코드를 내 컴퓨터로 받아 온다. (git clone https://github.com/아이디/이름.git)
풀(pull) - 원격 저장소 데이터을 가져온다. (git pull origin master)


