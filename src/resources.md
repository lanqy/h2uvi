# 额外的 vi 资源

关于 vi 或其克隆已经存在于您的计算机中可能有几个很好的信息来源。其中一个是 vi 手册页，可以通过在命令行输入 man vi 来访问它们。

另一个是帮助文件，可以在使用 vi 时访问，方法是键入 :help 并按 Enter。要退出帮助屏幕，请键入 :q 并按 ENTER。

Vim 附带了一个教程，该教程以文本形式存储在 /usr/share/vim/vim61/ 等目录中。确认系统上的确切位置后，您可以导航到该目录并使用如下命令打开文件

```text
cat tutor | more
```

这假设教程在您的系统中被命名为 “tutor”。 “cat” 命令用于以只读模式打开教程。 “|” 而“更多”是标准的 Unix 命令，它们一起显示一页长文件以便于阅读。

nvi 附带了一个教程，它作为压缩文件存储在 /usr/doc/nvi/ 中。可以通过将其复制到主目录，解压缩然后使用 vi 打开它来访问此文件。例如，从您的主目录中键入：

```text
cp /usr/doc/nvi/vi.beginner.gz
gunzip vi.beginner.gz
vi vi.beginner
```

同一目录中也提供了高级教程。

关于vi及其克隆的在线资料也很多。这里介绍了一些更有用的网站：

### 教程：
- [一个非常快速和简单的 Vi 文本编辑器简介](http://heather.cs.ucdavis.edu/~matloff/UnixAndC/Editors/ViIntro.html) - 一个简短的教程。
- [Vi 的显示编辑简介](http://docs.freebsd.org/44doc/usd/12.vi/paper.html) - 由 vi 的创建者 Bill Joy 撰写的广泛教程，当时他还是加州大学伯克利分校的研究生。
- [Vi For Smarties](http://jerrywang.net/vi/) - 一个包含八个短课程的教程。

### 参考：
- [vi Reference](http://www.ungerhu.com/jxh/vi.html) - vi 命令的单页列表，可能不适用于没有经验的用户。
- [VI（和克隆）编辑器参考手册](http://www.rru.com/~meo/useful/vi/vi.rm.html) - 1998年更常见的 vi 命令概述。

### 克隆：

- [Elvis 文本编辑器](http://elvis.the-little-red-haired-girl.org/) - Elvis 的官方主页。
- [Elvis - vi 克隆](http://phys.columbia.edu/~flame/elvis/) - 关于 Elvis 的信息。
- [Lemmy Version 4.5](http://www.softwareonline.org/lemmy45.html) - lemmy 的主页。
- [Berkeley Vi Editor主页](http://www.bostic.com/vi/) - nvi 的信息和源代码，最初是作为 BSD 的一部分分发的 vi 实现。
- [vile](http://dickey.his.com/vile/) - vile 的主页。
- [Vim 编辑器](http://vim.sourceforge.net/)--Vim 的主页，由 SourceForge  主持。
- [为什么要使用 Vi 克隆？ 为何选择 VIM？](http://chronos.cs.msu.su/vim/why.html) - 讨论 Vim 的优点。
- [WinVi](http://www.winvi.de/en/) - Microsoft Windows 的免费 vi 克隆。
