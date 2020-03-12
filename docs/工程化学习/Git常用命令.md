# Git常用命令

1. 下载远端的代码

   1. git clone  https://github.com/2227324689/gpmall.git

2. 创建自己的远端项目

   1. 去 github创建项目

3. 修改

   1. git status 查看当前状态

   2. git add 文件名

   3. git commit -m ’原因‘

   4.  与远程仓库关联 git remote add origin https://git.oschina.net/batrabbit/test 

   5. git push origin master 将文件push到远端master分支

   6. 拉取远程修改

      1. git  pull origin master 

   7. 获取远程分支状态

      1. git fetch  

   8. 对分支操作

      1. git branch 查看本地有哪些分支
      2. git branch -D 删除本地分支
      3. git branch -a 查看包含远程的分支

   9. 查看远端分支

      1. git remote -v 

   10. 合并分支

      1. git marge 分支名
      2. git rebase 分支名
      3. git add 文件名
      4. git commit -m '原因'

   11. git checkout

       1. git checkout branchName 切换分支 

       2. git checkout fileName 还原更改 

          >  PS:  . 为通配符代表全部的意思

   12. 查看变更内容

       1. git diff 查看变更内容

       2. git diff --stat 查看变更文件次数

          

4. 提升、经验

   1. git flow
   2. git tag  每次合master之前一定要打个tag
   3. .gitignore
      1. git rm --cached **/文件名 使配置在.gitignore文件里面的文件生效并删除
   
5. 常见错误由于本地与远端代码不一致导致push远端失败

git pull origin master --allow-unrelated-histories //把远程仓库和本地同步，消除差异

2、重新add和commit相应文件

3、git push origin master