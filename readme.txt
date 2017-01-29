git is a distributed version control system
git is free software
git has a mutable index called stage
git track changes

工作区(WORKING Directory)：即learnGit
版本库(Repository)：位于工作区中一个隐藏目录.git，这不是工作区而是git的版本库
版本库中有一个名为Stage的暂存区和git自动创建的第一个分支master以及指向master的指针HEAD
add命令将工作区的内容提交到暂存区(STAGE)，commit命令将暂存区的内容提交到当前分支
commd:
git init:初始化仓库
git add:添加文件到仓库
git commit -m "":提交(只会把暂存区的内容提交修改,如果修改后的内容没有add加入暂存区，就不会记录这次修改)
git status:查看仓库状态
git diff：查处仓库有哪些改变
HEAD:指向当前版本
git log 或者 git log --pretty=online:查看历史提交记录(COMMIT命令),包含commit_id，用来返回历史版本
git reset --hard HEAD^:返回历史上的那个版本(一个^表示上一个，二个^表示上上一个...
当然往上100个版本写100个^比较容易数不过来，所以写成HEAD~100)
git reset hard commit_id:要想再次回到未来的版本使用commit_ID
git reflog：显示了每一次提交的情况，可以用来查找commit_id(要重返未来，
用git reflog查看命令历史，以便确定要回到未来的哪个版本。)
