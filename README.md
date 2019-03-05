# 1. Front-End-interview-questions
分享请标记出处: [https://github.com/petitspois/Front-End-interview-questions](https://github.com/petitspois/Front-End-interview-questions)

<!-- TOC -->

- [1. Front-End-interview-questions](#1-front-end-interview-questions)
    - [1.1. HTML](#11-html)
        - [1.1.1. DOCTYPE相关](#111-doctype相关)
        - [1.1.2. web语义化](#112-web语义化)
        - [1.1.3. 前端SEO](#113-前端seo)
        - [1.1.4. 前端性能优化有哪些](#114-前端性能优化有哪些)
        - [1.1.5. web开发中会话跟踪的方法有哪些](#115-web开发中会话跟踪的方法有哪些)
        - [1.1.6. 什么是HTML](#116-什么是html)
        - [1.1.7. XHTML和HTML有什么区别](#117-xhtml和html有什么区别)
        - [1.1.8. 浏览器页面有哪三层构成，分别是什么，作用是什么](#118-浏览器页面有哪三层构成分别是什么作用是什么)
        - [1.1.9. 页面导入样式时，使用link和\@import有什么区别](#119-页面导入样式时使用link和\import有什么区别)
        - [1.1.10. 网页制作会用到的图片格式有哪些](#1110-网页制作会用到的图片格式有哪些)
        - [1.1.11. 文本标记](#1111-文本标记)
        - [1.1.12. 行内元素、块级元素、空(void)元素，有那些](#1112-行内元素块级元素空void元素有那些)
        - [1.1.13. iframe有那些缺点](#1113-iframe有那些缺点)
        - [1.1.14. Label的作用是什么？](#1114-label的作用是什么)
        - [1.1.15. 隐藏元素的几种方法](#1115-隐藏元素的几种方法)
        - [1.1.16. 简述一下src与href的区别](#1116-简述一下src与href的区别)
        - [1.1.17. 清除浮动的方法有哪些](#1117-清除浮动的方法有哪些)
        - [1.1.18. HTTP方法](#1118-http方法)
        - [1.1.19. HTTP报文结构](#1119-http报文结构)
        - [1.1.20. HTML全局属性global-attribute有哪些](#1120-html全局属性global-attribute有哪些)
        - [1.1.21. 何为渐进增强、优雅降级](#1121-何为渐进增强优雅降级)
        - [1.1.22. \<img>的title和alt有什么区别](#1122-\img的title和alt有什么区别)
        - [1.1.23. 从浏览器地址栏输入url到显示页面的步骤(以HTTP为例)](#1123-从浏览器地址栏输入url到显示页面的步骤以http为例)
        - [1.1.24. HTML5新增元素、标签](#1124-html5新增元素标签)
            - [1.1.24.1. form相关](#11241-form相关)
            - [1.1.24.2. 增强的页面元素](#11242-增强的页面元素)
    - [1.2. CSS部分](#12-css部分)
        - [1.2.1. CSS选择器有哪些](#121-css选择器有哪些)
            - [1.2.1.1. 基本选择器](#1211-基本选择器)
            - [1.2.1.2. 多元素的组合选择器](#1212-多元素的组合选择器)
            - [1.2.1.3. CSS 2.1 属性选择器](#1213-css-21-属性选择器)
            - [1.2.1.4. CSS 2.1中的伪类](#1214-css-21中的伪类)
            - [1.2.1.5. CSS 2.1中的伪元素](#1215-css-21中的伪元素)
            - [1.2.1.6. CSS 3的同级元素通用选择器](#1216-css-3的同级元素通用选择器)
            - [1.2.1.7. CSS 3 属性选择器](#1217-css-3-属性选择器)
            - [1.2.1.8. CSS 3中与用户界面有关的伪类](#1218-css-3中与用户界面有关的伪类)
            - [1.2.1.9. CSS 3中的结构性伪类](#1219-css-3中的结构性伪类)
            - [1.2.1.10. CSS 3的反选伪类](#12110-css-3的反选伪类)
            - [1.2.1.11. CSS 3中的 :target 伪类](#12111-css-3中的-target-伪类)
        - [1.2.2. display: none;与visibility: hidden;的区别](#122-display-none与visibility-hidden的区别)
        - [1.2.3. css sprite是什么,有什么优缺点](#123-css-sprite是什么有什么优缺点)
        - [1.2.4. CSS盒模型有那几种？](#124-css盒模型有那几种)
        - [1.2.5. CSS有哪些继承属性](#125-css有哪些继承属性)
        - [1.2.6. png、jpg、gif 这些图片格式解释一下，分别什么时候用。有没有了解过webp？](#126-pngjpggif-这些图片格式解释一下分别什么时候用有没有了解过webp)
        - [1.2.7. float、position 和 display 之间的关系](#127-floatposition-和-display-之间的关系)
        - [1.2.8. 超链接访问过后hover样式就不出现的问题？](#128-超链接访问过后hover样式就不出现的问题)
        - [1.2.9. box-sizing属性？](#129-box-sizing属性)
        - [1.2.10. CSS优先级算法如何计算？](#1210-css优先级算法如何计算)
        - [1.2.11. CSS3有哪些新特性？](#1211-css3有哪些新特性)
        - [1.2.12. 请解释一下CSS3的flexbox（弹性盒布局模型）,以及适用场景？](#1212-请解释一下css3的flexbox弹性盒布局模型以及适用场景)
        - [1.2.13. 为什么要初始化CSS样式](#1213-为什么要初始化css样式)
        - [1.2.14. 对BFC规范(块级格式化上下文：block formatting context)的理解？](#1214-对bfc规范块级格式化上下文block-formatting-context的理解)
        - [1.2.15. 为什么会出现浮动和什么时候需要清除浮动？清除浮动的方式？](#1215-为什么会出现浮动和什么时候需要清除浮动清除浮动的方式)
        - [1.2.16. 上下margin重合的问题](#1216-上下margin重合的问题)
        - [1.2.17. 移动端的布局用过媒体查询吗？](#1217-移动端的布局用过媒体查询吗)
        - [1.2.18. CSS优化、提高性能的方法有哪些？](#1218-css优化提高性能的方法有哪些)
        - [1.2.19. 浏览器是怎样解析CSS选择器的？](#1219-浏览器是怎样解析css选择器的)
        - [1.2.20. 在网页中的应该使用奇数还是偶数的字体？为什么呢？](#1220-在网页中的应该使用奇数还是偶数的字体为什么呢)
        - [1.2.21. margin和padding分别适合什么场景使用？](#1221-margin和padding分别适合什么场景使用)
        - [1.2.22. 元素竖向的百分比设定是相对于容器的高度吗？](#1222-元素竖向的百分比设定是相对于容器的高度吗)
        - [1.2.23. 如果需要手动写动画，你认为最小时间间隔是多久，为什么？](#1223-如果需要手动写动画你认为最小时间间隔是多久为什么)
        - [1.2.24. style标签写在body后与body前有什么区别？](#1224-style标签写在body后与body前有什么区别)

<!-- /TOC -->


## 1.1. HTML
### 1.1.1. DOCTYPE相关

1. 告诉浏览器需要通过哪一种规范（文档类型定义，DTD）解析文档（比如HTML或XHTML规范)。
2. DTD（document type definition，文档类型定义）是一系列的语法规则，用来定义 XML 或 (X)HTML 的文件类型。浏览器会使用它来判断文档类型， 决定使用何种协议来解析，以及切换浏览器模式。
3. 浏览器模式: 3.1 标准模式、3.2 混杂模式。
    - 3.1 标准模式
      - 标准模式（standards mode）：浏览器根据W3C标准来渲染页面。
    - 3.2 混杂模式
      - 混杂模式（quirks mode）：浏览器采用更加宽松的、向后兼容的方式来渲染页面。

      - 混杂模式下，浏览器会模仿旧浏览器的行为，比如IE6，在此基础上兼容新的标准特性。 混杂模式又称兼容模式、怪异模式等。
4. 声明文档的解析类型(document.compatMode)，避免浏览器的怪异模式。
5. 如果你是使用最新标准编写的页面但未给出 DOCTYPE 声明，这时就可能会出现一些怪异的行为。但若你声明了\<!DOCTYPE html>，那么浏览器等同于进入了标准模式，并且按照W3C标准渲染页面。

### 1.1.2. web语义化

- Web语义化是指使用恰当语义的html标签、class类名等内容，让页面具有良好的结构与含义，从而让人和机器都能快速理解网页内容。语义化的web页面一方面可以让机器在更少的人类干预情况下收集并研究网页的信息，从而可以读懂网页的内容，然后将收集汇总的信息进行分析，结果为人类所用；另一方面它可以让开发人员读懂结构和用户以及屏幕阅读器（如果访客有视障）能够读懂内容。
简单来说就是利于 SEO，便于阅读维护理解。
- 总结起来就是：
1. 正确的标签做正确的事情
2. 页面内容结构化
3. 无CSS样子时也容易阅读，便于阅读维护和理解
4. 便于浏览器、搜索引擎解析。 利于爬虫标记、利于SEO

- [拓展阅读](https://github.com/heweixiao/blog/issues/1)

### 1.1.3. 前端SEO

 1. 合理的title、description、keywords：搜索对着三项的权重逐个减小，title值强调重点即可，重要关键词出现不要超过2次，而且要靠前，不同页面title要有所不同；description把页面内容高度概括，长度合适，不可过分堆砌关键词，不同页面description有所不同；keywords列举出重要关键词即可
 2. 语义化的HTML代码，符合W3C规范：语义化代码让搜索引擎容易理解网页
 3. 重要内容HTML代码放在最前：搜索引擎抓取HTML顺序是从上到下，有的搜索引擎对抓取长度有限制，保证重要内容一定会被抓取
 4. 重要内容不要用js输出：爬虫不会执行js获取内容
 5. 少用iframe：搜索引擎不会抓取iframe中的内容
 6. 非装饰性图片必须加alt
 7. 提高网站速度：网站速度是搜索引擎排序的一个重要指标
 
### 1.1.4. 前端性能优化有哪些
 
 1. 尽量减少 HTTP 请求个数——须权衡
 2. 使用 CDN（内容分发网络）
 3. 为文件头指定 Expires 或 Cache-Control ，使内容具有缓存性。
 4. 避免空的 src 和 href
 5. 使用 gzip 压缩内容
 6. 把 CSS 放到顶部
 7. 把 JS 放到底部
 8. 避免使用 CSS 表达式
 9. 将 CSS 和 JS 放到外部文件中
 10. 减少 DNS 查找次数
 11. 精简 CSS 和 JS
 12. 避免跳转
 13. 剔除重复的 JS 和 CSS
 14. 配置 ETags
 15. 使 AJAX 可缓存
 16. 尽早刷新输出缓冲
 17. 使用 GET 来完成 AJAX 请求
 18. 延迟加载
 19. 预加载
 20. 减少 DOM 元素个数
 21. 根据域名划分页面内容
 22. 尽量减少 iframe 的个数
 23. 避免 404 （合理使用404页面）
 24. 减少 Cookie 的大小
 25. 使用无 cookie 的域
 26. 减少 DOM 访问
 27. 开发智能事件处理程序
 28. 少用@import
 29. 避免使用滤镜
 30. 优化图像
 31. 优化 CSS Spirite或字体图标
 32. 不要在 HTML 中缩放图像——须权衡
 33. favicon.ico要小而且可缓存
 34. 保持单个内容小于25K
 35. 打包组件成复合文本

 - [拓展阅读](https://juejin.im/post/5b0bff30f265da08f76cc6f0)

### 1.1.5. web开发中会话跟踪的方法有哪些
 
 1. cookie
 2. session
 3. url重写
 4. 隐藏input
 5. ip地址
 
### 1.1.6. 什么是HTML
 - HTML：HyperText Markup Language超文本标记语言
 
### 1.1.7. XHTML和HTML有什么区别
 - HTML是一种基本的WEB网页设计语言，XHTML是一个基于XML的标记语言
 
### 1.1.8. 浏览器页面有哪三层构成，分别是什么，作用是什么
 - 浏览器页面构成：结构层、表示层、行为层
 - 分别是：HTML、CSS、JavaScript
 - 作用：HTML实现页面结构，CSS完成页面的表现与风格，JavaScript实现一些客户端的功能与业务。
 
### 1.1.9. 页面导入样式时，使用link和\@import有什么区别
 1. 作用不同：link属于XHTML标签，除了加载CSS外，还能用于定义RSS, 定义rel连接属性等作用；而\@import是CSS提供的，只能用于加载CSS;
 2. 加载不同：页面被加载的时，link会同时被加载，而\@import引用的CSS会等到页面被加载完再加载;
 3. 兼容不同：import是CSS2.1 提出的，只在IE5以上才能被识别，而link是XHTML标签，无兼容问题;
 
### 1.1.10. 网页制作会用到的图片格式有哪些
 1. Webp：WebP格式，谷歌（google）开发的一种旨在加快图片加载速度的图片格式。并能节省大量的服务器带宽资源和数据空间。Facebook Ebay等知名网站已经开始测试并使用WebP格式。
 2. Apng：是PNG的位图动画扩展，可以实现png格式的动态图片效果，有望代替GIF成为下一代动态图标准。
 

### 1.1.11. 文本标记
```
1.特殊字符
  1.&nbsp; 表示一个空格
  2.&lt; 表示一个<
  3.&gt; 表示一个>
  4.&copy; 表示版权
  5.&yen; ￥
2.文本样式
  1.<b></b> :加粗
  2.<i></i> :斜体
  3.<u></u> :下划线
  4.<s></s> :删除线
  5.<sup></sup> :上标
  6.<sub></sub> :下标
```

### 1.1.12. 行内元素、块级元素、空(void)元素，有那些
1. 行内元素有：a b span img input select
2. 块级元素有: div p ul ol li dl dt dd h1-h6
3. 常见的空元素: br-换行，hr-水平分割线

### 1.1.13. iframe有那些缺点
1. iframe会阻塞主页面的Onload事件，会影响页面的并行加载；
2. 搜索引擎的检索程序无法解读这种页面，不利于SEO;
- 通过javascript动态给iframe添加src属性值，这样可以绕开以上两个问题

### 1.1.14. Label的作用是什么？
- label标签来定义表单控制间的关系,当用户选择该标签时，浏览器会自动将焦点转到和标签相关的表单控件上。

### 1.1.15. 隐藏元素的几种方法
1. display:none;
2. visibility:hidden;
3. opacity:0;
4. position:absolute; left:-10000px;

### 1.1.16. 简述一下src与href的区别
- src用于替换当前元素，href用于在当前文档和引用资源之间确立联系。

### 1.1.17. 清除浮动的方法有哪些
1. clear:both
   - 在父元素的里面添加一个空的clear的div（跟浮动的子级同级），然后再为这个类添加属性值clear:both;便可以清除浮动。
2. overflow：hidden
   - 在父元素的样式中添加overflow: hidden;也可以清除浮动，如下css代码，但不提倡使用这个方法，overflow: hidden;还有一个意思就是隐藏超出的部分，处理不好还是会给页面带来麻烦。
3. clearfix(推荐使用)
   1. 在父集元素类名中添加 clear-fix
   2. 写伪类样式
    ```
        .clearfix:after { 
            content: ".";     <----内容为“.”就是一个英文的句号而已。也可以不写。
            display: block;   <----加入的这个元素转换为块级元素。
            clear: both;     <----清除左右两边浮动。
            visibility: hidden;      <----可见度设为隐藏。注意它和display:none;是有区别的。仍然占据空间，只是看不到而已；
            height: 0;     <----高度为0；
            font-size:0;    <----字体大小为0；
        }
    ```
    
### 1.1.18. HTTP方法
1. **GET**是最常用的方法，通常用于请求服务器发送某个资源。
2. **HEAD**与GET类似，但服务器在响应中只返回首部，不返回实体的主体部分
3. **PUT**让服务器用请求的主体部分来创建一个由所请求的URL命名的新文档，或者，如果那个URL已经存在的话，就用这个主体替代它
4. **POST**起初是用来向服务器输入数据的。实际上，通常会用它来支持HTML的表单。表单中填好的数据通常会被送给服务器，然后由服务器将其发送到要去的地方。
5. **TRACE**会在目的服务器端发起一个环回诊断，最后一站的服务器会弹回一个TRACE响应并在响应主体中携带它收到的原始请求报文。TRACE方法主要用于诊断，用于验证请求是否如愿穿过了请求/响应链。
6. **OPTIONS**方法请求web服务器告知其支持的各种功能。可以查询服务器支持哪些方法或者对某些特殊资源支持哪些方法。
7. **DELETE**请求服务器删除请求URL指定的资源

### 1.1.19. HTTP报文结构
 - HTTP 报文有 请求报文 和 响应报文 两种。
 - 请求报文：从客户向服务器发送请求报文。
 - 响应报文：从服务端到客户的回答。
 - 由于 HTTP 是面向文本的，因此在报文中的每一个字段都是一些 ASCII 码串，因此各个字段的长度是不确定的。
这也造成了 HTTP 报文结构的统一性，不然无法解析出数据。
 - HTTP的这两种报文都由三部分组成：开始行、首部行、实体主体。
 1. 开始行
    - 区分请求报文与响应报文
    #### 请求报文的开始行:
    >也叫请求行，由 **方法**、[空格]、**URL**、[空格]、**HTTP**版本 组成。

    1. 方法： 向请求资源指定的资源发送请求报文的方法，其作用是可以指定请求的资源按期望产生某种行为。
    2. URL: 链接
    3. HTTP版本：目前有 HTTP/1.0、HTTP/1.1、HTTP/2.0 版本，其中 HTTP1.0 版本使用较广泛。

    #### 响应报文的开始行:
    > 也叫响应行，由 HTTP 版本、[空格]、状态码组成。

    - 状态码（Status-Code）都是三位数字的，分为 5 大类共 33 种。
    
    状态码 | 说明 | 请求行例子
    -|:-:| -
    1xx | 表示通知信息的，如请求收到了或正在进行处理|  
    2xx | 表示成功 | HTTP/1.1 200 OK
    3xx | 表示重定向
    4xx | 表示客户端的差错，如请求链接为不存在 | HTTP/1.1 404 Not Found
    5xx | 表示服务器的差错

    #### 首部行

    1. 是用来说明浏览器、服务器或报文主体的一些信息。
    2. 可以有好几行，也可以不使用
    3. 每个首部行都是由 首部字段名、[空格] 和 值 组成
    4. 每个首部行在结束地方都有 CRLF（『回车』和『换行』符）
    > HTTP 首部字段分为 4 种： 通用首部字段、请求首部字段、响应首部字段、实体首部字段。

    ![首部字段](images/http-header.png)

    #### 实体主体

    - 在请求报文中，一般是 post/put 提交的表单信息。与首部行之间有 CRLF 即空行。

### 1.1.20. HTML全局属性global-attribute有哪些

1. accesskey:设置快捷键，提供快速访问元素如aaa在windows下的firefox中按alt + shift + a可激活元素
2. class:为元素设置类标识，多个类名用空格分开，CSS和javascript可通过class属性获取元素
3. contenteditable: 指定元素内容是否可编辑
4. contextmenu: 自定义鼠标右键弹出菜单内容
5. data-*: 为元素增加自定义属性
6. dir: 设置元素文本方向
7. draggable: 设置元素是否可拖拽
8. dropzone: 设置元素拖放类型： copy, move, link
9. hidden: 规定元素仍未或不再相关
10. id: 元素id，文档内唯一
11. lang: 元素内容的的语言
12. spellcheck: 是否启动拼写和语法检查
13. style: 行内css样式
14. tabindex: 设置元素可以获得焦点，通过tab可以导航
15. title: 元素相关的建议信息
16. translate: 规定是否应该翻译元素内容

### 1.1.21. 何为渐进增强、优雅降级

- 常用两种策略：
- 要么优雅降级（graceful degradation，一开始就构建站点的完整功能，然后针对浏览器测试和修复），
- 要么渐进增强（progressive enhancement，一开始只构建站点的最少特性，然后不断针对各浏览器追加功能。

>两者间的（微妙）差别

- 万一你正挠着后脑勺，试图找出“优雅降级”和“渐进增强”之间的差别，那么我可以告诉你：“它们是看待同种事物的两种观点”。“优雅降级”和“渐进增强”都关注于同一网站在不同设备里不同浏览器下的表现程度。关键的区别则在于它们各自关注于何处，以及这种关注如何影响工作的流程。

> “优雅降级”观点

- “优雅降级”观点认为应该针对那些最高级、最完善的浏览器来设计网站。而将那些被认为“过时”或有功能缺失的浏览器下的测试工作安排在开发周期的最后阶段，并把测试对象限定为主流浏览器（如 IE、Mozilla 等）的前一个版本。

- 在这种设计范例下，旧版的浏览器被认为仅能提供“简陋却无妨 (poor, but passable)” 的浏览体验。你可以做一些小的调整来适应某个特定的浏览器。但由于它们并非我们所关注的焦点，因此除了修复较大的错误之外，其它的差异将被直接忽略。

> “渐进增强”观点

- “渐进增强”观点则认为应关注于内容本身。
- 内容是我们建立网站的诱因。有的网站展示它，有的则收集它，有的寻求，有的操作，还有的网站甚至会包含以上的种种，但相同点是它们全都涉及到内容。这使得“渐进增强”成为一种更为合理的设计范例。这也是它立即被 Yahoo! 所采纳并用以构建其“分级式浏览器支持 (Graded Browser Support)”策略的原因所在。
- GD和PE的区别在于：功能衰减是从复杂的现状开始，并试图减少用户体验的供给，而渐进增强则是从一个非常基础的，能够起作用的版本开始，并不断扩充，以适应未来环境的需要。功能衰减意味着往回看；而渐进增强则意味着朝前看，同时保证其根基处于安全地带。

### 1.1.22. \<img>的title和alt有什么区别

1. title是global attributes之一，用于为元素提供附加的advisory information。通常当鼠标滑动到元素上的时候显示。
2. alt是\<img>的特有属性，是图片内容的等价描述，用于图片无法加载时显示、读屏器阅读图片。可提图片高可访问性，除了纯装饰图片外都必须设置有意义的值，搜索引擎会重点分析。

### 1.1.23. 从浏览器地址栏输入url到显示页面的步骤(以HTTP为例)
1. 在浏览器地址栏输入URL
2. 浏览器查看缓存，如果请求资源在缓存中并且新鲜，跳转到转码步骤
   - 如果资源未缓存，发起新请求
   - 如果已缓存，检验是否足够新鲜，足够新鲜直接提供给客户端，否则与服务器进行验证。
   -  检验新鲜通常有两个HTTP头进行控制Expires和Cache-Control：
       - HTTP1.0提供Expires，值为一个绝对时间表示缓存新鲜日期
        - HTTP1.1增加了Cache-Control: max-age=,值为以秒为单位的最大新鲜时间
3. 浏览器解析URL获取协议，主机，端口，path
4. 浏览器组装一个HTTP（GET）请求报文
5. 浏览器获取主机ip地址，过程如下：
    - 浏览器缓存
    - 本机缓存
    - hosts文件
    - 路由器缓存
    - ISP DNS缓存
    - DNS递归查询（可能存在负载均衡导致每次IP不一样）
6. 打开一个socket与目标IP地址，端口建立TCP链接，三次握手如下：
    - 客户端发送一个TCP的SYN=1，Seq=X的包到服务器端口
    - 服务器发回SYN=1， ACK=X+1， Seq=Y的响应包
    - 客户端发送ACK=Y+1， Seq=Z
7. TCP链接建立后发送HTTP请求
8. 服务器接受请求并解析，将请求转发到服务程序，如虚拟主机使用HTTP Host头部判断请求的服务程序
9. 服务器检查HTTP请求头是否包含缓存验证信息如果验证缓存新鲜，返回304等对应状态码
10. 处理程序读取完整请求并准备HTTP响应，可能需要查询数据库等操作
11. 服务器将响应报文通过TCP连接发送回浏览器
12. 浏览器接收HTTP响应，然后根据情况选择关闭TCP连接或者保留重用，关闭TCP连接的四次握手如下：

    - 主动方发送Fin=1， Ack=Z， Seq= X报文
    - 被动方发送ACK=X+1， Seq=Z报文
    - 被动方发送Fin=1， ACK=X， Seq=Y报文
    - 主动方发送ACK=Y， Seq=X报文
13. 浏览器检查响应状态码：是否为1XX，3XX， 4XX， 5XX，这些情况处理与2XX不同
14. 如果资源可缓存，进行缓存
15. 对响应进行解码（例如gzip压缩）
16. 根据资源类型决定如何处理（假设资源为HTML文档）
17. 解析HTML文档，构件DOM树，下载资源，构造CSSOM树，执行js脚本，这些操作没有严格的先后顺序，以下分别解释
18. 构建DOM树：
    - Tokenizing：根据HTML规范将字符流解析为标记
    - Lexing：词法分析将标记转换为对象并定义属性和规则
    - DOM construction：根据HTML标记关系将对象组成DOM树
19. 解析过程中遇到图片、样式表、js文件，启动下载
20. 构建CSSOM树
    - Tokenizing：字符流转换为标记流
    - Node：根据标记创建节点
    - CSSOM：节点创建CSSOM树
21. 根据DOM树和CSSOM树构建渲染树:
    - 从DOM树的根节点遍历所有可见节点，不可见节点包括：1）script,meta这样本身不可见的标签。2)被css隐藏的节点，如display: none
    - 对每一个可见节点，找到恰当的CSSOM规则并应用
    - 发布可视节点的内容和计算样式
22. js解析如下
     - 浏览器创建Document对象并解析HTML，将解析到的元素和文本节点添加到文档中，此时document.readystate为loading
     - HTML解析器遇到没有async和defer的script时，将他们添加到文档中，然后执行行内或外部脚本。这些脚本会同步执行，并且在脚本下载和执行时解析器会暂停。这样就可以用document.write()把文本插入到输入流中。同步脚本经常简单定义函数和注册事件处理程序，他们可以遍历和操作script和他们之前的文档内容
     - 当解析器遇到设置了async属性的script时，开始下载脚本并继续解析文档。脚本会在它下载完成后尽快执行，但是解析器不会停下来等它下载。异步脚本禁止使用document.write()，它们可以访问自己script和之前的文档元素
     - 当文档完成解析，document.readState变成interactive
     - 所有defer脚本会按照在文档出现的顺序执行，延迟脚本能访问完整文档树，禁止使用document.write() 
     - 浏览器在Document对象上触发DOMContentLoaded事件
     - 此时文档完全解析完成，浏览器可能还在等待如图片等内容加载，等这些内容完成载入并且所有异步脚本完成载入和执行，document.readState变为complete,window触发load事件
23. 显示页面（HTML解析过程中会逐步显示页面）

### 1.1.24. HTML5新增元素、标签

#### 1.1.24.1. form相关

    1. **form属性**: 在HTML5中表单元素可放在表单之外，通过给该元素添加form属性来指向目标表单（form属性值设为目标表单id）即可。
    2. **formaction属性**：HTML5给提交按钮(如button、submit、image等)增加了formaction属性，以便提交到不同的服务器地址。
    ```html
    <input formaction="new.html" type="submit" value="提交到new.html">
    ```
    3. **formmethod**属性：用法同formaction。
    4. **placeholder**属性：用于文本框处于未输入状态时的一种文字提示。
    5. **autofocus**属性：自动获得焦点，一个页面只能有一个控件具有该属性。该属性无值，直接写就好。
    6. **list**属性：用于单行文本框，该属性的值为某个datalist元素的id，增加该属性后的单行文本框类似选择框(select)，但允许用户自定义输入，为了避免没有支持该元素的浏览器出现错误，我们通常使用CSS设置不显示。
    7. **autocomplete**属性：自动完成允许浏览器预测对字段的输入，HTML5实现了自定义设置该属性，避免了任何人都可以看到所存在的安全隐患。该属性值有“on”、”off“或“”(不指定)三种，不指定时使用浏览器的默认值。
    8. input元素种类
        - search：与text文本框类似，用于搜索；
        - tel： 与text文本框类似，用于电话；
        - url： 与text文本框类似，用于url格式的地址；
        - email： 与text文本框类似，用于email格式的地址；
        - number： 与text文本框类似，用于数值；
        - range： 只允许输入一段范围内的数值，通过min和max属性来设置范围；
        - color： 颜色文本框，“#000000”格式的文字；
        - file： 文件选择文本框，HTML5中通过multiple属性可以多选；
        -  datetime、date、month、week、time、datetime-local 各种日期与时间输入的文本框；
        -  output： 定义不同类型的输出；
    9. 表单验证相关
        - required属性：具有该属性的元素，如果其内容为空则不允许提交，并给出相应的提示。
        - pattern属性：具有该属性的元素，如果内容不为空则把内容与pattern的值进行正则匹配，匹配不成功则不通过并提示。
        - min属性和max属性：它们是值类型和日期类型的input元素专用属性，限制了输入的范围。
        - step属性：控制元素的值增加或减少的步幅，如输入1-100之间的数字，且步幅是5，那么只能输入1、6、11....
#### 1.1.24.2. 增强的页面元素
1. **figure**元素：figure是个组合元素，可以带标题figcaption，一个figure只允许放置一个figcaption。
```html
    <figure>
        <img src="logo.png" alt="图片">
        <figcaption>标志</figcaption>
    </figure>
```
2. **details**元素:details提供了一种替代Javascript的、将画面上局部区域进行展开或收缩的方法.
```html
    <details>
        <summary>点击我查看细节</summary>
        <p>我是细节内容。</p>
    </details>
```
3.  **mark**元素：mark元素表示页面需要突出显示或高亮显示的部分。
4. **progress**元素：一般用于写进度条，可以给progress设置value和max属性，value表示已经进行的，max表示总数，value和max只能为有效的浮点数，value必须大于0小于等于max。如果不给progress设置这两个属性，则是动态显示正在进行，进度不确定。
5. **meter**元素：定义度量衡。（界定上下的值会有颜色区分） 
    - high:定义度量的值位于哪个点，被界定为高的值。
    - low:定义度量的值位于哪个点，被界定为低的值。
    - max:定义最大值。默认值是 1。
    - min:定义最小值。默认值是 0。
    - optimum:定义什么样的度量值是最佳的值,如果该值高于 "high" 属性，则意味着值越高越好。如果该值低于 "low" 属性的值，则意味着值越低越好。
    - value:定义度量的值。 

6. 改良的ol列表：在HTML5中为ol元素添加了start属性和reversed属性。
7. 改良的dl列表：dl是专门用来定义术语的列表，在HTML5中为dt增加了名字dfn。
8. cite:用于表示作者。
9. small:用于标识“小型文本”。
10. \<article>标签:定义外部的内容。
11. \<aside>标签:定义 article 以外的内容。aside 的内容应该与 article 的内容相关。aside可以用于网站页尾一排排的广告或者链接，一竖排为一个aside。也可以用于博客侧栏。
12. \<audio> 标签：定义声音。
13. \<canvas> 标签：定义图形（是为了客户端矢量图形而设计的）。
14. \<command> 标签：定义命令按钮，比如单选按钮、复选框或按钮。
15. \<embed> 标签:定义嵌入的内容，比如插件
16. \<footer> 标签：定义 section 或 document 的页脚。
17. \<header> 标签：定义 section 或 document 的页眉。
18. \<hgroup> 标签：用于对网页或区段（section）的标题进行组合。
19. \<nav> 标签：定义导航链接的部分。
20. \<output> 标签：定义不同类型的输出，比如脚本的输出。
21. \<rp> 标签：在 ruby 注释中使用，以定义不支持 ruby 元素的浏览器所显示的内容。
22. \<rt> 标签：定义字符（中文注音或字符）的解释或发音。
23. \<ruby> 标签：定义 ruby 注释（中文注音或字符）。
24. \<section> 标签：定义文档中的节（section、区段）。比如章节、页眉、页脚或文档中的其他部分
25. \<source> 标签：为媒介元素（比如 \<video> 和 \<audio>）定义媒介资源。
26. \<summary> 标签：details 元素的标题，”details” 元素用于描述有关文档或文档片段的详细信息。”summary” 元素应该是 “details” 元素的第一个子元素。
27. \<time> 标签：定义日期或时间，或者两者。
28. \<video> 标签：定义视频，比如电影片段或其他视频流。
29. \<dialog>标签：定义对话（会话）dialog元素表示几个人之间的对话。

## 1.2. CSS部分

### 1.2.1. CSS选择器有哪些

#### 1.2.1.1. 基本选择器
序号|选择器|含义
-|:-:|-
1|*|通用元素选择器，匹配任何元素
2|E|标签选择器，匹配所有使用E标签的元素
3|.info|class选择器，匹配所有class属性中包含info的元素
4|#footer|id选择器，匹配所有id属性等于footer的元素

**实例：**
```css
* { margin:0; padding:0; }

p { font-size:2em; }

.info { background:#ff0; }

p.info { background:#ff0; }

p.info.error { color:#900; font-weight:bold; }

#info { background:#ff0; }

p#info { background:#ff0; }
```

#### 1.2.1.2. 多元素的组合选择器
序号|选择器|含义
-|:-:|-
5|E,F|多元素选择器，同时匹配所有E元素或F元素，E和F之间用逗号分隔
6|E F|后代元素选择器，匹配所有属于E元素后代的F元素，E和F之间用空格分隔
7|E > F|子元素选择器，匹配所有E元素的子元素F
8|E + F|毗邻元素选择器，匹配所有紧随E元素之后的同级元素F

**实例：**
```css
div p { color:#f00; }

#nav li { display:inline; }

#nav a { font-weight:bold; }

div > strong { color:#f00; }

p + p { color:#f00; }
```
#### 1.2.1.3. CSS 2.1 属性选择器
序号|选择器|含义
-|:-:|-
9|E[att]|匹配所有具有att属性的E元素，不考虑它的值。（注意：E在此处可以省略，比如"[cheacked]"。以下同。）
10|E[att=val]|匹配所有att属性等于"val"的E元素
11|E[att~=val]|匹配所有att属性具有多个空格分隔的值、其中一个值等于"val"的E元素
12|E[att\|=val]|匹配所有att属性具有多个连字号分隔（hyphen-separated）的值、其中一个值以"val"开头的E元素，主要用于lang属性，比如"en"、"en-us"、"en-gb"等等

**实例：**
```css
p[title] { color:#f00; }

div[class=error] { color:#f00; }

td[headers~=col1] { color:#f00; }

p[lang|=en] { color:#f00; }

blockquote[class=quote][cite] { color:#f00; }
```

#### 1.2.1.4. CSS 2.1中的伪类
序号|选择器|含义
-|:-:|-
13|E:first-child|匹配父元素的第一个子元素
14|E:link|匹配所有未被点击的链接
15|E:visited|匹配所有已被点击的链接
16|E:active|匹配鼠标已经其上按下、还没有释放的E元素
17|E:hover|匹配鼠标悬停其上的E元素
18|E:focus|匹配获得当前焦点的E元素
19|E:lang(c)|匹配lang属性等于c的E元素

**实例：**
```css
p:first-child { font-style:italic; }

input[type=text]:focus { color:#000; background:#ffe; }

input[type=text]:focus:hover { background:#fff; }

q:lang(sv) { quotes: "\201D" "\201D" "\2019" "\2019"; }
```

#### 1.2.1.5. CSS 2.1中的伪元素

序号|选择器|含义
-|:-:|-
20|E:first-line|匹配E元素的第一行
21|E:first-letter|匹配E元素的第一个字母
22|E:before|在E元素之前插入生成的内容
23|E:after|在E元素之后插入生成的内容

**实例：**
```css
p:first-line { font-weight:bold; color;#600; }

.preamble:first-letter { font-size:1.5em; font-weight:bold; }

.cbb:before { content:""; display:block; height:17px; width:18px; background:url(top.png) no-repeat 0 0; margin:0 0 0 -18px; }

a:link:after { content: " (" attr(href) ") "; }
```

#### 1.2.1.6. CSS 3的同级元素通用选择器
序号|选择器|含义
-|:-:|-
24|E ~ F|匹配任何在E元素之后的同级F元素

**实例：**
```css
p ~ ul { background:#ff0; }
```

#### 1.2.1.7. CSS 3 属性选择器
序号|选择器|含义
-|:-:|-
25|E[att^="val"]|属性att的值以"val"开头的元素
26|E[att$="val"]|属性att的值以"val"结尾的元素
27|E[att*="val"]|属性att的值包含"val"字符串的元素

**实例：**
```css
div[id^="nav"] { background:#ff0; }
```
#### 1.2.1.8. CSS 3中与用户界面有关的伪类

序号 |选择器|含义
-|:-:|-
28|E:enabled|匹配表单中激活的元素
29|E:disabled|匹配表单中禁用的元素
30|E:checked|匹配表单中被选中的radio（单选框）或checkbox（复选框）元素
31|E::selection|匹配用户当前选中的元素

**实例：**
```css
input[type="text"]:disabled { background:#ddd; }
```

#### 1.2.1.9. CSS 3中的结构性伪类
序号 |选择器|含义
-|:-:|-
32|E:root|匹配文档的根元素，对于HTML文档，就是HTML元素
33|E:nth-child(n)|匹配其父元素的第n个子元素，第一个编号为1
34|E:nth\-last\-child\(n\)|匹配其父元素的倒数第n个子元素，第一个编号为1
35|E:nth-of-type(n)|与:nth-child()作用类似，但是仅匹配使用同种标签的元素
36|E:nth-last-of-type(n)|与:nth-last-child() 作用类似，但是仅匹配使用同种标签的元素
37|E:last-child|匹配父元素的最后一个子元素，等同于:nth-last-child(1)
38|E:first-of-type|匹配父元素下使用同种标签的第一个子元素，等同于:nth-of-type(1)
39|E:last-of-type|匹配父元素下使用同种标签的最后一个子元素，等同于:nth-last-of-type(1)
40|E:only-child|匹配父元素下仅有的一个子元素，等同于:first-child:last-child或 :nth-child(1):nth-last-child(1)
41|E:only-of-type|匹配父元素下使用同种标签的唯一一个子元素，等同于:first-of-type:last-of-type或 :nth-of-type(1):nth-last-of-type(1)
42|E:empty|匹配一个不包含任何子元素的元素，注意，文本节点也被看作子元素

**实例：**
```css
p:nth-child(3) { color:#f00; }

p:nth-child(odd) { color:#f00; }

p:nth-child(even) { color:#f00; }

p:nth-child(3n+0) { color:#f00; }

p:nth-child(3n) { color:#f00; }

tr:nth-child(2n+11) { background:#ff0; }

tr:nth-last-child(2) { background:#ff0; }

p:last-child { background:#ff0; }

p:only-child { background:#ff0; }

p:empty { background:#ff0; }
```

#### 1.2.1.10. CSS 3的反选伪类

序号 |选择器|含义
-|:-:|-
43|E:not(s)|匹配不符合当前选择器的任何元素

**实例：**
```css
:not(p) { border:1px solid #ccc; }
```

#### 1.2.1.11. CSS 3中的 :target 伪类

序号 |选择器|含义
-|:-:|-
44|E:target|匹配文档中特定"id"点击后的效果

### 1.2.2. display: none;与visibility: hidden;的区别

1. display:none;会让元素完全从渲染树中消失，渲染的时候不占据任何空间；visibility: hidden;不会让元素从渲染树消失，渲染师元素继续占据空间，只是内容不可见
2. display: none;是非继承属性，子孙节点消失由于元素从渲染树消失造成，通过修改子孙节点属性无法显示；visibility: hidden;是继承属性，子孙节点消失由于继承了hidden，通过设置visibility: visible;可以让子孙节点显式
3. 修改常规流中元素的display通常会造成文档重排。修改visibility属性只会造成本元素的重绘。
4. 读屏器不会读取display: none;元素内容；会读取visibility: hidden;元素内容

### 1.2.3. css sprite是什么,有什么优缺点
定义：将多个小图片拼接到一个图片中。通过background-position和元素尺寸调节需要显示的背景图案。
- 优点：
    1. 减少HTTP请求数，极大地提高页面加载速度
    2. 增加图片信息重复度，提高压缩比，减少图片大小
    3. 更换风格方便，只需在一张或几张图片上修改颜色或样式即可实现
- 缺点：
    1. 图片合并麻烦
    2. 维护麻烦，修改一个图片可能需要从新布局整个图片，样式

### 1.2.4. CSS盒模型有那几种？

 - 一个盒子中主要的属性就5个：width、height、padding、border、margin。如下：
    - width和height：内容的宽度、高度（不是盒子的宽度、高度）。
    - padding：内边距。
    - border：边框。
    - margin：外边距。
- 标准盒模型
![标准盒模型](images/box-model.jpg)
- IE盒模型
![标准盒模型](images/box-model-ie.jpg)

### 1.2.5. CSS有哪些继承属性

- 关于文字排版的属性如
    - [font](https://developer.mozilla.org/zh-CN/docs/Web/CSS/font)
    - [word-break](https://developer.mozilla.org/zh-CN/docs/Web/CSS/word-break)
    - [letter-spacing](https://developer.mozilla.org/zh-CN/docs/Web/CSS/letter-spacing)
    - [text-align](https://developer.mozilla.org/zh-CN/docs/Web/CSS/text-align)
    - [text-rendering](https://developer.mozilla.org/zh-CN/docs/Web/CSS/text-rendering)
    - [word-spacing](https://developer.mozilla.org/zh-CN/docs/Web/CSS/word-spacing)
    - [white-space](https://developer.mozilla.org/zh-CN/docs/Web/CSS/white-space)
    - [text-indent](https://developer.mozilla.org/zh-CN/docs/Web/CSS/text-indent)
    - [text-transform](https://developer.mozilla.org/zh-CN/docs/Web/CSS/text-transform)
    - [text-shadow](https://developer.mozilla.org/zh-CN/docs/Web/CSS/text-shadow)
- line-height
- color
- visibility
- cursor

### 1.2.6. png、jpg、gif 这些图片格式解释一下，分别什么时候用。有没有了解过webp？

- png是便携式网络图片（Portable Network Graphics）是一种无损数据压缩位图文件格式.优点是：压缩比高，色彩好。 大多数地方都可以用
- jpg是一种针对相片使用的一种失真压缩方法，是一种破坏性的压缩，在色调及颜色平滑变化做的不错。在www上，被用来储存和传输照片的格式。
- gif是一种位图文件格式，以8位色重现真色彩的图像。可以实现动画效果.
- webp格式是谷歌在2010年推出的图片格式，压缩率只有jpg的2/3，大小比png小了45%。缺点是压缩的时间更久了，兼容性不好，目前谷歌和opera支持。

### 1.2.7. float、position 和 display 之间的关系
1. 如果display的值为none，那么后两者就不会产生作用，也不会有任何的盒子产生；
2. 除此之外，如果元素为absolute或者fixed定位，那么float的属性值相当于‘none’，display的属性如下面的表格所示。 
盒的位置根据“top”，“right”，“bottom”和“left”属性与盒的包含块决定。
3. 除此之外，如果float属性的值为不是none，那么元素将会浮动，元素的display属性将如下表所示；
4. 除此之外，如果元素是根元素，那么元素的属性如下表所示；
5. 除此之外，元素的display属性则根据设定来取值。
![postion](images/float-postion-display.png)

指定值|计算值
-|:-:|-
Inline-table|Table
inline,table-row-group,table-column, table-column-group,table-header-group,table-footer-group,table-row,table-cell,table-caption,inline-block|block
other|Same as specified

### 1.2.8. 超链接访问过后hover样式就不出现的问题？
-  被点击访问过的超链接样式不再具有hover和active了.
- 解决方式是改变CSS属性的排列顺序：L-V-H-A（linked, visited, hover, active）。

### 1.2.9. box-sizing属性？
 - 用来控制元素的盒子模型的解析模式，默认为content-box
 - context-box：W3C的标准盒子模型，设置元素的 height/width 属性指的是content部分的高/宽
 - border-box：IE传统盒子模型。设置元素的height/width属性指的是border + padding + content部分的高/宽

### 1.2.10. CSS优先级算法如何计算？
- 元素选择符： 1 (如p）或伪元素选择符(如 :firstchild)等，
- class选择符： 10
- id选择符：100
- 元素标签：1000（Style属性）
> 然后，将这四个数字分别累加，就得到每个CSS定义的优先级的值， 
然后从左到右逐位比较大小，数字大的CSS样式的优先级就高。

**注意：**
1. !important声明的样式优先级最高，如果冲突再进行计算。 
2. 如果优先级相同，则选择最后出现的样式。
3. 继承得到的样式的优先级最低。

### 1.2.11. CSS3有哪些新特性？

1. RGBA和透明度
2. background-image,background-origin(content-box/padding-box/border-box),background-size ,background-repeat
3. word-wrap（对长的不可分割单词换行）word-wrap：break-word
4. 文字阴影：text-shadow： 5px 5px 5px #FF0000;（水平阴影，垂直阴影，模糊距离，阴影颜色）
5. font-face属性：定义自己的字体
6. 圆角（边框半径）：border-radius 属性用于创建圆角
7. 边框图片：border-image: url(border.png) 30 30 round
8. 盒阴影：box-shadow: 10px 10px 5px #888888
9. 媒体查询：定义两套css，当浏览器的尺寸变化时会采用不同的属性

### 1.2.12. 请解释一下CSS3的flexbox（弹性盒布局模型）,以及适用场景？
 - 该布局模型的目的是提供一种更加高效的方式来对容器中的条目进行布局、对齐和分配空间。在传统的布局方式中，block 布局是把块在垂直方向从上到下依次排列的；
 - 而 inline 布局则是在水平方向来排列。弹性盒布局并没有这样内在的方向限制，可以由开发人员自由操作。
 - 试用场景：弹性布局适合于移动前端开发，在Android和ios上也完美支持。

### 1.2.13. 为什么要初始化CSS样式
 - 因为浏览器的兼容问题，不同浏览器对有些标签的默认值是不同的，如果没对CSS初始化往往会出现浏览器之间的页面显示差异

### 1.2.14. 对BFC规范(块级格式化上下文：block formatting context)的理解？
 > BFC规定了内部的Block Box如何布局。

 - 定位方案：
    1. 内部的Box会在垂直方向上一个接一个放置。
    2. Box垂直方向的距离由margin决定，属于同一个BFC的两个相邻Box的margin会发生重叠。
    3. 每个元素的margin box 的左边，与包含块border box的左边相接触。
    4. BFC的区域不会与float box重叠。
    5. BFC是页面上的一个隔离的独立容器，容器里面的子元素不会影响到外面的元素。
    6. 计算BFC的高度时，浮动元素也会参与计算。
- 满足下列条件之一就可触发BFC:
    1. 根元素，即html
    2. float的值不为none（默认）
    3. overflow的值不为visible（默认）
    4. display的值为inline-block、table-cell、table-caption
    5. position的值为absolute或fixed

### 1.2.15. 为什么会出现浮动和什么时候需要清除浮动？清除浮动的方式？
> 浮动元素碰到包含它的边框或者浮动元素的边框停留。由于浮动元素不在文档流中，所以文档流的块框表现得就像浮动框不存在一样。

- 浮动带来的问题：
    1. 父元素的高度无法被撑开，影响与父元素同级的元素
    2. 与浮动元素同级的非浮动元素（内联元素）会跟随其后
    3. 若非第一个元素浮动，则该元素之前的元素也需要浮动，否则会影响页面显示的结构。

- 清除浮动的方式：
    1. 父级div定义height
    2. 最后一个浮动元素后加空div标签 并添加样式clear:both。
    3. 包含浮动元素的父标签添加样式overflow为hidden或auto。
    4. 父级div定义zoom

### 1.2.16. 上下margin重合的问题
- 在重合元素外包裹一层容器，并触发该容器生成一个BFC。

### 1.2.17. 移动端的布局用过媒体查询吗？
> 通过媒体查询可以为不同大小和尺寸的媒体定义不同的css，适应相应的设备的显示。

### 1.2.18. CSS优化、提高性能的方法有哪些？
1. 避免过度约束
2. 避免后代选择符
3. 避免链式选择符
4. 使用紧凑的语法
5. 避免不必要的命名空间
6. 避免不必要的重复
7. 最好使用表示语义的名字。一个好的类名应该是描述他是什么而不是像什么
8. 避免！important，可以选择其他选择器
9. 尽可能的精简规则，你可以合并不同类里的重复规则

### 1.2.19. 浏览器是怎样解析CSS选择器的？
- CSS选择器的解析是从右向左解析的。若从左向右的匹配，发现不符合规则，需要进行回溯，会损失很多性能。
- 若从右向左匹配，先找到所有的最右节点，对于每一个节点，向上寻找其父节点直到找到根元素或满足条件的匹配规则，则结束这个分支的遍历。
- 两种匹配规则的性能差别很大，是因为从右向左的匹配在第一步就筛选掉了大量的不符合条件的最右节点（叶子节点），而从左向右的匹配规则的性能都浪费在了失败的查找上面。
- 而在 CSS 解析完毕后，需要将解析的结果与 DOM Tree 的内容一起进行分析建立一棵 Render Tree，最终用来进行绘图。
- 在建立 Render Tree 时（WebKit 中的「Attachment」过程），浏览器就要为每个 DOM Tree 中的元素根据 CSS 的解析结果（Style Rules）来确定生成怎样的 Render Tree。

### 1.2.20. 在网页中的应该使用奇数还是偶数的字体？为什么呢？
- 使用偶数字体。偶数字号相对更容易和 web 设计的其他部分构成比例关系。Windows 自带的点阵宋体（中易宋体）从 Vista 开始只提供 12、14、16 px 这三个大小的点阵，而 13、15、17 px时用的是小一号的点。（即每个字占的空间大了 1 px，但点阵没变），于是略显稀疏。

### 1.2.21. margin和padding分别适合什么场景使用？
- 何时使用margin：
    1. 需要在border外侧添加空白
    2. 空白处不需要背景色
    3. 上下相连的两个盒子之间的空白，需要相互抵消时。
- 何时使用padding：
    1. 需要在border内侧添加空白
    2. 空白处需要背景颜色
    3. 上下相连的两个盒子的空白，希望为两者之和。
>兼容性的问题：在IE5 IE6中，为float的盒子指定margin时，左侧的margin可能会变成两倍的宽度。通过改变padding或者指定盒子的display：inline解决。

### 1.2.22. 元素竖向的百分比设定是相对于容器的高度吗？
- 当按百分比设定一个元素的宽度时，它是相对于父容器的宽度计算的，但是，对于一些表示竖向距离的属性，例如 padding-top , padding-bottom , margin-top , margin-bottom 等，当按百分比设定它们时，依据的也是父容器的宽度，而不是高度。

### 1.2.23. 如果需要手动写动画，你认为最小时间间隔是多久，为什么？
- 多数显示器默认频率是60Hz，即1秒刷新60次，所以理论上最小间隔为1/60＊1000ms ＝ 16.7ms。

### 1.2.24. style标签写在body后与body前有什么区别？
- 页面加载自上而下 当然是先加载样式。
- 写在body标签后由于浏览器以逐行方式对HTML文档进行解析，当解析到写在尾部的样式表（外联或写在style标签）会导致浏览器停止之前的渲染，等待加载且解析样式表完成之后重新渲染，在windows的IE下可能会出现FOUC现象（即样式失效导致的页面闪烁问题）