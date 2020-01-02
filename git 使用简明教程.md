# git 使用简明教程

### 下载 git 二进制包

https://git-scm.com/downloads

选择对应os版本，默认安装即可

### 初始化配置

git config --global user.name xxx

git config --global user.email xxx@x.com

git config --list

### 

### 远程下载代码

git clone https://github.com/zjfsdnu/deer_go_guide.git

### 初始化空文件夹

git init

### 提交代码

git status

git add

git commit -m

git log

### 撤销

git checkout (git restore )

git rm --cached

git reset --hard commitID

### 分支

git branch

git checkout

git merge

git branch -d (-D)

git stash

git stash pop

### github

git push https://github.com/zjfsdnu/deer_go_guide.git master

#### 起别名

git remote add *origin* https://github.com/zjfsdnu/deer_go_guide.git

之后只需要使用*origin*替代地址即可

git push **-u** origin master 加入**-u** 之后 存储到Windows 凭据管理器 之后直接git push即可

