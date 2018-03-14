

# Mac初体验之配置与工具

入职的第一天就给配了MacBook Pro，以前只看别人用，这次自己也体验上了，还是有点小激动，原谅我的没有追求 (~_~)。

好景不长，对于用惯了Windows和Ubuntu (diao si) 的我，终于发现还是使用不惯高大上的Mac，光看着外观好看并没有什么卵用。程序怎么安装，sad…...



## 一、应用程序安装

在网上找到想要下载的对应的Mac版的应用，应用的扩展名为dmg格式，本以为会像Windows一样，双击就安装了，然而 too young。。

![Mac初体验之配置与工具](/Users/changyafei/yafeichang.github.io/Mac初体验之配置与工具.png)

嗯，还需要将对应的图标拖动到"Applications"中。



## 二、常用工具

### 1. 软件包管理工具brew

用惯了Ubuntu的 "apt-get install"，突然间离开Ubuntu环境还真感觉不舒服，终于找到了Mac下的替代工具—— brew，安装也很简单：

```Bash
$/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

brew安装完成后，就可以使用该工具安装自己想要的软件了

如，安装wget:

```Bash
$ brew install wget
```

想要卸载通过brew安装的软件也很容易：

```Bash
$ brew uninstall wget
```

瞬间有一种Ubuntu的既视感

### 2. Alfred

Mac系统上一款专注于效率提升的著名应用。能快速打开网页、快速进行自定义搜索、查看剪贴板历史、快速查询单词等等。

具体应用参见https://www.cnblogs.com/chanshuyi/p/the_efficient_app_alfred.html

与alfred的workflow相关：http://www.alfredworkflow.com/

### 3. 跨平台MarkDown工具 Typora

Typora在三种系统下，都有相对应的版本。所见即所得，优点多多~

### 4. 终端利器 iTerm2

强大的终端利器，Mac下的终端替代者，经常与zsh一起使用

iTerm2 + zsh + oh my zsh: http://blog.csdn.net/chenyufeng1991/article/details/50492626

Oh my zsh主题相关：http://www.siguoya.name/pc/home/article/256

主题相关及iTerm2快捷键：https://www.cnblogs.com/xishuai/p/mac-iterm2.html

### 5. Dash

Dash是一个API文档浏览器（ API Documentation Browser），以及代码片段管理工具（Code Snippet Manager）。

具体使用：https://www.jianshu.com/p/bc90b212c0a7

dash与alfred结合使用：https://www.zhihu.com/question/33468993



## 三、其他相关Mac的使用教程

[程序员如何优雅地使用 macOS？](https://www.zhihu.com/question/20873070)

[开始使用Mac OS X——写给Mac新人](http://www.cnblogs.com/chijianqiang/archive/2011/08/03/2126593.html)

