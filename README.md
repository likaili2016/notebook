## 写在最前面

我的测试之路已经走了三年多了（包含一年实习），现在是第三份工作，经历的多了感悟也多了，多了些阅历与工作经历，觉得应该把这些整理一下，选择gitbook 这种记录方式的原因有很多，它看起来高大上，并且也希望自己的笔记能给别人帮助，我的笔记真的是小白教程哦，不要嫌弃

## 测试理论

\`\`\`

\`\`\`

## UI自动化测试

现在的测试招聘信息基本上都要求有自动化测试经验，可以说这个自动化测试已经越来越受重视了。不捣鼓点自动化都不好意思说自己是测试了。我最初接触的是silktest 这是一个企业级的工具，可以录制脚本，当初只用它录制了一个计算器的脚本，现在基本忘却了用法，之后接触了 QTP （当然是破解版的了）也只是简单的尝试了录制，在之后就是近几年流行起来的selenium了 selenium IED这是一个火狐的插件操作简单 上手容易 但是如果要是用它录制的话 它只支持Firefox浏览器，很有局限性， 对于兼容性很好的系统是可以采用录制脚本的方式的。但是有些系统还是建议使用某一浏览器，例如我现在测试的系统就是推荐使用chrome浏览器的 那么录制脚本就行不通了，为了实现chrome浏览器的UI自动化 我们使用了robot framework + Selenium2Library 这样的结构，本章重点讲解 robot framework+Selenium2Library 进行UI自动化

## UI自动化环境搭建

robot framework 是用python语言写的一个自动化测试框架 它还具有丰富的第三方库，robot framework 与第三方的配合就可以完成UI API App的自动化测试，详情可以访问robot framework 官网查看：[http:\/\/www.robotframework.org\/](http://www.robotframework.org/)

### 自动化测试环境搭建

1.安装 参照安装文档 [https:\/\/www.ibm.com\/developerworks\/cn\/opensource\/os-cn-robot-framework\/](https://www.ibm.com/developerworks/cn/opensource/os-cn-robot-framework/)

    ps：如果安装的是64位的python 要安装 pyw32

2.创建ride的快捷方式 参照：[http:\/\/www.fx114.net\/cuixiping\/qa-212-149474.aspx](http://www.fx114.net/cuixiping/qa-212-149474.aspx)

3.使用chrome 浏览器安装 chromewebdiver、ie也是安装iewebdirver



### 一起写UI自动化

双击ridi的小人图标出现工作页面，

!\[Alt text\]\(\/F:\/李凯丽\/gitbook\/likaili2016\/articles.png\)

### API自动化测试

### 性能测试

### 配置管理

