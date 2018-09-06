# gitskills

git init      把当前目录变成git可以管理的仓库

git add 文件名;     提交文件     提交到暂存区  add之后要commit一下 

git commit -m "最好填写更改描述";   告诉git把文件提交到仓库

git status     查看仓库状态

git reset --hard commit_id    回到某一版本

git log     查看提交历史      英文状态下按Q退出

git reflog  查看历史命令 查看历史记录，确定要回到哪个版本

git checkout -- 文件名      丢弃工作区的修改

git reset HEAD <file>     回到最近的版本

git rm 文件名  删除文件   删除之后commit一下

git remote add origin https://github.com/233-3/learngit.git   //本地仓库的内容推送到GitHub仓库   添加远程库

git push origin master //推送至github

git clone https://github.com/233-3/gitskills  //克隆到本地

git branch              //查看分支   

git branch <name>       //创建分支
 
git checkout <name>     //切换分支

git checkout -b <nmae>  //创建+切换分支

git merge <name>        //合并某分支到当前分支

git merge --no-ff -m"msg" <name>  //合并分支并加上commit

git branch -d <name>    //删除分支

git log --graph         //查看分支合并图

git log --graph --pretty=oneline --abbrev-commit   //查看分支历史

git stash   //先把工作现在给“储藏”起来 

git stash pop  //恢复工作现场

git stash list //查看被储藏工作现场 

git rebase    //可以把本地未push的分叉提交历史整理成一条直线，使查看历史提交的变化时更容易

git tag <tagname>   //创建标签

git tag -a<tagname> -m"balabala..."   //创建带有说明信息的标签  ，指定表亲

git tag                    //查看所有标签 

git show <tagname>         //查看标签信息

git tag -d <tagname>       //删除一个本地标签

git push origin <tagname>  //推送一个本地标签

git push origin --tags     //推送全部本地未推送过的标签

git push roigin :refs/tags/<tagname>  //删除一个远程标签 得先把本地的标签给删除了

如果两个分支都有新的提交 这种情况下git无法快速合并需要手动解决冲突（直接在文件里面改）然后再提交，
