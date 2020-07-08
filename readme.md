参照博客 https://www.cnblogs.com/alinainai/p/11080655.html 完成

1. git init // git初始化,使当前路径下识别git命令
2. git remote add github https://github.com/kll982/origin-pro.git // 添加远程仓库  git remote add <别名> <地址>
3. git remove -v // 查看是否关联成功,如果没有继续执行第二步
4. git pull github master // 拉取仓库  git pull <别名> <分支>
5. git pull github master --allow-unrelated-histories，--allow-unrelated-histories //本地提交过文件，远程仓库也提交过文件，git认为这是两个分支。可以使用git pull <别名> <分支> --allow-unrelated-histories，--allow-unrelated-histories会允许关联两个分支的历史分支
// 仓库和本地之前都未提交过,没有验证是否正确
6. git push --set-upstream github master // 推送到远程仓库  git push --set-upstream <别名> <分支>

7. 之后正常执行 git pull 和 git push 就可以