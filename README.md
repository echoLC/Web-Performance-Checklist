# Web-Performance-checklist
Web-Performance-checklist is a repo that collect web performance measures.It helps you to optimize your web project performance.  



## Loading

- 对于文本资源，开启Gzip压缩，还可以使用[Brotli](https://github.com/google/brotli) 进行更好的压缩
- 压缩CSS、JS、图片等资源
- 使用CDN存储图片、字体等静态资源



## Tool

工欲善其事必先利其器，有很多因素影响你的应用加载性能，所以要有可靠的工具能够指导我们优化的方向。当然现在有很多可用的性能测试工具，下面这些是值得考虑的工具。

### Lighthouse

[Lighthouse](https://developers.google.com/web/tools/lighthouse)是一个开源的、自动化的，用来提高你网页质量的工具。你可以使用它运行在任何网站上，它能够审查网页性能、可访问性、PWA等项。你可以使用**Lighthouse** 作为Chrome的扩展，也可以使用命令行，或者把它作为一个Node模块使用。你只需要给它一个URL，它就会对页面进行一系列的审查，然后生成一个页面表现的如何的报告。每个审查项，都会有参考文档解释为什么当前审查项很重要，也会告诉你怎么修复问题。

## PageSpeed Insights

[PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/)，这个Google的工具执行一个广泛的页面分析，并交付原始结果和改进的建议，它为手机端和桌面端提供单独的报告。它的使用也很简单，只需要输入一个URL，点击Analyze按钮。它的界面如图：

![PageSpeed Insights](https://developers.google.com/web/fundamentals/performance/get-started/images/image_201.png)

它的报告建议包括简单的解释，例如“利用浏览器缓存”，一个专用性资源的列表和更多详细解释的链接。

## WebPageTest

跟[Pingdom](https://tools.pingdom.com/)类似，这个网站会针对一个URL运行一系列的测试，然后生成一系列的报告。它不仅仅可以让你从50个测试站点中选择，使用下拉菜单或漂亮的地图界面，它也可以让你指定一个浏览器甚至是一个手机设备，因此你可以比较页面在各种各样的环境下的性能。使用[WebPageTest](https://www.webpagetest.org) ，也是提供一个URL，然后选择你的首选项，点击**START TEST** 按钮即可。

![WebPageTest](https://developers.google.com/web/fundamentals/performance/get-started/images/image_203.png)

## Summary

上面列举的工具是最受欢迎，可以用来帮助度量web页面加载和性能速度。你应该尝试使用尽可能多的不同的工具来测试你的页面，并比较常见因素和一些异常值的分析。

当然，对于这些工具最合适的应用就是局部地反映了它在你工作流中的位置。考虑如下一般的建议。

- Lighthouse主要用于构建站点时的本地迭代
- WebPageTest非常适合在真实的移动设备上进行测试，并设想更真实的设置
- 如果你不确定从哪里开始，想要一个有用的改进机会的概述，那么PageSpeed Insights是很好的选择，PageSpeed Insights最近开始集成来自Chrome用户体验报告的数据，并可能最好地捕捉现实世界用户对你的站点的体验





