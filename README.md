# 写在最前面

我的测试之路已经走了三年多了（包含一年实习），现在是第三份工作，经历的多了感悟也多了，多了些阅历与工作经历，觉得应该把这些整理一下，选择gitbook 这种记录方式的原因有很多，它看起来高大上，并且也希望自己的笔记能给别人帮助，我的笔记真的是小白教程哦，不要嫌弃

# 测试理论

# UI自动化测试

现在的测试招聘信息基本上都要求有自动化测试经验，可以说这个自动化测试已经越来越受重视了。不捣鼓点自动化都不好意思说自己是测试了。我最初接触的是silktest 这是一个企业级的工具，可以录制脚本，当初只用它录制了一个计算器的脚本，现在基本忘却了用法，之后接触了 QTP （当然是破解版的了）也只是简单的尝试了录制，在之后就是近几年流行起来的selenium了 selenium IED这是一个火狐的插件操作简单 上手容易 但是如果要是用它录制的话 它只支持Firefox浏览器，很有局限性， 对于兼容性很好的系统是可以采用录制脚本的方式的。但是有些系统还是建议使用某一浏览器，例如我现在测试的系统就是推荐使用chrome浏览器的 那么录制脚本就行不通了，为了实现chrome浏览器的UI自动化 我们使用了robot framework + Selenium2Library 这样的结构，本章重点讲解 robot framework+Selenium2Library 进行UI自动化

## UI自动化环境搭建

robot framework 是用python语言写的一个自动化测试框架 它还具有丰富的第三方库，robot framework 与第三方的配合就可以完成UI API App的自动化测试，详情可以访问robot framework 官网查看：[http:\/\/www.robotframework.org\/](http://www.robotframework.org/)

### 自动化测试环境搭建

1.安装 参照安装文档 [https:\/\/www.ibm.com\/developerworks\/cn\/opensource\/os-cn-robot-framework\/](https://www.ibm.com/developerworks/cn/opensource/os-cn-robot-framework/)

```
ps：如果安装的是64位的python 要安装 pyw32
```

2.创建ride的快捷方式 参照：[http:\/\/www.fx114.net\/cuixiping\/qa-212-149474.aspx](http://www.fx114.net/cuixiping/qa-212-149474.aspx)

3.使用chrome 浏览器安装 chromewebdiver、ie也是安装iewebdirver

## 一起写UI自动化

双击ridi的小人图标出现工作页面，

![](/assets/QQ图片20160929161536.png)

工具构造简单，就这么几部分但是功能强大，现在我们就可以开始编写ui自动化脚本了。

### 第一个UI自动化脚本

1.建立一个存放脚本的工程，点击file 选择new project 给工程取一个名字并选择parent dictionary（最后建立一个新的文件夹用于存放脚本）新建工程时最好选择dictionary这样方便建立树形结构，使目录结构清晰 并且可以存放多个case suit

![](/assets/新建工程.png)

2.建立suit 点击刚刚建立完成的工程右键选择new suit；

3.建立test case 点击刚刚建立完成的suit 右键选择new test case 并给你的第一个case起一个高大上的名字。

4.导入Selenium2Library 库，点击suit后点击Library导入，点击确定后如果导入的字体是黑色的说明导入成功。（其他库的导入方法与之类似，导入前要确保安装了这些library）

![](/assets/导出library.png)

![](/assets/导入.png)

以上步骤完成就可以开始着手写脚本了，第一个case我们要完成一个百度的过程。

暂定case内容为：打开浏览器，使用百度搜索python，并打开相应的百度百科词条，关闭浏览器。

在开始写case之前要通读一下robot framework的官方文档中的关于 Selenium2Library 的关键字介绍。网址：http:\/\/robotframework.org\/Selenium2Library\/Selenium2Library.html

case已经准备好了，从哪里开始呢 是不是一点头绪都没有？思路是这样的 首先怎么实现自动打开浏览器呢，回到ride的工作区点击F5，打开了一个名叫“search keyword”的对话框 我们要在这里搜索robot framework 封装好的关键字 搜索open，第一个open browser就是我们要找的打开浏览器的关键字，下面就是这个关键字的参数

![](/assets/搜索关键字.png)

### API自动化测试

### 性能测试

### 配置管理

