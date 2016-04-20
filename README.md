# GitHubMem
1.创建分支
git checkout -b mybranch1 
2.添加文件
git add README.md
3.提交修改
git commint -m "update readme" 
4.提交到仓库
git push -u origin mybranch1 
5.添加tag
git tag -m "add all file onto master"     masterv1.0
6.查看tag
git tag -l -n1 
7.分享标签到远端仓库
git push origin [tagname] 
8.合并分支到master
如果出现问题，首先建立一个分支，然后进行修复，测试ok之后
git checkout -b  mybranch2
vim index.html
git commit -a -m 'fixed the *****'
回到master分支，并将修复的分支合并过来
git checkout master
git merge mybranch2 
