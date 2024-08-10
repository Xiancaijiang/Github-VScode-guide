# Github

## 1.Git 和 Github分别是什么
Git 是一个运行在你电脑上的版本控制软件，而Github是基于Git这个版本控制软件打造的网站。
Git的三个概念:提交 commit、仓库repository、分支 branch。

## 2.安装

### 2.1 git安装

- git

- https://gitforwindows.org

	点击Download

![image-20240810151620241](./Github/image-20240810151620241.png)

直接双击安装包，出现界面后点Next

![image-20240810151634338](./Github/image-20240810151634338.png)

改到你想要的位置（最好别C盘）,Next

![image-20240810151646684](./Github/image-20240810151646684.png)

默认即可，;on the desk桌面快捷方式/windows explorer integration资源管理器集成可以勾上，Next

![image-20240810151718476](./Github/image-20240810151718476.png)

Next

![image-20240810152146824](./Github/image-20240810152146824.png)

默认vim，建议改成VS code，如下图，然后点击Next

![image-20240810152248548](./Github/image-20240810152248548.png)

后面全部默认，有一些新出现的功能可以不用管

最后一个界面点击，Install,下载完成如下

![image-20240810152519948](./Github/image-20240810152519948.png)

安装好了可以找到

![image-20240810152621081](./Github/image-20240810152621081.png)

### 2.2 vscode安装

https://code.visualstudio.com/



## 3. 使用

来github，我们要尊重别人的知识，但是你看到好的项目，看到了就是自己的了（bushi

### 3.1 拉取项目

#### 3.1.1 拉取方法

首先找到一个github开源的链接，以下以mick-robot举例，这是一个开源的自主导航小车项目，当前地址的代码为麦克纳姆轮和四轮差速ROS底盘的ROS导航节点包[RuPingCen/mick_robot: 基于激光传感器实现了简易的自主导航demo-开源自主导航小车项目(mick) (github.com)](https://github.com/RuPingCen/mick_robot)

打开页面，点击code,出现如下

![image-20240810153344842](./Github/image-20240810153344842.png)

- 直接Download ZIP，得到的是文件夹而不是仓库,唤醒git bash窗口输入

	```
	git init     //可以得到git 仓库，有仓库你才和git有关系，方便加入团队写代码
	```

- 也可以通过github远程托管仓库地址，首先复制这个地址https://github.com/RuPingCen/mick_robot.git

	打开你准备好的文件夹，右键点击 git bash here

![image-20240810153701473](./Github/image-20240810153701473.png)

在唤醒的git bash窗口，输入

```
git clone <git 仓库地址>
```

![image-20240810154151695](./Github/image-20240810154151695.png)

git clone成功如下

![image-20240810154321778](./Github/image-20240810154321778.png)

![image-20240810154337253](./Github/image-20240810154337253.png)

#### 3.1.2 注意事项

- 可以收藏该库，点击右上方Star,之后点击自己头像，选择your star就能顺利找到了

- 还有一个README.md区域，作者往往会把项目整体介绍或者使用方法放这，必看

	和本教程一样都是markdown文档，大家也可以学习

	![image-20240810155246290](./Github/image-20240810155246290.png)

- LICENCE：想直接拉取仓库要注意，知识产权也是很重要的

- commit ：可以观看整个项目的成长历史（多次提交过程），点击下图55 Commits处（代表55次提交）

![image-20240810155230490](./Github/image-20240810155230490.png)

然后能看到项目的update过程，也是我们学习项目构建的好方法

![image-20240810155431441](./Github/image-20240810155431441.png)

- branch,点击master可以观看分支（现在很多改成了main)

	![image-20240810155613326](./Github/image-20240810155613326.png)

- Issues，作为开源项目总是有人会提出疑问或改进意见，点击上方Issues就相当于进入项目论坛（注意礼貌
	- open:未解决
	- closed:已解决

![image-20240810155807328](./Github/image-20240810155807328.png)

### 3.2 寻找合适的项目

你熟悉的社区就是最适合的寻找地方了，比如我们的https://bbs.robomaster.com/portal.php论坛

以下是常见的、我比较推荐的几个地方

https://github.com/trending/  GitHub Trending，筛选条件自选，star数较多的

![image-20240810160550341](./Github/image-20240810160550341.png)https://github.com/521xueweihan/HelloGitHub  汉语内比较有名的媒体推荐，对我们倒没那么有用

https://github.com/ruanyf/weekly   ruanyf老师写的科技爱好者周刊，介绍工具

https://www.zhihu.com/column/mm-fe  前端，我这篇文档参考作者的前端快报

- 查找技巧，常用前缀后缀

	- 找百科大全 awesome xxx，基本上最好的官方的有效的选第一个就可以了

		![image-20240810161146975](./Github/image-20240810161146975.png)

	- 找例子 xxx sample

	- 找空项目架子 xxx starter/xxx boilerplate

	- 找教程 xxx tutorial

### 3.3 创建自己的github仓库

实践中产生的工具实践中学习即可

 ![image-20240810163735229](./Github/image-20240810163735229.png)

#### 3.3.1 从工作区到本地仓库

将有.git 的仓库用VScode打开后，点击查看终端

![image-20240810164621934](./Github/image-20240810164621934.png)

出现的窗口右上方既可以找到Git Bash(集成到VS code),之后在这进行管理就行了

![image-20240810164715090](./Github/image-20240810164715090.png) 

打开代码点击下面这个也可以初始化仓库

![image-20240810202809804](./Github/image-20240810202809804.png)

进入源代码管理，更改区如下，后面有U代表是你之前仓库没有的东西

![image-20240810203410663](./Github/image-20240810203410663.png)

首先把代码加入暂停区,在终端输入

```
git add -A      //-A,工作区即当前全部代码，提交到暂停区
git checkout <文件名>     //后悔改代码也没提交，可以撤回更改的文件，不再出现在更改区
```

或者点加号

这时，你的更改区已经空了，然后提交到本地仓库，在终端输入

```
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
git commit -m "first commit"
git reset HEAD^1   //把上一次提交给撤回
```

或者在源代码管理下方框输入first commit,	Ctrl+回车即可

![image-20240810205731260](./Github/image-20240810205731260.png)

查看commit历史

```
git log --star
```

![image-20240810210011235](./Github/image-20240810210011235.png)

在VS code中安装扩展GitLens（可以将git图形化）

![image-20240810164125644](./Github/image-20240810164125644.png)

安装扩展后，你在左下角的commit也可以直接查看历史

![image-20240810210148609](./Github/image-20240810210148609.png)

并且左下角的FILE HISTORY会有效记录你的更改痕迹

#### 3.3.2 分支

让协作成为可能的工具,一般默认主分支是完成态

```
git checkout -b<branchname>       //以当前分支为基础新建分支
git branch            //列举所有的分支     
git checkout<branchname>         // 单纯地切换到某个分支
git branch -D<branchname>        //删掉特定的分支
git merge <branchname>          //合并分支，合并是种艺术，有冲突请仔细看
//代码中会高亮标出冲突，Accept current/incoming/both change，需要人为处理
git merge --abort               //放弃合并分支，放弃也是一种勇气
```

![image-20240810211448460](./Github/image-20240810211448460.png)

#### 3.3.3 上传到github仓库

github有你想要上传的目标仓库，比如我们队伍的仓库

![image-20240810212529137](./Github/image-20240810212529137.png)

```
git remote add origin https://github.com/BJFU-Forestry-Wolves/MiracleVision2.git
git branch -M main    //master都得改成main
git push -u origin main      //验证信息
```

```
git push          //之后在本地修改，在vscode终端输出
git pull          //之后在远程修改，在vscode终端输出，两端同时更新先pull再push
```

















[全文参考]:https://www.bilibili.com/video/BV1db4y1d79C?vd_source=436470546f64e53b7d4516956091ffd7

