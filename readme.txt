learn git order
 git add<file> //file must be in learngit folder
 git commit -m "message" //message explains what be modified

 //if you change the contents ,you ought to do
  git add<file>
  git commit -m "message"

//if you want to check the difference between before and now
  git diff
  
//if you want to check the contents what you forget
 git status

 //if you want to back before version
 git reset --hard HEAD^
 
//if you want to back future version
 git reset --hard commit_id

 //if you want to check the before all version
  git log

//if you want to check the future all version
 git reflog

 添加分支
 
 //创建dev分支
 git branch dev
 //切换分支
 git checkout dev 或者 git switch dev
 

 //相当于,创建并查看分支
git checkout -b dev 或者 git switch -c dev

//查看所有分支
git branch

//合并分支
git merge dev

//删除分支
git branch -d dev


查看远程库信息，使用git remote -v；

本地新建的分支如果不推送到远程，对其他人就是不可见的；

从本地推送分支，使用git push origin branch-name，如果推送失败，先用git pull抓取远程的新提交；

在本地创建和远程分支对应的分支，使用git checkout -b branch-name origin/branch-name，本地和远程分支的名称最好一致；

建立本地分支和远程分支的关联，使用git branch --set-upstream branch-name origin/branch-name；

从远程抓取分支，使用git pull，如果有冲突，要先处理冲突。