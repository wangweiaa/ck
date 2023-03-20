1、检查一下用户名和邮箱是否配置（gitlab支持我们用用户名或邮箱登录）

```js
git config --global  --list
```

## git新建仓库并上传

1.在本地创建一个git仓库

~~~js
git init
~~~

2.将项目添加到暂存区

~~~js
git add .
~~~

3. 将项目提交到git仓库

~~~js
git commit -m "提交信息" 
~~~

4.本地git仓库与远程仓库关联（两种方式：1.https方式；2.SSL方式）

~~~js
git remote add origin git@github.com:wangweiaa/ck.git
~~~

~~~js
git remote add origin https://github.com/wangweiaa/ck.git
~~~

5.将项目推送到远程仓库

~~~js
git push -u origin master
~~~

## 分支

1) 切换到基础分支，比如如master分支

~~~js
git checkout master
~~~

2） 创建**并**切换到新分支

~~~js
//分布式
// 1、新建分支
git branch newBranch
// 2、切换分支
git checkout 分支名字
// 新建并切换分支
git checkout -b newBranch

~~~

3）更新分支代码**并**提交

~~~js
git add *
git commit -m "init newBranch"
git push origin newBranch
~~~

### git 如何查看与切换分支

~~~js
git branch -a
~~~

查看当前使用分支（结果列表前面*号，代表当前使用的分支)

~~~js
git branch
~~~

切换分支

~~~js
git checkout 分支名字
~~~

