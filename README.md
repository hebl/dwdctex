# dwdctex

自定义的LaTeX中文版式。

实现参考：

- 陈硕, [typeset](https://github.com/chenshuo/typeset)
- Chad Jones, [latex2](http://web.stanford.edu/~chadj/latex2.html)


## 参数

### 基础

使用[`CTeX`](http://www.ctex.org)作为中文处理的引擎，`CTeX`已经配置好了大量的供中文使用习惯的用法，可以直接
拿来使用。

### 版式

参考陈硕的版式设计，技术书籍一般为“国际十八开”：`185mm x 230mm`。

### 字体

- 中文字体采用`adobe`字体，安装`Acrobat Reader`中文版就带有这四个常用字体。
- 英文字体采用`TeX Gyre Pagella`，主页：[tex-gyre](http://www.gust.org.pl/projects/e-foundry/tex-gyre/pagella/) 
- 代码字体采用`Source Code Pro`，这是`Adobe`开源的一个字体。主页：[source-code-pro](https://github.com/adobe-fonts/source-code-pro)

由于使用`xelatex`进行编译，因此上述字体安装到系统的目录即可。

### 安装

建议安装再`$TEXMFLOCAL`目录下，路径为`$TEXMFLOCAL/tex/latex/dwdctex/dwdcstyle.sty`，然后运行`mktexlsr`更新文件信息，就可以
在多个地方写文档进行调用了。前面的路径可以使用链接（在Linux/MacOS）下。

一般情况下，以`TexLive`为例，其定义的`$TEXMFLOCAL`就是在其安装目录下的`texmf-local`目录，如果没有，可以自己建一个。