
# git 브랜치 기본 명령

* 브랜치 로그 확인

> git log --branches --decorate --graph --oneline  
> gitk

* 브랜치 비교

> git log \<branch\>..\<branch\>  
> git log \<branch\>...\<branch\>  
> git log -p \<branch\>..\<branch\>  
> git diff \<branch\>..\<branch\>  

* 브랜치 리스트

> git branch  
> git branch --list  
> git branch -r --remote  
> git branch -a, --all  
> git branch -v  
> git branch --merged  
> git branch --no-merged  

* 브랜치 생성

> git checkout -b \<branch\>

* 브랜치 삭제

> branch -d \<branch\>  
> branch -D \<branch\>  
> branch -r -d \<branch\>

* 리모트 브랜치 삭제

> git push \<remote\> **:\<branch\>**

* 브랜치 전환

	브랜치 변경할 때 워킹 디렉토리 정리 필요 (stash \/ commit --amend)  
	tracked 아닌 파일은 브랜치 변경시 남게된다.

> git checkout \<branch\>

* 브랜치 머지

> git merge \<branch\>  
> git checkout --ours \<file\>  
> git checkout --theirs \<fiel\>  

* 머지툴 셋팅 

.gitconfig \(글로벌 콘피그 파일\)

```
[merge]
	tool = kdiff3
	
[mergetool "kdiff3"]
	path = <path>
	
[diff]
	tool = kdiff3
	guitool = kdiff3
	
[difftool "kdiff3"]
	path = <path>
```

* HEADs

> HEAD : 워킹 트리 베이스 헤드  
> FETCH_HEAD : 원격 저장소(remote repository) 마지막 fetch HEAD  
> ORIG_HEAD : HEAD를 옴기는 작업(reset등) 의경우 기존 HEAD 위치 저장  
> MERGE_HEAD : 브렌치 머지를 위한 HEAD  