# 2차 git 교육

이 레포지토리는 성균관대학교 프로그래밍 학회 SKKU Overflow에서 주최하는 2차 git 교육용 레포지토리입니다.

## 브랜치 이름

이번 교육에서 사용되는 브랜치들의 이름은 다음과 같습니다.

- `master`: 검증된 코드를 저장하는 브랜치
- `dev`: 개발중인 코드를 저장하는 브랜치
- `hotfix`: 심각한 오류를 수정하기 위한 브랜치

# 1. fork

# git clone

- git clone git@github.com:`${github 사용자명}`/git-study-2.git

- cd git-study-2

# 기본 작업 (브랜치: master)

- main.py 수정
- git add main.py
- git commit
- git push

# hotfix 브랜치 작업

- git checkout -b hotfix
- main.py 수정
- git add main.py
- git commit
- git push

# merge

- git checkout master
- git merge hotfix
- 충돌 병합
- git branch -d hotfix

# 개발 브랜치

- git checkout dev
- git rebase master
- git push -u origin dev --force
