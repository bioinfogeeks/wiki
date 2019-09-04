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

+ 存好资料之后，打开README.md文件，用 **`markdown`** 语法将自己本次分享的信息 **`【按格式，规范的】`** 编辑好。编辑结束后，点击保存，准备进入下一步的 **`push`** 并且 **`merge`** 的环节。




## 参考链接 
+ https://blog.csdn.net/devnn/article/details/83386918
+ https://www.liaoxuefeng.com/wiki/896043488029600/900375748016320