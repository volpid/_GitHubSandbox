
# Git으로 버그 찾기

### 파일 어노테이션

* git blame

> git blame \<file\>
>   -L \<line Start\>,\<line end\>
>   -C

### 이진 탐색

* git bisect

1. 현재 브랜치에 문제가 있다고 표시

> git bisect start  
> git bisect bad  

2. 문제가 없는 커밋으로 이동 및 표시

> git checkout \<commit\>  
> git bisect good

3. bisect good 또는 bad 로 이진 탐색

4. 기타

> git bisect reset  
> git bisect run  
> git bisect log  
> git bisect visualize