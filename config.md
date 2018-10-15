1用户名和邮箱地址的作用

用户名和邮箱地址是本地git客户端的一个变量，不随git库而改变。

每次commit都会用用户名和邮箱纪录。

github的contributions统计就是按邮箱来统计的。

2修改密码

git config --global credential.helper store (输入这个命令后,以后只要在输入一次用户名密码)

3.查看用户名和邮箱地址：

```
$ git config user.name

$ git config user.email

```
4.修改用户名和邮箱地址：

```
$ git config --global user.name "username"
 
$ git config --global user.email "email"

```
