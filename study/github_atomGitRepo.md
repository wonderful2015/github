

## 20200127  github网站上资源库和本地资源库的连接

直接通过本地，然后 git remote add --再 push，发现不成功
github上创建仓库，然后再折腾下面命令，可以连接成功！


TerencedeMBP:github xmly$ echo "# github" >> README.md
TerencedeMBP:github xmly$ git init
Reinitialized existing Git repository in /Users/xmly/github/.git/
TerencedeMBP:github xmly$ git add README.md
TerencedeMBP:github xmly$ git commit -m "first commit"
[master 289b94e] first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
TerencedeMBP:github xmly$ git remote add origin git@github.com:wonderful2015/github.git
TerencedeMBP:github xmly$ git push -u origin master
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (11/11), 3.58 KiB | 1.79 MiB/s, done.
Total 11 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), done.
To github.com:wonderful2015/github.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
TerencedeMBP:github xmly$
TerencedeMBP:github xmly$
