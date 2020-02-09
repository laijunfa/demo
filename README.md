**##Git**

**版本管理**

编码的时候有些节点非常关键,那我们就可以存个档,以防出现代码丢失等意外.

理解游戏存档

**常见版本管理软件**

1.svn

2.git

​     安装 

​        选中

![img](C:\Users\15702\AppData\Local\YNote\data\weixinobU7VjvXzd2ysX_dWnGDwrtZH-g4\82294ad540b5435d9459ad62791ce045\561255270875.png)

直接一直下一步

​        右键出现git bash就表示成功

​                 

![img](C:\Users\15702\AppData\Local\YNote\data\weixinobU7VjvXzd2ysX_dWnGDwrtZH-g4\3ac7021e4b4c44339e81d8b90f2ad5a4\561255322828.png)

**git使用步骤**

1.新建一个文件夹

2.进入到文件夹, 右键 点击  Git Bash Here 

![img](C:\Users\15702\AppData\Local\YNote\data\weixinobU7VjvXzd2ysX_dWnGDwrtZH-g4\3318bd25bbb74fb392e55c70a18f0893\561255397522.png)

,他就会出现一个小黑框

3.就在小黑框里写:  git init    (意思是初始化一个仓库)

​    会出现一个隐藏的.git文件夹. 不要动这个文件夹.

4.吃着火锅,愉快的敲着代码..

1. git  add  .

git   commit   -m "描述提交的代码"

**补充:** 

​    如果是第一次执行add commit,会出现下面这个问题

​                    

![img](C:\Users\15702\AppData\Local\YNote\data\weixinobU7VjvXzd2ysX_dWnGDwrtZH-g4\2fb3b0442f3b4b07a8e64c06336dae4b\561256313982.png)

​      这个问题的意思是: 设置你邮箱和用户名, 这个问题只会在第一次出现.   

​      注意的是:设置的时候一个一个的设置

​     git status

​                    

![img](C:\Users\15702\AppData\Local\YNote\data\weixinobU7VjvXzd2ysX_dWnGDwrtZH-g4\cbc99ae19d524581922804b931a52acc\561256053495.png)

就表示add commit 成功的

​      git  log

​                   

![img](C:\Users\15702\AppData\Local\YNote\data\weixinobU7VjvXzd2ysX_dWnGDwrtZH-g4\0a5b76b410c84441b3b88a367caf35cf\561256128351.png)

查看提交日志,

​                   有的时候会卡死, 卡死按q退出.    或者ctrl+c两次退出

**出现的问题 :**

 1.新建编写代码的文件夹,要进到文件夹里面去之后, 右键点击git bash here

 2.git init 不要写错, 出现一个.git影藏文件夹, 如果没有出现这个文件夹,检查一下自己的电脑隐藏文件夹是不是不显示.

1. 我们要提交内容, 那首先得有内容. 意思就是要写点代码, 代码要和上次不一样.
2. git add .

git commit -m"描述的信息"

这两句代码  add 和后面的点 有空格.   commit 和-m中间也有空格.

5.第一次提交会出现让你输入邮箱和用户名, 一行代码一行代码的执行. 复制的时候不要把后面的空格给复制来额

**查看设置的邮箱和用户名**

​	  git  config  user.email

​          git  config  user.name

**修改用户邮箱和用户名:**

第一种办法:  直接重新再设置一下,他就会覆盖.

​          git config --global user.email "[you@example.com](mailto:you@example.com)"           git config --global user.name "Your Name" 

第二种办法:  退出再登录

​        退出:

​         git  config  --global   --unset  user.email

​         git  config  --global   --unset  user.name

​         推荐大家使用 github注册的邮箱和用户名来登录.

​                       

**git版本穿梭(回滚)**

命令:   git    reset    --hard  版本号       //版本回滚的命令

命令:  git  log --oneline          //查看一行类型的日志,包括版本号

​              

![img](C:\Users\15702\AppData\Local\YNote\data\weixinobU7VjvXzd2ysX_dWnGDwrtZH-g4\b3704ebf2748495b9b1c6c6f692f93cf\561259844523.png)

前面黄色的就是版本号

命令:  git  reflog     //查看所有的日志,包括回滚的日志

**本地git工作流程**

![img](C:\Users\15702\AppData\Local\YNote\data\weixinobU7VjvXzd2ysX_dWnGDwrtZH-g4\60073c079cbe47fca2f89f59ef7c035e\561261071875.png)

**github**

**远程仓库**

以下这些都可以作为远程仓库.

1.github

2.gitlab

3.码云

4.公司的机房里某一台服务器(电脑)

5.....

**github 是什么**

<https://github.com/>

1.是一个免费的远程仓库

2.是一个代码托管平台,很多优秀的开源的项目都有放在github上,供大家学习/使用.

3.自嘲:"全球最大的同性交友网站"

**github和git有关系吗?**

没有,就是名字长的很像而已, 就像北大和北大某鸟的关系...

git是代码版本管理工具, 同样的工具还要svn等之类的.

github是一个代码托管平台.

**用github远程仓库托管代码使用步骤:**

**一:创建github克隆本地仓库**

1.建立远程仓库

​	1.1 

![img](C:\Users\15702\AppData\Local\YNote\data\weixinobU7VjvXzd2ysX_dWnGDwrtZH-g4\8912a1e7011a4f81957fdd864cede385\561262281600.png)

​	1.2  

![img](C:\Users\15702\AppData\Local\YNote\data\weixinobU7VjvXzd2ysX_dWnGDwrtZH-g4\a5c2ee6622ea40fda8367f4d5303f52e\561262574079.png)

   

2.把远程仓库克隆到本地

​    2.1

![img](C:\Users\15702\AppData\Local\YNote\data\weixinobU7VjvXzd2ysX_dWnGDwrtZH-g4\aeb4a761c0594e8da10d2790b3f18a5e\561262641626.png)

   2.2 复制一下这个远程仓库的地址

   2.3  来到   本地你需要把这个仓库 放到所在地 的文件夹.  右键点击git bash here

​           命令:  git clone 仓库地址

​           

![img](C:\Users\15702\AppData\Local\YNote\data\weixinobU7VjvXzd2ysX_dWnGDwrtZH-g4\b55439a9b3fd483a8ffa156c18f7b309\561262803439.png)

​           出现了done就说明克隆完成,  在当前文件夹就会出现一个和远程仓库名字一毛一样的一个文件夹.

3.在本地编码

1. add  commit  提交到本地仓库 

注意啦: 编码提交到本地,一定要进入到这个文件夹中去. 再右键点击git gitHub here 出来小黑框 

   

1. 推送到远程仓库

命令: git push

 

![img](C:\Users\15702\AppData\Local\YNote\data\weixinobU7VjvXzd2ysX_dWnGDwrtZH-g4\3fe9365573134779a6053d8f53ed0870\561263091289.png)

 出现了这个done就说明ok了.



​    

![img](C:\Users\15702\AppData\Local\YNote\data\weixinobU7VjvXzd2ysX_dWnGDwrtZH-g4\33cb8648c7ef48ac840befcb2c7567c7\clipboard.png)

![img](C:\Users\15702\AppData\Local\YNote\data\weixinobU7VjvXzd2ysX_dWnGDwrtZH-g4\01bb8a8d66a34b0b96d6161cb3fc8404\clipboard.png)

![img](C:\Users\15702\AppData\Local\YNote\data\weixinobU7VjvXzd2ysX_dWnGDwrtZH-g4\a081117fbfec443fb03c56c908264a66\clipboard.png)