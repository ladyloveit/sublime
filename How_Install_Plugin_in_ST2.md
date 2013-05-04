# 如何安装Sublime Text 2的插件

本文针对那些对[Sublime Text 2](http://www.sublimetext.com/)没有任何基础的童鞋。就像Vim一样，Sublime Text 2具有一定的学习曲线，只有当你学习了解它一段时间后，才能领略它的强大。它被人称为当今最酷最性感的编辑器。

让我们先从安装开始，渐渐了解它的强大之处。

首先在[这里](http://www.sublimetext.com/2)下载你需要的Sublime版本，目前它还是开发版，但已经相当稳定。安装好之后，我们就可以进行插件的安装了。

首先我们需要安装[Package control](http://wbond.net/sublime_packages/package_control)。[Package control](http://wbond.net/sublime_packages/package_control)是必装插件，所有其他的插件和主题都可以通过它来安装。希望它能集成在正式版中。

## <a name="InstallPackageControl">如何安装Package control</a>

要安装"Package Control"，打开Sublime，按下<code>Control + \`</code>(Mac)或者<code>Ctrl + \`</code>(Windows)，然后粘贴上下面的代码：

	import urllib2,os;pf='Package Control.sublime-package';ipp=sublime.installed_packages_path();os.makedirs(ipp) if not os.path.exists(ipp) else None;open(os.path.join(ipp,pf),'wb').write(urllib2.urlopen('http://sublime.wbond.net/'+pf.replace(' ','%20')).read())

然后重启Sublime Text，点击`Preferences -> Package Settings`。如果安装成功了，Package Control会出现在菜单里。

![Package Control](Sublime_Text2_Tips_Tricks/PackageControl.png)

## <a name="UsePackageContol">如何使用Package control安装插件</a>

假设我们要使用Package Control安装插件[Alignment](http://wbond.net/sublime_packages/alignment)这个插件:

- 按下`Shift + Command + P` (Mac)或者`Shift + Ctrl + P`(Windows)调出命令面板
- 输入`install`，你会见到`Package Control: Install Package`，选中它按下Enter
- 等待片刻，会弹出一个插件列表，找到"Alignment"，按下Enter安装它
- 完成了，就这么简单！然后按下`Shift + Command + A`(Mac)或者`Ctrl + Alt + A`(Windows)来进行自动对齐吧。

![使用Package Control安装Sublime Alignment插件](Sublime_Text2_Tips_Tricks/InstallAlignment.png)

