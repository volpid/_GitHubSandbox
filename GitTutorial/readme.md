
# 기본 사용법 정리

* 설정 관련

> git config --global user.name \<name\>
> <br/>
> git config --global user.email \<email\>
> <br/>
> git config --list
> <br/>
> git config --global color.status \<auto\>
> <br/>
> git config --global color.branch \<auto\>
> <br/>
> git config --global i18n.commitEncoding \<cp949/utf8\>
> <br/>
> git config --global i18n.logOutputEncoding \<cp949/utf8\>

* 이그노어 파일

> .gitignore
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> Library/**/
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> Debug/
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> *.opendb
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> *.sdf


* 리포지토리 관련

> git init
> <br/>
> git clone \<url\>
> <br/>
> git remote
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> add \<name\> \<url\>
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> remove \<name\>
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> rename \<oldname\> \<newname\>
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> get-url \<name\>
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> set-url \<name\> \<url\>

* 기본 사용
> git status
> <br/>
> git add
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> \<file\>
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> .
> <br/>
> git rm \<file\>
> <br/>
> git commit
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
-o \<file\> \<file\> \<file\>
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
-m "\<msg\>"
> <br/>
> git commit --amend -m "\<msg\>"
> <br/>
> git reset \<HEAD\> \<file\>
> <br/>
> git revert \<HEAD\>
> <br/>
> git checkout
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> -b \<branch\>
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> \<branch\> 브랜치 이동
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> \<file\> or \<folder\>  : 리버트
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> -f
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> \<hash/tag\> : 이번 버전 가져오기
> <br/>
> git push 
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> \<remote\> \<branch\>
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> --set-upstream \<remote\> \<branch\>
> <br/>
> git pull \<remote\>
> <br/>
> git fetch \<remote\>
> <br/>
> git tag \<name\>
> <br/>
> git log
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> -p
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> -\<number\>
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> --stat
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> --pretty=online
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> --pretty=short
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> --graph
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> --name-status
> <br/>
> git diff 
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> \<commit hash\> \<commit hash\>
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> HEAD \<file\>
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> --cached \<file\>
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> --stat
> <br/>
> git blame \<file\>
> <br/>
> git branch
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> -a 
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> -d \<branch\>
> <br/>
> git stash
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> push / pop
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> list
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> show \<stash: stash@{0}\>
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> drop \<stash: stash@{0}\>
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> apply \<stash: stash@{0}\>
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> clear
> <br/>
> &nbsp;&nbsp;&nbsp;&nbsp;
> craete <msg>

