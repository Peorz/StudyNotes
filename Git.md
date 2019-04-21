# Git笔记

#### 在当前目录下初始化一个空的git仓库
* `git init`

#### 设置全局用户名和邮箱
* `git config --global user.name "name"` 
* `git config --global user.email "xxxxx@email.com"`
* `git config user.name` 查看git用户名
* `git config user.email` 查看邮箱配置

#### 查看git配置
* `git config --list`

#### 提交修改到暂存区
* `git add -A` 提交全部修改。（git add -All）
* `git add -u` 只提交修改，不提交新文件。（git add -update
* `git add .` 不提交删除文件
* `git add <filename>` 提交指定文件

#### 查看暂存区
* `git status`

#### 提交修改到本地仓库
* `git commit -m 'msg'` 提交暂存区到本地仓库
* `git commit -a -m 'msg'` 提交修改到本地仓库（不提交新增文件）

#### 查看提交记录
* `git log`

#### 添加远程仓库
* `git remote add <name> <url>`

#### 查看远程仓库信息
* `git remote show <name>`

#### 远程仓库的删除和重命名
* `git remote rm <remote_name>`
* `git remote rename <old_name> <new_name>`

#### 拉取远程仓库数据到本地
* `git pull <remote_name> <branch_name>`

#### 提交本地仓库到远程仓库
* `git push <remote_name> <branch_name>`

#### 查看&创建&切换分支
* `git branch` 查看已有分支
* `git branch -v` 查看已有分支及各个分支最后一个提交对象的信息
* `git branch <branch_name>` 创建新的空分支
* `git branch <branch_name> <exist_branch_name>` 创建新分支
* `git checkout -b <branch_name> <exist_branch_name>` 创建并切换到新分支
* `git checkout <branch_name>` 切换分支

#### 删除&合并分支
* `git branch -D <branch_name>` 删除分支
* `git merge <branch_name>` 当前分支合并到指定分支

#### 暂存区恢复到HEAD
* `git reset HEAD`
* `git reset HEAD <file_name>`

#### 工作区恢复到暂存区
* `git checkout -- <file_name>`