# **Git 学习笔记**

***

* ##[Git的概念](#Git的概念)                             
* ##[Git的基本工作流程](#Git的基本工作流程)

* ##[Git的常用代码](#Git的常用代码)

* ## [如何通过Github进行远程协作](#如何通过Github进行远程协作)

* ## [更加便利的远程传输](#更加便利的远程传输)

***

## Git的概念 

1. *工作区：* **及本地仓库，存储本地文件，存放修改文件的地方**
2. *暂存区：* **一个临时区域，用于存放“准备提交”的修改**
3. *版本库：* **Git本地存储所有提交历史的数据库**
4. *远程仓库：* **及Github上的存储库，用于在服务器上存储文件，代码**
5. *分支：* **分为主分支与功能分支，*主分支(main)*为主要的分支和最终代码文件的存储地。*功能分支*是从主分支派生的临时分支，用于开发特定功能、修复Bug或实验性代码。**

**参考文献(下同)    1. [知乎1](https://blog.csdn.net/ThinkWon/article/details/101450420)          2. [知乎2](https://blog.csdn.net/ThinkWon/article/details/94346816)**            **3.**  **[博客园](https://www.cnblogs.com/qdhxhz/p/9757390.html)**

***

## Git的基本工作流程

1. 初始化(init)仓库并配置用户信息
2. 从远程仓库**克隆(clone)**文件至本地
3. 运用编程软件对文件进行本地修改
4. 将文件**传输(commit)**至暂存区
5. 将文件**添加(add)**至本地版本库或者**推送(push)**至远程仓库

***

## Git的常用代码        

**采用于[Git快速入门指南-CSDN博客](https://blog.csdn.net/ThinkWon/article/details/101450420)**

<img src= "https://i-blog.csdnimg.cn/blog_migrate/fd8e7db8faeb8dc350d61d5980d6d8aa.png" height=700 style="float: left; margin-right: 20px;" />

***

## 如何通过Github进行远程协作     

### Github上的前置操作：

1. 进入仓库 → **Settings** → **Collaborators** → **Add collaborator**。

2. 输入成员 GitHub 用户名或邮箱，发送邀请。

3. 成员接受邀请后即可协作。

***
###Git上的联动步骤：

1. 连接本地仓库与远程仓库(**git remote add 远程仓库名 url地址** )    *<span style ="color : pink;font-size : 10px">注：远程仓库名可随便填写</span>*
2. 首次推送，需指定分支(**git push -u origin 分支名**)；后续推送直接为**git push**
3. 需要从远程仓库拉取更新(**git pull 远程仓库名 分支名**)
4. 可创建功能分支（**git checkout -b 分支名 远程仓库名/main**）*<span style ="color : yellow;font-size : 10px">注：后需再次指定推送分支名</span>*
5. **本地开发与提交**
6. **推送分支到远程**
7. 后于Github的仓库页面**选择创建PR**，在代码通过审查后选择 **Squash and Merge** 合并到分支。

***
## 更加便利的远程传输

第三方软件的应用，如Github的桌面应用[GitHub Desktop ](https://desktop.github.com/download/)

不必打开命令行手动输入代码，只需要简单的步骤便可完成仓库的克隆与上传
