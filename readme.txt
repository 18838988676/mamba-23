1.初始化:git init
2.查看状态:   git status
3.将本地文件添加到仓库:git add .
4.将本地文件提交到仓库:git commit -m "123"
5.本地和github关联:git remote add origin url  //去github上创建一个项目(可以和本地项目名称不通),然后获得URL https：https://github.com/18838988676/mamba-23/
6.git push -u origin master //由于新建的远程仓库是空的，所以要加上-u这个参数，等远程仓库里面有了内容之后，下次再从本地库上传内容的时候就不用-u了。

==========================================
git push 时用户的配置
Pycharm临时配置git提交的账户：
git 修改当前的project的用户名的命令为：git config user.name 你的目标用户名**;
git 修改当前的project提交邮箱的命令为：git config user.email 你的目标邮箱名**;
8888888888888@163.com
git1888888888888

如果你要修改当前全局的用户名和邮箱时，需要在上面的两条命令中添加一个参数，--global，代表的是全局。命令分别为：
git config --global user.name 你的目标用户名；
git config --global user.email 你的目标邮箱名;



配置ssh密钥：
打开你的Git目录下的 git-bash.exe ，
命令：**ssh-keygen -t rsa -C "youremail@example.com"**
把邮件地址换成你自己的邮件地址，然后一路回车，使用默认值即可.
如果一切顺利的话，可以在C盘 用户主目录里 找到 .ssh 目录，里面有id_rsa和id_rsa.pub两个文件，这两个就是SSH Key的秘钥对，id_rsa是私钥，不能泄露出去，id_rsa.pub是公钥，可以放心地告诉任何人。
然后将id_rsa.pub公钥复制到github或码云上，