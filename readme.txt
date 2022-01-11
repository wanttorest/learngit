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
git checkout

//删除分支
git branch -d dev