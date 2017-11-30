It is empty.

I just try to upload a new repostory, and try to practice some operation of github.

Such as to uopload a new respostory, to download someting from github, to check the information, to pull and then modify an then push.  

## 让你的PC具备推送的功能，电脑与github远端仓库绑定

git config --global user.name "xiaoxiaohanhanhan" （github账号）

git config --globa user.email "627342660@qq.com" （github邮箱）
 
ssh-keygen -t rsa -b 4096 -C "627342660@qq.com"   

cat ~/.ssh/id_rsa.pub  （私钥，将其写在github setting里，完成绑定）

通过网页，添加你的ssh

## 如何把一个本地工程上传到github

1. 在你的github账号上，添加你电脑的ｓｓｈ信息,让你的PC具备推送的功能 （如果之前已经将电脑绑定过，则之后不需要再次绑定）

2. 在github账号理创建一个新仓库，名字与本地工程文件名字一致 （githublianxi）

3. 将本地工程文件修改后，git add . 更新，git commit 即提交至本地git仓库

		cd githublianxi （进入文件夹）

		git init （初始化）

		git add .

		git commit -m "本地工程上传至远端仓库"

		（可添加多个对应远程仓库，git remote -v 查看）

4. 将本地工程提交至远端github仓库 （githublianxi）

		（可添加多个对应远程仓库，git remote -v 查看）

		git remote add origin git@github.com:xiaoxiaohanhanhan/githublianxi.git

		git push -u origin master (第一次)

		git push (后面默认用第一次那个)

之后在githublianxi即可看到对应的提交文件

## 如何在github上已有的工程上接着开发
1. 在你的github账号上，添加你电脑的ｓｓｈ信息,让你的PC具备推送的功能

		git clone git@github.com:xiaoxiaohanhanhan/githublianxi.git(如果之前已经下载可以跳过此步，但必须保证本地文件与远端同步！)
		
		cd githublianxi 

		(打开文件，做你的修改)

		git add .

		git commit -m "在github已有工程上接着开发"

		git push				





