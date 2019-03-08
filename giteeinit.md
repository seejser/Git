git config --global user.name "taotao"
git config --global user.email "13621970338@139.com"
创建 git 仓库:

mkdir aiorder
cd aiorder
git init
touch README.md
git add README.md
git commit -m "first commit"
git remote add origin https://gitee.com/qingshouyun_admin/aiorder.git
git push -u origin master
已有仓库?

cd existing_git_repo
git remote add origin https://gitee.com/qingshouyun_admin/aiorder.git
git push -u origin master
