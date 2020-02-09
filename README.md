**一.Git的使用**

**1.Git使用前的配置**

​	在使用git前,需要告诉git你是谁,在向git仓库中提交时需要用到 

​	(**推荐大家使用 github注册的邮箱和用户名来登录**)

```text
  1.配置提交人姓名: git config --global user.name "用户名"text
```

```text
  2.配置提交人邮箱: git config --global user.emial "邮箱"		
```

​	**查看设置的邮箱和用户名**

​	  git  config  user.email

​          git  config  user.name

**2.提交步骤**

​	1.git init 初始化git仓库

​	2.git status 查看文件状态

​	3.git add 文件列表  (添加到缓存区)

​	4.git commit -m  "提交代码的描述" 

​	5.git log 查看提交记录

**3.恢复记录(回滚)**

```text
$ git reset --hard 版本号 
```

```text
$ git log --oneline   (查看历史版本)
```

```text
$ git reflog (查看所有的日志,包括回滚的日志)
```

**(2)（最好操作一下）注意在每次提交之前要首先进行pull，这是防止冲突**

**二.将本地项目与GitHub进行关联**

**(1)这一步是本地和远程服务器建立联系的一步，后面链接为github远程仓库**

```text
$ git remote add origin https://github.com/xxx/xxx.git
```

**(2)（最好操作一下）注意在每次提交之前要首先进行pull，这是防止冲突**

如果远程主机的版本比本地版本更新，推送时Git会报错，要求先在本地做git pull合并差异，然后再推送到远程主机，这是正常合理的代码提交流程。

```text
$ git pull origin master
```

如果失败，在进行git pull 时，添加一个可选项，告诉 git 允许不相关历史合并

```text
$ git pull origin master --allow-unrelated-histories
```

or

```text
$ git pull --rebase origin master 
```

**还有一种方法 强推 本地强制上传到远程，把远程的覆盖，不推荐：**

```text
$ git push -f origin master 
```

**(3)最后推送到Github远端：**

```text
$ git push -u origin master
```

