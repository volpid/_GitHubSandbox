
## git rebase 사용하기

* git rebase -i HEAD~\<num\>
1. 커밋 순서 바꾸기

![초기 log](../../Resource/Image/1_git_log_initial_state.png)
<br/>
![rebase](../../Resource/Image/2_rebase_reorder.png)
<br/>
![after log](../Resource/Image/3_git_log_after_reorder.png)

2. 커밋 합치기

![rebase](../../Resource/Image/4_rebase_squash.png)
<br/>
![after log](../../Resource/Image/5_git_log_after_squash.png)

3. 커밋 메시지 변경

![rebase](../../Resource/Image/6_rebase_reword.png)
<br/>
![after log](../../Resource/Image/7_git_log_after_reword.png)
