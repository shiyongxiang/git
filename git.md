hwo to used fastly
=================================
#1.下载及开始的配置

	#install:
	sudo aptitude install git
	sudo aptitude install git-doc git-svn git-email git-gui gitk

	#config：
	git config --global user.name "SmallStrawHat"		(设置git账户名)
	git config --global user.email jiaqizhang79@gmail.com	(设置email)
	git config --global color.ui true			(开启颜色显示)
#2.本地操作

	#git创建仓库(如，test)：	
	mkdir test
	cd test
	git init	(执行之后，会建立一个隐藏的.git文件夹)

	#git提交到服务器
	ps:git文件有三种状态：本地，暂存，版本库。只有版本库里的文件可以上传到远程服务器。
	
	git add change-file	(或者git add -A 添加所有的改变)
	git commit -m "change file" (必须加-m)
#3.远程操作

	git clone ssh-address 克隆远程的仓库	(or git clone https-address)
	git push 将自己本地的文件推送到远程服务器上（版本库里的文件）
	git pull 将远程服务器的文件拉到本地
