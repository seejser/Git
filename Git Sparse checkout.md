# Git Sparse checkout

问题：如何只git pull 自己想要的目录，而不是全部project呢？

1.创建和初始化新的本地repository:
```
mkdir <repo> && cd <repo>
git init
git remote add –f <name> <url>
```
eg:
```
mkdir web

cd web/

git int

git remote add -f origin https://gitee.com/dapeng18/wxmall.git

```
2.允许sparse-checkout（关键）：
```
git config core.sparsecheckout true
```
3.配置sparse-checkout，将需要的目录添加到.git/info/sparse-checkout中（路径根目录为repository的.git所在位置）：
```
echo some/dir/ >> .git/info/sparse-checkout              #设置需要pull的目录，*表示所有，!表示匹配相反的
echo another/sub/tree >> .git/info/sparse-checkout

```

4.Checkout from the remote：
```
git pull origin master
```