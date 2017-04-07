
## 일반적인 파일 이그노어

**리포지토리에 올라간(Tracked) 파일은 이그노어파일에 적용받지 않는다.**

* \.gitignore
```
#folder
.vs/
/**/__pycache__/

#files
*.user
*.VC.db
```


***

1. Untracked 하기

    * 리포지토리에서 해당 파일 지운다.
    * 이그노어 파일에 해당 파일 추가

    ```
        git reset \<file\>
        git rm --cached \<file\>
    ```

2. Tracked 파일 로컬에서 변경 추척안하기

    * 리포지토 변경 안됨
    * 로컬 변경을 무시

    ```
    git update-index --assume-unchanged <file>
    
    #make tracked again
    git update-index --no-assume-unchanged <file>

    ```