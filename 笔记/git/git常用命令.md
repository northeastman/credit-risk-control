# 一、 常用命令
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
# 二 、提交git时指定忽略的文件
## 方法一：创建项目级 .gitignore 文件
```
touch .gitignore # 在项目根目录创建 .gitignore 文件
echo "*.DS_Store" >> .gitignore # 编辑文件，添加要忽略的文件类型
echo ".ipynb_checkpoints" >> .gitignore # 编辑文件，添加要忽略的文件类型
```
## 方法二：使用全局 .gitignore 文件
```
# 创建全局 gitignore 文件
git config --global core.excludesfile ~/.gitignore_global

# 编辑全局忽略文件
echo "*.DS_Store" >> ~/.gitignore_global
echo ".ipynb_checkpoints" >> ~/.gitignore_global
```

