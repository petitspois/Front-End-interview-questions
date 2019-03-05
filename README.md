# Front-End-interview-questions
分享请标记出处: [https://github.com/petitspois/Front-End-interview-questions](https://github.com/petitspois/Front-End-interview-questions)


<!-- TOC -->

- [Front-End-interview-questions](#front-end-interview-questions)
    - [HTML](#html)
        - [DOCTYPE相关](#doctype相关)
        - [web语义化](#web语义化)
        - [前端SEO](#前端seo)
        - [什么是HTML](#什么是html)
        - [XHTML和HTML有什么区别](#xhtml和html有什么区别)
        - [浏览器页面有哪三层构成，分别是什么，作用是什么](#浏览器页面有哪三层构成分别是什么作用是什么)
        - [行内元素、块级元素、空(void)元素，有那些](#行内元素块级元素空void元素有那些)
        - [iframe有那些缺点](#iframe有那些缺点)
        - [Label的作用是什么？](#label的作用是什么)
        - [隐藏元素的几种方法](#隐藏元素的几种方法)
        - [简述一下src与href的区别](#简述一下src与href的区别)
        - [清除浮动的方法有哪些](#清除浮动的方法有哪些)
        - [HTTP方法](#http方法)
        - [HTTP报文结构](#http报文结构)
        - [HTML全局属性global-attribute有哪些](#html全局属性global-attribute有哪些)
        - [何为渐进增强、优雅降级](#何为渐进增强优雅降级)
        - [\<img>的title和alt有什么区别](#\img的title和alt有什么区别)
        - [从浏览器地址栏输入url到显示页面的步骤(以HTTP为例)](#从浏览器地址栏输入url到显示页面的步骤以http为例)
        - [HTML5新增元素、标签](#html5新增元素标签)
            - [form相关](#form相关)
            - [增强的页面元素](#增强的页面元素)
    - [CSS部分](#css部分)
        - [CSS选择器有哪些](#css选择器有哪些)
            - [基本选择器](#基本选择器)
            - [多元素的组合选择器](#多元素的组合选择器)
            - [CSS 2.1 属性选择器](#css-21-属性选择器)
            - [CSS 2.1中的伪类](#css-21中的伪类)
            - [CSS 2.1中的伪元素](#css-21中的伪元素)
            - [CSS 3的同级元素通用选择器](#css-3的同级元素通用选择器)
            - [CSS 3 属性选择器](#css-3-属性选择器)
            - [CSS 3中与用户界面有关的伪类](#css-3中与用户界面有关的伪类)
            - [CSS 3中的结构性伪类](#css-3中的结构性伪类)
            - [CSS 3的反选伪类](#css-3的反选伪类)
            - [CSS 3中的 :target 伪类](#css-3中的-target-伪类)

<!-- /TOC -->


## HTML
### DOCTYPE相关

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

### web语义化

- Web语义化是指使用恰当语义的html标签、class类名等内容，让页面具有良好的结构与含义，从而让人和机器都能快速理解网页内容。语义化的web页面一方面可以让机器在更少的人类干预情况下收集并研究网页的信息，从而可以读懂网页的内容，然后将收集汇总的信息进行分析，结果为人类所用；另一方面它可以让开发人员读懂结构和用户以及屏幕阅读器（如果访客有视障）能够读懂内容。
简单来说就是利于 SEO，便于阅读维护理解。
- 总结起来就是：
1. 正确的标签做正确的事情
2. 页面内容结构化
3. 无CSS样子时也容易阅读，便于阅读维护和理解
4. 便于浏览器、搜索引擎解析。 利于爬虫标记、利于SEO

- [拓展阅读](https://github.com/heweixiao/blog/issues/1)

### 前端SEO
 1. 合理的title、description、keywords：搜索对着三项的权重逐个减小，title值强调重点即可，重要关键词出现不要超过2次，而且要靠前，不同页面title要有所不同；description把页面内容高度概括，长度合适，不可过分堆砌关键词，不同页面description有所不同；keywords列举出重要关键词即可
 2. 语义化的HTML代码，符合W3C规范：语义化代码让搜索引擎容易理解网页
 3. 重要内容HTML代码放在最前：搜索引擎抓取HTML顺序是从上到下，有的搜索引擎对抓取长度有限制，保证重要内容一定会被抓取
 4. 重要内容不要用js输出：爬虫不会执行js获取内容
 5. 少用iframe：搜索引擎不会抓取iframe中的内容
 6. 非装饰性图片必须加alt
 7. 提高网站速度：网站速度是搜索引擎排序的一个重要指标
 
 ### 前端性能优化有哪些
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

 ### web开发中会话跟踪的方法有哪些
 1. cookie
 2. session
 3. url重写
 4. 隐藏input
 5. ip地址
### 什么是HTML
 - HTML：HyperText Markup Language超文本标记语言
### XHTML和HTML有什么区别
 - HTML是一种基本的WEB网页设计语言，XHTML是一个基于XML的标记语言
### 浏览器页面有哪三层构成，分别是什么，作用是什么
 - 浏览器页面构成：结构层、表示层、行为层
 - 分别是：HTML、CSS、JavaScript
 - 作用：HTML实现页面结构，CSS完成页面的表现与风格，JavaScript实现一些客户端的功能与业务。
 ### 页面导入样式时，使用link和@import有什么区别
 1. 作用不同：link属于XHTML标签，除了加载CSS外，还能用于定义RSS, 定义rel连接属性等作用；而@import是CSS提供的，只能用于加载CSS;
 2. 加载不同：页面被加载的时，link会同时被加载，而@import引用的CSS会等到页面被加载完再加载;
 3. 兼容不同：import是CSS2.1 提出的，只在IE5以上才能被识别，而link是XHTML标签，无兼容问题;
 ### 网页制作会用到的图片格式有哪些
 1. Webp：WebP格式，谷歌（google）开发的一种旨在加快图片加载速度的图片格式。并能节省大量的服务器带宽资源和数据空间。Facebook Ebay等知名网站已经开始测试并使用WebP格式。
 2. Apng：是PNG的位图动画扩展，可以实现png格式的动态图片效果，有望代替GIF成为下一代动态图标准。
 ### 文本标记
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

### 行内元素、块级元素、空(void)元素，有那些
1. 行内元素有：a b span img input select
2. 块级元素有: div p ul ol li dl dt dd h1-h6
3. 常见的空元素: br-换行，hr-水平分割线

### iframe有那些缺点
1. iframe会阻塞主页面的Onload事件，会影响页面的并行加载；
2. 搜索引擎的检索程序无法解读这种页面，不利于SEO;
- 通过javascript动态给iframe添加src属性值，这样可以绕开以上两个问题

### Label的作用是什么？
- label标签来定义表单控制间的关系,当用户选择该标签时，浏览器会自动将焦点转到和标签相关的表单控件上。
### 隐藏元素的几种方法
1. display:none;
2. visibility:hidden;
3. opacity:0;
4. position:absolute; left:-10000px;
### 简述一下src与href的区别
- src用于替换当前元素，href用于在当前文档和引用资源之间确立联系。
### 清除浮动的方法有哪些
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
### HTTP方法
1. **GET**是最常用的方法，通常用于请求服务器发送某个资源。
2. **HEAD**与GET类似，但服务器在响应中只返回首部，不返回实体的主体部分
3. **PUT**让服务器用请求的主体部分来创建一个由所请求的URL命名的新文档，或者，如果那个URL已经存在的话，就用这个主体替代它
4. **POST**起初是用来向服务器输入数据的。实际上，通常会用它来支持HTML的表单。表单中填好的数据通常会被送给服务器，然后由服务器将其发送到要去的地方。
5. **TRACE**会在目的服务器端发起一个环回诊断，最后一站的服务器会弹回一个TRACE响应并在响应主体中携带它收到的原始请求报文。TRACE方法主要用于诊断，用于验证请求是否如愿穿过了请求/响应链。
6. **OPTIONS**方法请求web服务器告知其支持的各种功能。可以查询服务器支持哪些方法或者对某些特殊资源支持哪些方法。
7. **DELETE**请求服务器删除请求URL指定的资源

### HTTP报文结构
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

### HTML全局属性global-attribute有哪些

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

### 何为渐进增强、优雅降级

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

### \<img>的title和alt有什么区别

1. title是global attributes之一，用于为元素提供附加的advisory information。通常当鼠标滑动到元素上的时候显示。
2. alt是\<img>的特有属性，是图片内容的等价描述，用于图片无法加载时显示、读屏器阅读图片。可提图片高可访问性，除了纯装饰图片外都必须设置有意义的值，搜索引擎会重点分析。

### 从浏览器地址栏输入url到显示页面的步骤(以HTTP为例)
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

### HTML5新增元素、标签

#### form相关

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
#### 增强的页面元素
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

## CSS部分

### CSS选择器有哪些

#### 基本选择器
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

#### 多元素的组合选择器
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
#### CSS 2.1 属性选择器
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

#### CSS 2.1中的伪类
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

#### CSS 2.1中的伪元素

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

#### CSS 3的同级元素通用选择器
序号|选择器|含义
-|:-:|-
24|E ~ F|匹配任何在E元素之后的同级F元素

**实例：**
```css
p ~ ul { background:#ff0; }
```

#### CSS 3 属性选择器
序号|选择器|含义
-|:-:|-
25|E[att^="val"]|属性att的值以"val"开头的元素
26|E[att$="val"]|属性att的值以"val"结尾的元素
27|E[att*="val"]|属性att的值包含"val"字符串的元素

**实例：**
```css
div[id^="nav"] { background:#ff0; }
```
#### CSS 3中与用户界面有关的伪类

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

#### CSS 3中的结构性伪类
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

#### CSS 3的反选伪类

序号 |选择器|含义
-|:-:|-
43|E:not(s)|匹配不符合当前选择器的任何元素

**实例：**
```css
:not(p) { border:1px solid #ccc; }
```

#### CSS 3中的 :target 伪类

序号 |选择器|含义
-|:-:|-
44|E:target|匹配文档中特定"id"点击后的效果




