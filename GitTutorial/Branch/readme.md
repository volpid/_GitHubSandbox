
# git 브랜치 기본 명령

* 브랜치 로그 확인
> git log --branches --decorate --graph --oneline
> gitk

* 브랜치 비교
git log \<branch\>..\<branch\>
git log -p \<branch\>..\<branch\>
git diff \<branch\>..\<branch\>

* 브랜치 리스트
> git branch  
> git branch --list  
> git branch -r --remote  
> git branch -a, --all  

* 브랜치 생성
> git checkout -b \<branch\>

* 브랜치 삭제
> branch -d \<branch\>  
> branch -D \<branch\>

* 리모트 브랜치 삭제
> git push \<remote\> **:\<branch\>**

* 브랜치 전환
> git checkout \<branch\>

* 브랜치 머지
> git merge \<branch\>  