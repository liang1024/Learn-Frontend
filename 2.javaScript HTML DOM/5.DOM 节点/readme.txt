

添加和删除节点

目录：
1.创建并添加新的 HTML 元素
2.删除已有的 HTML 元素
3.HTML DOM 教程更多


1.创建并添加新的 HTML 元素
如需向 HTML DOM 添加新元素，您必须首先创建该元素（元素节点），然后向一个已存在的元素追加该元素。
        <div id="div1">
        <p id="p1">这是一个段落</p>
        <p id="p2">这是另一个段落</p>
        </div>

        <script>
        var para=document.createElement("p");
        var node=document.createTextNode("这是新段落。");
        para.appendChild(node);

        var element=document.getElementById("div1");
        element.appendChild(para);
        </script>
参考：demo1.html

例子解释：

这段代码创建新的 <p> 元素：
var para=document.createElement("p");

如需向 <p> 元素添加文本，您必须首先创建文本节点。这段代码创建了一个文本节点：
var node=document.createTextNode("这是新段落。");

然后您必须向 <p> 元素追加这个文本节点：
para.appendChild(node);

最后您必须向一个已有的元素追加这个新元素。
这段代码找到一个已有的元素：
var element=document.getElementById("div1");

这段代码向这个已有的元素追加新元素：
element.appendChild(para);



2.删除已有的 HTML 元素

如需删除 HTML 元素，您必须首先获得该元素的父元素：
        <div id="div1">
        <p id="p1">这是一个段落。</p>
        <p id="p2">这是另一个段落。</p>
        </div>

        <script>
        var parent=document.getElementById("div1");
        var child=document.getElementById("p1");
        parent.removeChild(child);
        </script>
参考：demo2.html

例子解释：
这个 HTML 文档含有拥有两个子节点（两个 <p> 元素）的 <div> 元素：

    <div id="div1">
    <p id="p1">这是一个段落。</p>
    <p id="p2">这是另一个段落。</p>
    </div>

找到 id="div1" 的元素：
var parent=document.getElementById("div1");

找到 id="p1" 的 <p> 元素：
var child=document.getElementById("p1");

从父元素中删除子元素：
parent.removeChild(child);

提示：如果能够在不引用父元素的情况下删除某个元素，就太好了。
不过很遗憾。DOM 需要清楚您需要删除的元素，以及它的父元素。
这是常用的解决方案：找到您希望删除的子元素，然后使用其 parentNode 属性来找到父元素：
    var child=document.getElementById("p1");
    child.parentNode.removeChild(child);


3.HTML DOM 教程更多

在我们的 JavaScript 教程的 HTML DOM 部分，您已经学到了：
如何改变 HTML 元素的内容 (innerHTML)
如何改变 HTML 元素的样式 (CSS)
如何对 HTML DOM 事件作出反应
如何添加或删除 HTML 元素
如果您希望学到更多有关使用 JavaScript 访问 HTML DOM 的知识，请访问我们完整的 HTML DOM 教程。

http://www.w3school.com.cn/htmldom/index.asp