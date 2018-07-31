
# git command
1.查看本地分支
```
git branch
```
2.查看远程分支
```
git branch -r
```
3.新建分支
```
git branch -b
```
4.切换分支
```
git branch branchname
```
5.提交
```
git add readme.txt 
git commit -m "branch test"
```
6.删除分支：
  ```
  git branch -d <name>
  ```
  7.git提交项目到已存在的远程分支
  ```
  git push origin dev:init
  ```
  上面命令表示，将本地的dev分支推送到origin主机的init分支。
