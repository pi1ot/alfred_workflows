alfred_workflows
================

Safari UserAgent Switcher.alfredworkflow
---------------------------
* 用于快速修改Safari当前页面的UserAgent并刷新，主要用途是快速切换不支持H5视频播放的网站到iPad/iPhone方式
* 默认启动命令“ua”，支持选项：auto/ipad/iphone
* 依赖：
	- 将Alfred加入隐私控制名单
	- 在Safari偏好设置中打开显示“开发”菜单
	- AppleScript控制菜单点击和系统语言及App版本有关，非中文版本Safari 10用户需要自己修改Workflow中的AppleScript代码

Search Tools.alfredworkflow
---------------------------
* 谷歌(g)、维基百科(k)、微博(w)、知乎(z)、必应(b)、新浪新闻(n)、IMFDB(imf)的实时搜索工具，括号中为默认热键
* google和wikipedia接口默认通过本地goagent代理（127.0.0.1:8087）和HTTPS访问，若需修改请编辑search.py中set_proxy()函数
* 因谷歌、微博、知乎未提供不限流量可匿名访问的API，故其结果均为解析HTML输出而得，若有改版可能失效

google-translate-cli.alfredworkflow
-----------------------------------
* input window:
	- zh {words}:		translate words into chinese
	- en {words}:		translate words into english
* depends on google-translate-cli
	- https://github.com/soimort/google-translate-cli
	
jEdit.alfredworkflow
--------------------
* input window:
	- j {file}:		open file with jedit
	- e {text}:		edit text with jedit
* hotkey:
	- ctrl-cmd-j:		open selected file with jedit
	- ctrl-cmd-e:		edit selected text with jedit
	- ctrl-cmd-p:		edit clipboard text with jedit
* tips:
	- change path of jedit.app and paste_new.bsh first
	
Quick Search & Browse.alfredworkflow
------------------------------------
* hotkey:
	- ctrl-cmd-g:		search selected word
	- ctrl-cmd-l:		open selected url
	- ctrl-cmd-t:		translate selected words ( en -> cn )
