Title: [git] 刪除遠端的branch
Slug: [git]_delete_remote_branch
Category: git
Author: Chris Yang
要刪除本地端的 branch 非常容易

先切換到其他的branch

然後下 <code>git branch -d  branch-name</code> 即可



然而如果要刪除遠端的branch

則必須下 <code>git push branch --delete branch-name</code>
