# git 使用简明教程

### 下载 git 二进制包

https://git-scm.com/downloads

选择对应os版本，默认安装即可

在工作目录里 右键选择 *Git Bash Here*

### 初始化配置

git config --global user.name xxx （--global 表示存到当前用户的目录里 --system表示全部用户）

git config --global user.email xxx@x.com

git config --list


### 远程下载代码

git clone https://github.com/zjfsdnu/deer_go_guide.git

### 初始化空文件夹

git init

### 提交代码

git status （-s 简短模式）

git add xxx （. 全部修改）

git commit -m （-a 省略git add）（不加-m打开默认编辑器）

git log （-p 显示修改内容）（--stat 显示统计）

### 撤销

git checkout (git restore ) xxx

git rm --cached xxx

git reset --hard commitID

git commit --amend 覆盖上次提交

### 分支

git branch xxx

git checkout xxx

git merge xxx

git branch -d (-D 强制删除) xxx

#### 暂存代码

git stash

git stash pop

### github

git push https://github.com/zjfsdnu/deer_go_guide.git master

#### 起别名

git remote add *origin* https://github.com/zjfsdnu/deer_go_guide.git

之后只需要使用*origin*替代地址即可

git push **-u** origin master 加入 **-u** 之后 存储到Windows 凭据管理器 之后直接git push即可

