# Front-End-interview-questions
分享请标记出处: [https://github.com/petitspois/Front-End-interview-questions](https://github.com/petitspois/Front-End-interview-questions)

- [HTML部分](#HTML)
  - [DOCTYPE相关](#DOCTYPE相关)



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






