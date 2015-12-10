## D3中文网

D3 中文网是以 D3 为主的数据可视化专业社区。包含文档、在线演示、问答、博客、书签、个人中心等多种功能。

## 项目总览

* [**项目计划**](项目计划) *&* [**进度**](项目进度)
* [**需求说明**](一期核心需求) *&* [**产品设计**](产品原型文件说明)
* [**开发组 & 分工**](分组分工)
* [**开发请进**](开发请进)

## 加入我们

<a href="https://github.com/VisualCrew" target="_blank"><b>一、申请成为 VisualCrew 成员</b></a>

* 发送邮件到：zhang_tianxu@sina.com
* QQ 群：[D3数据可视化](http://jq.qq.com/?_wv=1027&k=ZGcqYF)：205076374，[大数据可视化](http://jq.qq.com/?_wv=1027&k=S8wGMe)：436442115
* [小纸条](https://github.com/VisualCrew/d3js.org.cn/issues)

<a href="https://github.com/VisualCrew" target="_blank"><b>二、Fork & PR</b></a>

* **Fork**

1. 注册 / 登录你的 Github 账号，并 [Fork](https://github.com/VisualCrew/d3js.org.cn#fork-destination-box) 我们的项目到你的 Github 账户下；

2. clone 你的账户下已 *Fork* 的我们的项目到你本地，比如这样：

    ```
    git clone https://github.com/【你的 Github 账号】/d3js.org.cn.git
    ```

3. 新增远程主机 *d3js-org-cn* ，并关联到我们的项目库（[VisualCrew/d3js.org.cn](https://github.com/VisualCrew/d3js.org.cn)），以便实时获取我们提交的更新，如下：
    
    ```
    git remote add d3js-org-cn https://github.com/VisualCrew/d3js.org.cn.git
    ```

4. ```cd```到已 clone 的本地 *d3js.org.cn* 项目根目录，先切换到 **dev** 分支，再从 **dev** 分支新建一个分支用于你的开发，命令如下：
	
	```
	git checkout dev
	git checkout -b <你的分支名>
	```
> 注意：在新建你的分支时，请确保不会和已有的分支重名

5. 现在，你可以在新建的分支上进行开发了，在开发过程中，你可以将代码提交到你的 Github 账户下的项目，比如：
	
	```
	git push origin
	```

6. 在你的开发过程中，需要实时的获取我们提交的更新；大致步骤如：
	
	1. 获取我们的更新；
	2. 将获取到的更新合并到你的本地的对应分支上（一般是 **dev** 分支）；
	3. 将你本地的 **dev** 分支上的更新合并到你正在开发的分支：
	
	```
	# 获取我们的更新
	git fetch d3js-org-cn
	# 切换到你本地 dev 分支
	git checkout dev
	# 合并我们在 dev 分支上提交的更新到你本地的 dev 分支
	git merge d3js-org-cn/dev
	# 切换到你开发的分支
	git checkout <你的分支名>
	# 将你本地的 dev 分支上的更新合并到你正在开发的分支
	git merge dev
	```
> 如果合并时出现冲出，请保留我们的更新，酌情对应更改你的代码。

* **PR**

1. 当你开发完成，我们欢迎你将你的代码提交给我们；首先，请合并我们最新的更新，参考上面的第 6 步；

2. 然后，将你在你的分支上开发的所有更改合并到 **dev** 分支：

	```
	git checkout dev
	git merge <你的分支名>
	```

3. 把你本地的所有修改提交到你的 Github 仓库中，然后登录你的 Github 账户，查看是否所有的更新都被提交了（在你的分支中），提交命令例如：

	```
	git checkout dev
	git push origin
	```

4. 登录你的 Github 账户，进入到你 *Fork* 的项目：
 * 点击 [**New pull request**] 按钮进入到新建 PR 的页面；
 * 更改 *base fork* 的 *base* 按钮，修改分支为 **dev** 分支；
 * 更改 *head fork* 的 *compare* 按钮，修改分支为 **dev** 分支；
 * 在下面的文本框中，输入：标题、你对更改的详细描述；请尽量描述详细，比如这样的格式：

		> 问题描述：
		
		> 解决方案：
		
		> 其他补充：