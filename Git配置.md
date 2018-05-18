# git 配置

##### 设置git的userName 和email

```
git config --global user.name"xxx"

git config --global user.email "xxx@xx.com" 

```

## ssh key实行免密码登录

##### 检查是否已经有ssh秘钥

```
cd ~/.ssh

```

##### 生成ssh密钥

```
ssh-keygen -t rsa -C “xxx@xxx.com”

```
这样默认会在本地的～/.ssh目录下生成id_rsa，id_rsa.pub两个文件，
id_rsa是私钥，id_rsa.pub是公钥。

##### 查看ssh密钥

```
cat ~/.ssh/id_rsa.pub

```

##### 把私钥加入到ssh中

```
ssh-add ~/.ssh/id_rsa

```

##### 测试一下
输入ssh git@server，第一次连接会请你确认，输入yesy即可。第二次连接就直接welcome你啦

```

ssh -T git@github.com

```


