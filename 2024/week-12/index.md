# week 12

## 好文

[Mac终极武装教程](https://44maker.github.io/wiki/Mac/index.html)

[国光的 macOS Ventura 13 优化配置（基于 ARM 平台）](https://www.sqlsec.com/2023/07/ventura.html)

## 大佬

[国光](https://www.sqlsec.com/about/)
97年人（27），网络安全工程师，UP主：国光酱

[OlegWock](https://sinja.io/)

## 好网站

[visual capitalist](https://visualcapitalist.com/)
全球趋势数据可视化分析的网站

[锚坞](https://atelier-anchor.com/)
atelier-anchor 锚坞是一家着力于字体与平面的设计事务所

[ux百科](https://uxbaike.com/)

[元素周期表](https://pt.ziziyi.com/)

[ideas about website etc.](https://supercreative.design/)

[CSS Grid Generator](https://cssgrid-generator.netlify.app/)

[languagereactor](https://www.languagereactor.com/)
Language Reactor is a powerful toolbox for learning languages. It helps you to discover, understand, and learn from native materials. Studying will become more effective, interesting, and enjoyable! 

[菜鸟程序员须知](https://icodeit.org/2017/07/tips-for-newbies/)

[js -> python](https://luckrnx09.com/python-guide-for-javascript-engineers/zh-cn/)

[A姐分享](https://www.ahhhhfs.com/)

[AI时间线如何使用](http://www.ai-timeline.top/)
AI时间线是一款基于AI将某个事件以时间线的方式产出的AI网站，根据关键词生成时间线的在线AI工具，是作者在过年期间利用半天时间开发出来的AI产品，前端就是html+css+jquery，后端主要就是java、springboot，AI时间线结果支持图片导出。

## github

[programmer knowledge](https://github.com/mtdvio/every-programmer-should-know)
程序员应该知道的计算机科学、算法数据结构、分布式、正则、安全、可用性、代码设计、工程哲学

[Awesome Prompts](https://github.com/ai-boost/awesome-prompts)
开源OpenAI GPT Store优质ChatGPT提示词库，这个很好啊，好的prompt能正准确快速的得到想要的答案。

[ChatGPT提示词生成器](https://mitenmit.github.io/gpt/)
GPT Prompting是一个在线ChatGPT提示词生成器，支持 ChatGPT、Bard、Claude2 等提示词模板在线生成，内置各种角色模版，选择合适的提示词模版，按需填入需求即可生成相应的提示词，直接复制使用即可，不过暂不支持中文。

[AI时间线如何使用](https://github.com/zhugezifang/ai_timeline)


## CSS

```css
@media (prefers-color-scheme: dark) {
  html {
    filter: invert(1) hue-rotate(180deg);
  }
  html img,
  html video {
    filter: invert(1) hue-rotate(180deg);
  }
}
```

这段 CSS 代码利用了媒体查询（Media Query）和 `prefers-color-scheme` CSS 特性，来为支持深色模式的设备提供一个反色的样式，使网页的颜色方案与操作系统的深色模式相匹配。

媒体查询 `@media (prefers-color-scheme: dark)` 用于检测用户系统是否设置为深色模式。如果是，那么这段媒体查询内的样式将被应用。

```css
html {
  filter: invert(1) hue-rotate(180deg);
}
```

这个样式将会对整个 HTML 文档应用一个滤镜（filter），其中 `invert(1)` 实现了颜色反转，而 `hue-rotate(180deg)` 对所有颜色进行了180度的色相旋转，这样可以保持图片中黑白色的原始状态，因为黑色和白色色相旋转后不会改变。

但是，由于这样会影响到网页中的所有元素，包括图片和视频，所以接下来的规则是一个必要的修正：

```css
html img,
html video {
  filter: invert(1) hue-rotate(180deg);
}
```

这个样式再次对 `img` 和 `video` 元素应用同样的滤镜，以便将它们的显示效果还原为原始色彩。因为两次反色和色相旋转相互抵消，图片和视频应该会显示它们原本的颜色。

这种方法的一个缺点是可能会对网站的性能有一定影响，尤其是在复杂的页面或者较老的设备上，因为浏览器需要对页面上的所有元素应用滤镜效果。同时，对于包含颜色信息的图片（例如地图或者图表），这种反色处理可能会导致信息丢失或误解。

## 工具

[shottr](https://shottr.cc/)
理想的截图工具

[自定义背景的截图生成工具](https://shots.so/)

[excalidraw](https://excalidraw.com/) web在线绘图工具(重复了，还是想在这里重复一下)

[CLI for managing the battery charging status for M1 Macs](https://github.com/actuallymentor/battery)
一个开源的电池保护工具，电池充到80停止，`brew install --cask raycast`

[Gopeed](https://gopeed.com/)
多个平台使用的下载工具

[开发tools](https://it-tools.tech/)

[简历制作](https://rxresu.me/)

## 生活

[A Good Movie To Watch](https://agoodmovietowatch.com/all/)
一个国外好电影推荐的网站

[虚实之间](https://www.xiaoyuzhoufm.com/podcast/652fda39f071cb959eef1af4)

[数学方程，JS实现](https://runjs.app/blog/equations-that-changed-the-world-rewritten-in-javascript)

## 其他

[地震学网站](https://seismo-learn.org/)

## 热榜

![](../week-12/imgs/SCR-20240318-meil.png)
