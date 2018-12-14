# learncss
- 本文为重新学习css的记录，参考资料[love丁酥酥的简书](https://www.jianshu.com/nb/19084159) 
- 本文只记录简单的点，方便自己进行知识的检索


## 1. [head标签能嵌套的标签](https://www.jianshu.com/p/5a9260ac2974)
- title, base, meta, style, link, script
### 1.1 meta标签 [meta深入](https://www.jianshu.com/p/c28b0e50cc0b)
- META标签是HTML标记HEAD区的一个关键标签，提供文档字符集、使用语言、作者等基本信息，以及对关键词和网页等级的设定等，最大的作用是能够做搜索引擎优化（SEO）
- 指明文件的编码属性<br>
`<meta charset="utf-8" /> `
- 把 content 属性关联到一个名称<br>
`<meta name="author" content="Your Name"/>  `
- 把 content 属性关联到 HTTP 头部<br>
`<meta http-equiv="Refresh" content="5;url=http://www.jianshu.com/u/7a62ab344c39" />`
5秒后会定义到指定页。
- scheme 属性设置或返回用于解释 content 属性的值的格式<br>
`<meta name="revised" content="2006-11-03" scheme="YYYY-MM-DD" />`


## 2. [认识html之元素](https://www.jianshu.com/p/04c6e922e2a2)
### 顶级元素
html, body, frameset
### 块级元素Block-level element
- 高度宽度可设置
- p, h1~h6, div, ul, table, ul, ol, li, hr水平分隔线, form, dl, blockquote
- 占一行
- 非块级转换 display:block
### 内联元素inline elelment
- 高度宽度不可设置
- a, span, input, img, button, select, br, textarea, q, b, big, i, em
- 转换 display:inline     float


## 3. [css引入](https://www.jianshu.com/p/b11dfc3438ab)
- 内联样式、内部样式（style）、外部链接样式（link）、外部导入（import）


## 4. [选择器](https://www.jianshu.com/p/65e0adc57ff7)
- "#id", "元素选择器", ".class", "属性选择器[ ]", "通配选择器*"
### 伪类选择器
- 顺序：link-visited-focus-hover-active
- 静态伪类：link, visited;只应用于超链接;只能设置字体颜色、边框颜色、outline颜色
- 动态伪类：focus, hover, active;用于所有元素
- 目标伪类:target;IE8-不支持
- UI元素伪类(IE8-不支持):enabled可用状态,disabled不可用状态,checked选中状态
- 结构伪类(IE8-不支持)
    - E:first-child(IE6-不支持) 父元素的第一个子元素,且该子元素是E，与E:nth-child(1)等同
    - E:last-child(IE6-不支持) 父元素的最后一个子元素，且该子元素是E，与E:nth-last-child(1)等同
    - :root 选择文档的根元素，即html元素
    - .....
### 伪元素选择器
- :first-letter, :first-line, :first-child, :before, :after, ::selection
### 亲戚关系
- 后代element element, 子代element>element, 兄弟element~element, 相邻兄弟element+element


## 5. [盒模型](https://www.jianshu.com/p/a2215e65a641)
### box-sizing属性
- 设定那种标准的盒模型
    - content-box
    默认值，表现形式同W3C标准和模型。（总宽度 = width + padding + border + margin）
    - border-box
    表现形式同IE盒模型，常用值，经常在css-reset中设置。（总宽度 = width + margin）
    - inherit
    规定应从父元素继承box-sizing属性的值。


## 6. [css三大特性](https://www.jianshu.com/p/6bb19b620af5)
- 继承性、层叠性、优先级
- [CSS中可以和不可以继承的属性](http://www.cnblogs.com/thislbq/p/5882105.html)
### [优先级](https://www.jianshu.com/p/0ea3fd082a2e)
- 仅内联：后来居上
- id > （类，属性，伪类）> 元素 > 通配符 > 浏览器默认样式 > 继承样式
- 伪元素其实是在元素内容内虚拟创建了一个元素，且无法被其他选择器选取。对于伪元素的样式，不用考虑优先级
- 社群关系、亲戚关系不会影响其本身的权重







