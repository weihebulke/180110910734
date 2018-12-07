## 软件
- 文本编辑软件：Notepad++/Sublime/Visual Studio Code/Editplus/。。。。。。
- 图像处理软件
- 版本管理软件SVN/**Git**
- 浏览器 **Google Chrome**/FireFox

## 入门的过程
1. 新建空白文档，输入少量代码后保存，务必加上“.html”后缀
1. 浏览器打开正在编辑的html文件
1. 边保存边刷新
1. 参考http://www.w3school.com.cn

## 版本管理软件Git的使用
1. https://git-scm.com
1. 安装，然后“以管理员身份运行”
1. cd /d/cwf/workspace
1. ls 列出当前文件
1. git init创建版本仓库
1. git add . 将当前目录下的所有文件进行版本跟踪
1. *git status 显示当前版本的信息*
1. git commit -m "message" 将当前版本提交至仓库（.git）
> 后续执行`git add .`和`git commit`命令提交即可保留完整的本地版本
1. 在https://github.com或https://coding.net网站注册用户
1. 在网站上创建项目
1. git remote add origin https://git.coding.net/xxx/xxxx 添加远程仓库 
1. git push[ -u origin master]第一次上传需要添加参数，后续可省略[]内参数
> - 如果远程的仓库有内容，则会失败，需要先pull远程内容，并commit
> - git pull origin master --allow-unrelated-histories
> - 再次执行git push[ -u origin master]
1. git clone https://git.coding.net/cwfzufe/Internet2018.git 首次克隆仓库
1. git pull 后续拉取更新

## git快速上手指南 (coding.net与腾讯合作，因此可以参考下面的指南)
1. 访问https://coding.net，注册用户（xxxxx，自取），以学号1234567890作为项目名称创建空项目
1. 可以重复下列步骤完成版本管理
> - 通过cd命令进入合适的目录，
> - 首次，使用git clone https://coding.net/xxxxx/1234567890 下载自己的项目；后续，使用git pull命令拉取最新代码，
> - 然后将所有代码自行组织在1234567890目录下面
> - 需要提交时，依次运行git add . / git commit -m "some msg" / git push 完成提交


## git快速上手指南(https://dev.tencent.com，github.com以此类推)
1.假定用户名为myname，假定新建的项目名称为1234567890，假定工作目录为D盘abcde目录

2.访问https://dev.tencent.com，微信登录，点击右上角获取用户名和密码（忘记密码请重置）

![](./img/tencent1.png)
![](./img/tencent2.png)

3.创建项目

![](./img/tencent3.png)

4.项目名称建议自己学号，务必勾选“公开源代码”选项（否则别人无法clone）

![](./img/tencent4.png)

5.项目创建之后，在右边栏可以找到如图所示的项目git地址，复制即可。

![](./img/tencent5.png)

6.根据假定，工作目录为D:\abcde，git地址为https://git.dev.tencent.com/myname/123456789.git

> - **当前电脑不存在你的项目**
> - 进入工作目录 cd /d/abcde
> - 首次复制项目 git clone https://git.dev.tencent.com/myname/123456789.git
> - 进入项目目录 cd 1234567890 
> - 所有作业代码均组织在1234567890目录下面
> - 将所有修改记录下来 git add . 
> - 提交至版本库 git commit -m "some msg"
> - 同步至远程仓库 git push
> - 完成！

> - **当前电脑已经存在你的项目**
> - 进入项目目录 cd /d/abcde/1234567890
> - 获取更新 git pull 
> - 修改、增加、删除现有项目代码
> - 将所有修改记录下来 git add . 
> - 提交至版本库 git commit -m "some msg"
> - 同步至远程仓库 git push
> - 完成！