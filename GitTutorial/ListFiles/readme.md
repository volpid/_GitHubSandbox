
# ls-files

### options

* -c \| --cached  

    Show cached files in the output (default)

* -d \| --deleted  

    Show deleted files in the output

* -m \| --modified  

    Show modified files in the output

* -o \| others  

    Show other (i.e. untracked) files in the output

* -i \| --ignored  

    Show only ignored files in the output. 

* -s \| --stage

    Show staged contents' object name, mode bits and stage number in the output.

* -u \| --unmerged

    Show unmerged files in the output (forces --stage)

* -k \| --killed

    Show files on the filesystem that need to be removed

* --exclude-standard

    Add the standard Git exclusions

* -v

    identifies the file status  
    lowercase letters for files that are marked as assume unchanged

        H : cached
        S : skip-worktree
        M : unmerged
        R : removed/deleted
        C : modified/changed
        K : to be killed
        ? : other

***

### Usage

* list ignored files

    > git ls-files \<path\> --ignored --exclude-standard -- others

* list untracked files

    > git ls-files --others --exclude-standard

    It\'s possible use git clean dry run

    > git clean -n

* list assume unchanged file 

    > git ls-files -v | grep \'\^[[:lower:]]\'