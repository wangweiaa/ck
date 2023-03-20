1、检查一下用户名和邮箱是否配置（gitlab支持我们用用户名或邮箱登录）

```jsp
git config --global  --list
```

1.在本地创建一个git仓库

~~~
git init
~~~

2.将项目添加到暂存区

~~~
git add .
~~~

3. 将项目提交到git仓库

~~~
git commit -m "提交信息" 
~~~

4.本地git仓库与远程仓库关联（两种方式：1.https方式；2.SSL方式）

~~~
git remote add origin git@github.com:wangweiaa/ck.git
~~~

~~~
git remote add origin https://github.com/wangweiaa/ck.git
~~~

5.将项目推送到远程仓库

~~~
git push -u origin master
~~~

