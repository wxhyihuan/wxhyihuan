---
title: 如何构建和维护Blog
author: wxhyihuan
date: '2021-01-07'
slug: running-with-blogdown
categories:
  - Read
tags:
  - Markdown
  - Tutorial
---

关于这个blog的形成过程, 以前在读书的时候查一些资料会看到很多技术性相关的帖子, 一般都是会把这些资料保存到[Microsoft Onenote]中, 后来自己也尝试过用网易博客，[Google Site]，[Github Pages] 去做自己的博客，但是维护和更新相对来讲还是复杂了一些。去年开始接触一些[Markdowng]内容，并很快接触到的 [谢益辉] 老师及其所在的[RStudio]团队开发维护的[Rbookdown]，和详细的[Rmarkdown]和[Blogdown]教程，让我觉得排版和码字的工作也能变得更轻松容易，关键是您可以在完全么有[HTML，CSS，JS等]技术基础也能做好想做的事情。 

好的工具可以让工作和学习达到事半功倍的效果，而且我认为这样的工具可能对过程有良好的反馈。如果您现在或不久将来也会考虑做维护个人Blog，以便去分享和记录一些内容，至少目前为止，我认为最容易轻松和最推荐的方案就是使用 R/Rstudio + Blogdown&[Hugo] +Github/[Netfily]的 。

如何实现这个方案？那么我们一起来看看这条爬山的路吧~~

**首先**，您最好有一定[R]语言基础，或者至少能安装好 R 和[Rstudio]软件，根据您的电脑操作系统，安装方式会不同：

- Windows系统可以参考 [手把手教你在Windows系统下安装R]。

- Linux系统的发行版较多，运维或专业人士可以根据R/Rstudio官网说明安装，或结合系统发行版寻找相应的帖子参考安装。

**其次**，您需要学习掌握[Markdown]或[Rmarkdown]的基本语法。关于Markdown和Rmarkdown的异同，从我的使用(并没有很深入比较学习)来看，基本语法差不多，后者在功能(比如数学公式，Bookdown和整合Pandoc的支持)上要完善强大很多。

学习[Rmarkdown]后，更进一步的可能还需要适当了解[Rbookdown]的内容。这部分内容应该说是整个方案实现过程中最具挑战的部分，不仅需要学习新的内容，而且主要还都是英文版的(相信我，谢老师他们在整理的时候一定考虑到广大英语困难户的问题了，没有很复杂很难度读懂)。但是等你了解它，你可能会明白有人打开新世界大门。

如果您认为实在困难，那可以选择学习[Markdown]，比如这里[Markdown中文]的资料还不错，你也可以在[stackedit]边学边练。

**再次**，这里就要提到[Blogdown]和[Hugo]框架了。[Blogdown]是一个R拓展包，也是方案里构建Blog的最关键部分，你需要按照文档中的说明在R/Rstudio中安装好Blogdown包和Hugo环境。另外，文档中详细介绍Blog框架的结构和一些使用技巧，从如何下载主题，修改配置，申请免费域名和发布Blog很详细的介绍等。

关于[Hugo]其实我基本上一点也不了解它，从谢老师和以往接触到一些网络只是，大概知道它可能是一个架构什么的，可以把我们按照架构的规则设计的东西支撑起来，就是按照模特的身形，你只要按照他的身形去做自己喜欢的款式服装，完成之后给她穿上一样。所以，你只需要按照适当的方式在你的电脑上安装好Hugo就好了。

这里要特别注意一下，当你在Hugo网站找到中意的主题模板([Hugo Theme])，并下载之后，请参考主题的官方文档和Demo看是不是能正常运行和符合自己的预期，因为有的模板可能比较久远，不一定还能用，有的可能说明不完整，使用修改起来比较麻烦。

**最后**，就是部署(Deploy)我们Blog了。在完成上面的内容后，我已经快接近山顶--部署呢。所谓部署，就是把网站托管到服务器上，听上去所以这个过程有点麻烦，又是部署又是服务器的。这个方案部署可以让你一劳永逸，体验如丝一般的顺滑，有点像德芙~

这一步主要做什么呢？要确定是部署在Github上还是Netfily上。

1. 如果是部署在[Github Pages]上，你需要先按照[Great github pages]做好代码仓(repository)，然后按照Blogdown或者[Github Pages]上的说明把Blog相应的文件传上去，就可以啦。

2. 如果是部署在[Netfily]上，你需要先按照[Netfily]要求注册一个账号，然后将我们的Blog代码仓和Netfily关联起来，并设置好架构的软件发版本(默认的一般就没问题)，就可以啦。

坚持到这里，我们距离自己的Blog就只有一步之遥了！不都到山顶了吗？为啥还没完？？因为我们还要下山--实践！这部分内容我已经体验完了，相对于*学习掌握[Markdown]或[Rmarkdown]*，下山的过程可以说是到底坐缆车了~

具体的时间过程我不赘述，因为Alison Hill将这部分整理的非常详细了，而且是谢老师官方推荐哦！那么，请君移步上 Alison Hill 的缆车吧 🚋 **[Up & Running with blogdown]**。



[Great github pages]:https://docs.github.com/en/free-pro-team@latest/github/working-with-github-pages/creating-a-github-pages-site
[R]: https://www.r-project.org/
[Microsoft Onenote]: https://www.onenote.com/signin?wdorigin=ondc
[Github Pages]: https://pages.github.com/
[Google Site]: https://sites.google.com/
[Markdowng]:https://daringfireball.net/projects/markdown/
[谢益辉]: https://yihui.org/en/vitae/
[Rbookdown]:https://bookdown.org/home/
[Rmarkdown]:https://bookdown.org/yihui/rmarkdown/
[Blogdown]: https://bookdown.org/yihui/blogdown/
[RStudio]: https://rstudio.com/
[HTML，CSS，JS等]:https://www.runoob.com/
[Netfily]: https://www.netlify.com/
[手把手教你在Windows系统下安装R]: https://www.jianshu.com/p/6b80e0c46221
[stackedit]:https://stackedit.io/app#
[Hugo]: https://gohugo.io/
[Hugo Theme]:https://themes.gohugo.io/
[Up & Running with blogdown]:https://alison.rbind.io/post/2017-06-12-up-and-running-with-blogdown/