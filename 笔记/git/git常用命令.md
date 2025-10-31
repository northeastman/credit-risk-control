# 一 常用命令
```
git config --global user.email "2318595275@qq.com"
git config --global user.name "northeastman"

git clone # 创建本地仓库并克隆远程仓库的全部内容
git pull # 用于将远程仓库的更新合并到本地仓库
git branch # 显示所有本地分支
git branch test # 基于当前提交创建分支test
git checkout test # 切换为test分支
git add -A # 将所有改动（包括新增、修改、删除的文件）添加到暂存区
git commit -m 'message' # 提交暂存区到本地仓库
git push origin master # 推送到远程仓库master
git merge test # 将test分支合并到当前分支，如果有冲突需要解决冲突。一般用于两个人对master创建出的分支同时进行了修改，将两人的修改合并到一起
```