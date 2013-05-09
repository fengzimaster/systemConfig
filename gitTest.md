# Git test commond
## 新建仓库
> git init 
> git clone remote-repository

## 新建裸库 
> git init --bare

## 常规操作
> git status
> git log
> git add 
> git commit 
> git branch
> git checkout

## 差异比较
> git diff 比较索引库中和工作目录中的差异
> git diff --cached 比较索引库中和HEAD差异

## 取消操作
> git checkout --filename 取消工作目录下文件的修改
> git reset HEAD filename 取消 上次add操作文件的修改
> git commit -amend 取消提交
> git reset HEAD --hard 取消当前head后所有修改
> git reset HEAD^ --soft 回滚到head的前一个提交，所做修改仍然保存
> git reset HEAD^ --hard 回滚到head的前一个提交，修改不保存

##远程仓库操作
> git remote add 
> git remote -v
> git push remote branch
> git pull remote



