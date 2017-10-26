
目录：
1.操作 HTML 元素
2.写到文档输出
3.输出覆盖

JavaScript 通常用于操作 HTML 元素。

1.操作 HTML 元素

如需从 JavaScript 访问某个 HTML 元素，您可以使用 document.getElementById(id) 方法。
请使用 "id" 属性来标识 HTML 元素：

参考:  例子1.html
JavaScript 由 web 浏览器来执行。在这种情况下，浏览器将访问 id="demo" 的 HTML 元素，并把它的内容（innerHTML）替换为 "My First JavaScript"。


2.写到文档输出

下面的例子直接把 <p> 元素写到 HTML 文档输出中：

参考： 例子2.html


3.输出覆盖

请使用 document.write() 仅仅向文档输出写内容。
如果在文档已完成加载后执行 document.write，整个 HTML 页面将被覆盖：

参考：例子3.html