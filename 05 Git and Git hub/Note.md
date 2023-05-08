# An introduction to GitHub
![](./Screenshot%202023-05-04%20at%2009.50.21.png)
## GitHub account
- 删除远程git仓库
git remote rm origin
- 删除本地仓库
 ls -a  #找到目录下.git
 rm -rf  .git   #删除
- git token重新配置
[token 配置](https://blog.csdn.net/qq_36160277/article/details/119785943)
- 源引用规格 master 没有匹配
  - git branch -a 
  local,local tracking branches+remote tracking branches
  - git branch -r
  查看远程分支
  - 本地分支的名称，要与远程分支的名称保持一致
  - git remote show origin: show detailed configuration
## local master branch and remote branch 
![](./Screenshot%202023-05-04%20at%2014.42.42.png)
  - git ls-remote
  查看远程分支
## git pull
git fetch + git merge
[Caution] 在使用git pull的时候，需要明确merge的本地仓库名称，即：
> git pull <远程> <分支>
> 举例：git pull origin master
## local tracking branch 
![](./Screenshot%202023-05-04%20at%2015.19.41.png)
- git branch --track local_tracking_branch_name remote_tracking_branch_name
when created a local tracking branch, you can edit files in this branch and then, **git push** to remote tracking branch
[caution] local and remote tracking branch should have the same name
git branch -vv: shows local tracking branches and thier remotes
- overview
![](./Screenshot%202023-05-04%20at%2016.42.56.png)
## git clone
git clone URL
## Summary 
![](./Screenshot%202023-05-04%20at%2021.55.08.png)