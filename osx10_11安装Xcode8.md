#黑苹果OXS10.11 安装Xcode8.2.1
<center>
<img src="https://avatars1.githubusercontent.com/u/16749698?s=460&v=4" width="25%" height="25%"/>
<br/>
<font color="Gray">作者：潘全星   日期：2018-02-06</font>
</center>
[**cordova-ios**](https://www.npmjs.com/package/cordova-ios)需要Xcode 8.x以上平台。Mac OS X10.11只支持Xcode  7.x到Xcode 8.2.1。安装Xcode 8.2.1建议将系统更新到Mac OS X10.11.6。

##1.下载Xcode 8.2.1
* 进入[**苹果开发者中心下载**](https://developer.apple.com/)在菜单**Acount**中登陆你的开发者账户。
* 进入**Download Tools**找到[**See more downloads**](https://developer.apple.com/download/more/)点击进入（往往用于下载旧版本Xcode）。
* 在列表中找到[Xcode 8.2.1](https://download.developer.apple.com/Developer_Tools/Xcode_8.2.1/Xcode_8.2.1.xip)点击下载Xcode 8.2.1.xip。

##2.安装Xcode 8.2.1
* 确保你的Mac系统安装了**The Unarchiver**，如果没有就到App Store中搜索并下载。
* 使用**The Unarchiver**解压Xcode 8.2.1.xip到下载目录得到Xcode.app。
* 初次运行需要验证，旧版本Xcode往往会卡在`正在验证中...`，验证通过后直接将Xcode.app拷贝到应有程序文件夹中进行覆盖即可。

##3.如何跳过验证
* 在Mac OS下，所有下载到`.dmg`安装文件打开都需要验证来源和里面软件源`.app`文件。
* 跳过来源验证：
	- 在`设置－>安全性与隐私－>通用`的`允许从以下位置下载的应用`设置为`任何来源`，建议安装完dmg安装包后，恢复原来设置。
* 跳过软件源验证(你已经确信安装的应用是安全的)：
	- 将在App Store以外下载的`.dmg`文件安装到一个位置，变成`.app`文件。
	- 在终端中允许：
	```
	$ sudo xattr -dr com.apple.quarantine 路径/Xcode.app
	```
	如果你是管理员用户可以不加`sudo`，否则需要加上。