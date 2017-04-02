
# reset, checkout, revert

Command | Scope | common use cases
--------|-------|----------
git reset | commit-level | 개인 브랜치의 커밋을 버린다, 또는 커밋되지 않은 변경을 지운다
git reset | file-level | 스테이징에서 없앤다 = Unstage a file
git checkout | commit-level | 브랜치 변경, 또는 오래된 커밋 버전 파일 가져오기
git checkout | file-level | 워킹 디렉토리 파일 변경을 버린다
git revert | commit-level | 공용 브랜치의 커밋을 Undo
git revert | file-level | \(N/A\)

* git reset (commit-level)  
> --soft  
> --mixed : \(기본\) 워킹 디렉토리는 건들지 않음  
> --hard : 워킹 디렉토리까지  
> <br/>
> **log 에서 기존 커밋 내용을 지운다.**  

* checkout
> 워킹 디렉토리 변경  
> 히스토리\(log\) 를 건들지 않음

* revert
> Undo 내용으로 새 커밋 생성  
> file 레벨 연산 없음

***

* 현재 브랜치를 리모트 브랜치와 동일하게 만들기  
> git add . (or) git stash  
> git fetch \<remote\> \<branch\>  
> git reset --hard FETCH_HEAD

* 변경된 파일을 HEAD와 동일하게 (추가된 파일 제외)
> git checkout -f

* 오래된 커밋 버전 파일 가져오기
> git checkout \<HEAD\~num\> \<file\> 

* 추적 중이지 않은 파일 지우기 (추가된 파일 지우기)
> clean -n : 드라이 테스트  
> clean -f : 강제  
> clean -d : 디렉토리  
> clean -x, -X : 이그노어 파일  
