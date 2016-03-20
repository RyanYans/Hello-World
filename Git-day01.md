-------------------------
Date:2016.03.19

#今天开始静下心来学学Git和Github!
######前几天到图书馆借了本书---《Github入门与实践》，看着挺简单的，借回来就没翻几页。还自傲的认为这玩意半天都能摸透玩熟，殊不知。。。
![Github之旅](http://www.embeddedlinux.org.cn/uploads/allimg/141011/1107470.png)

##开始我的Git之旅

* Git是什么？

 Git是目前世界上最先进的分布式版本控制系统（没有之一）。

 
* Git有什么特点？

简单来说就是：高端大气上档次！(别人面前逼格高)

###1. Git入门
使用Git前，需要先建立一个仓库(repository)。您可以使用一个已经存在的目录作为Git仓库或创建一个空目录。使用您当前目录作为Git仓库，我们只需使它初始化：

	 $ git init
或者先转到要存放的目录：

	$ git init ./newrepo
从现在开始，我们将假设您在Git仓库根目录下，除非另有说明。

#####* 添加新文件

我们有一个仓库，但什么也没有，可以使用add命令添加文件。

	 $ git add filename

此时可以继续使用add... 继续添加任务文件。  
当然也有批处理方式，来到目录：

	 $ git add .

#####* 提交版本

	 $ git commit -m "Adding files because..."
-m 后面来让你写自己的版本注释信息。（强烈建议大家都写上，因为输入说明对自己对别人阅读都很重要！）

###2. Git与Github协作

* 开始前的准备
	1. 创建账号(不做累赘)
	2. 设置SSH Key:  

			$ ssh-keygen -t rsa -C "your_email@example.com"  
遇到提示按回车，接着输入密码...  
然后就会看到fingerprint值和一只<草泥马(忘了是羊还是马勒)>

		接着输入：  

				$ cat ~/.ssh/id_rsa.pub
按下回车！就会看到公开密钥内容。整体复制到github的setting—SSH Keys上。

	3. 在github上创建版本New repository:  
	
		创建成功后在版本页面会有URL---这就是仓库号啦！
	
	当然此时可以Clone该版本在你主机上。  
	git-bash下:	

		$ git clone URL

以后就是大象放到冰箱了(三部走)：

	$ git add  
	$ git commit -m "View"
	$ git push
######附上Github 简明教程：http://www.w3cschool.cc/w3cnote/git-guide.html

* 生命在于折腾嘛！

********************
********************
