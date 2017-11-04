
目录:
1.HTML DOM （文档对象模型）
2.怎么查找HTML元素
3.通过id查HTML元素
4.通过标签名查找HTML元素

参考：
http://www.w3school.com.cn/js/js_htmldom.asp
通过 HTML DOM，可访问 JavaScript HTML 文档的所有元素。



1.HTML DOM （文档对象模型）

当网页被加载时，浏览器会创建页面的文档对象模型（Document Object Model）。
HTML DOM 模型被构造为对象的树。

HTML DOM 树

http://www.w3school.com.cn/i/ct_htmltree.gif

通过可编程的对象模型，JavaScript 获得了足够的能力来创建动态的 HTML。
JavaScript 能够改变页面中的所有 HTML 元素
JavaScript 能够改变页面中的所有 HTML 属性
JavaScript 能够改变页面中的所有 CSS 样式
JavaScript 能够对页面中的所有事件做出反应




2.怎么查找HTML元素

通常，通过 JavaScript，您需要操作 HTML 元素。
为了做到这件事情，您必须首先找到该元素。有三种方法来做这件事：
通过 id 找到 HTML 元素
通过标签名找到 HTML 元素
通过类名找到 HTML 元素



3.通过id查找HTML元素
在DOM中查找HTML元素的最简单的方法，是通过使用元素的id

本例查找 id ="intro"元素

var x=document.getElementById("intro");

参考：demo1.html

如果找到该元素，则该方法将以对象（在 x 中）的形式返回该元素。
如果未找到该元素，则 x 将包含 null。




4.通过标签名查找HTML元素

本例查找 id="main" 的元素，然后查找 "main" 中的所有 <p> 元素：

var x=document.getElementById("main");
var y=x.getElementsByTagName("p");

参考：demo2.html










