初始化本地仓库  

```

git init

```

连接远程仓库并建了一个名叫：origin的别名，当然可以为其他名字，但是origin一看就知道是别名，youname记得替换成你的用户名 

```
git remote add origin git@github.com:yourname/xxxx.git 
```

添加所有文件

```

git add .

```

添加的注释

```
git commit -m "上传项目源代码" 

```

将本地仓库的文件提交到别名为origin的地址的master分支下，-u为第一次提交，需要创建master分支，下次就不需要了  

```
git push -u origin master  

```

为避免远程仓库的版本比本地仓库的要新，每次使用先进行更新

```
git pull git@github.com:yourname/xxxx.git 

```
克隆项目

```
git clone git@github.com:yourname/xxxx.git 

```

添加 gitignore ~/dev/github/gitignore/ 是保存 gitignore 的目录

可以从 https://github.com/github/gitignore 获取最新版本的 gitignore 文件
添加 .gitignore 文件之后，每次提交时不会将个人的项目设置信息（例如：末次打开的文件，调试断点等）提交到服务器，在团队开发中非常重要

```
cp ~/dev/github/gitignore/Swift.gitignore .gitignore

```
