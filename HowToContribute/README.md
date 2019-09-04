[toc]

## 如何协作

#### 第一步： 将远程仓库克隆到本地 
```git
git clone git@github.com:bioinfogeeks/Bioinfo-Club.git
```
+ 克隆后会出现以下信息：
```git
Cloning into 'Bioinfo-Club'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
```

#### 第二步：切换分支
+ 首先在本地新建一个 **`branch`**， 最好是以自己姓名的拼音字母作为branch的名字
```git
git branch XiangYujia
```
+ 我的界面会出现以下分支，master前有一个 **`*`**，代表我现在正处于master分支
```git
git branch  # 首先查看现在有哪些分支
#  XiangYujia
#  dev
# * master
```
+ 现在，将 **`master`** 分支切换为 **`XiangYujia`** 分支
```git
$ git checkout XiangYujia
Switched to branch 'XiangYujia'
D       Session2_0825/Genome-wide efficient mixed-model analysis for association studies..pdf
```



#### 第三步：进入本地文件夹编辑内容并push上传
+ 把自己准备的资料存入此文件夹，如下，如果我下次分享的是下面这两篇文献，那么我就把这两篇文献存入刚才从远程库克隆到本地的文件夹内

![directory](https://github.com/bioinfogeeks/wiki/blob/master/HowToContribute/pic/directory.png)

+ 存好资料之后，打开README.md文件，用 **`markdown`** 语法将自己本次分享的信息 **`【按格式，规范的】`** 编辑好。编辑结束后，点击保存，准备进入下一步的 **`push`** 环节。

![vim](https://github.com/bioinfogeeks/wiki/blob/master/HowToContribute/pic/vim.png)

+ 使用 **`git status, git add, git commit , git push origin yourBranchName `** 添加并上传刚才自己做了改动的文件
```git
git status
#On branch XiangYujia
#Untracked files:
#  (use "git add <file>..." to include in what will be committed)
#        README.md
git add README.md
git commit -m "add materials"
#[XiangYujia 0d00d37] add readme
# 1 files changed, 48 insertions(+)
# create mode 100644 README.md

git push origin XiangYujia
# Enumerating objects: 8, done.
# Counting objects: 100% (8/8), done.
# Delta compression using up to 4 threads
# Compressing objects: 100% (7/7), done.
# Writing objects: 100% (7/7), 41.68 KiB | 215.00 KiB/s, done.
# Total 7 (delta 0), reused 0 (delta 0)
# remote:
# remote: Create a pull request for 'XiangYujia' on GitHub by visiting:
# remote:      https://github.com/bioinfogeeks/wiki/pull/new/XiangYujia
# remote:
# To github.com:bioinfogeeks/wiki.git
#  * [new branch]      XiangYujia -> XiangYujia
```

#### 第四步： pull request
在本地使用git 将自己改动了的文件推送到远程库后，现在打开BioinfoGeeks的github的网页，发起一个 **`pull request`** 提交自己的修改
![newpullrequest](https://github.com/bioinfogeeks/wiki/blob/master/HowToContribute/pic/newpullrequest.png)

![openpullrequest](https://github.com/bioinfogeeks/wiki/blob/master/HowToContribute/pic/openpullrequest.png)

+ 写好后点击 create pull request的按钮

![create](https://github.com/bioinfogeeks/wiki/blob/master/HowToContribute/pic/create.png)

+ 会跳转下面的页面，那么整个协作流程就完成啦

![ok](https://github.com/bioinfogeeks/wiki/blob/master/HowToContribute/pic/2985765.png)

## 注意
+ 在第一次克隆了远程仓库后，由于仓库内容可能发生更新，所以每次修改自己的文件之前，请先修改为自己的分支，然后 **`git pull`** ，将远程的更新内容拉到本地，接着再修改文件内容以及 **`git push`**

## 参考链接 
+ https://blog.csdn.net/devnn/article/details/83386918
+ https://www.liaoxuefeng.com/wiki/896043488029600/900375748016320