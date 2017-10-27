

目录：
1.改变HTML输出流
2.改变HTML内容
3.改变HTML属性

HTML DOM 允许 JavaScript 改变 HTML 元素的内容。

1.改变HTML输出流

JavaScript 能够创建动态的 HTML 内容：
今天的日期是： Fri Oct 27 2017 10:25:58 GMT+0800 (中国标准时间)
在 JavaScript 中，document.write() 可用于直接向 HTML 输出流写内容。

<!DOCTYPE html>
<html>
<body>

<script>
document.write(Date());
</script>

</body>
</html>

参考：demo1.html

提示：绝不要使用在文档加载之后使用 document.write()。这会覆盖该文档。


2.改变HTML内容

修改 HTML 内容的最简单的方法时使用 innerHTML 属性。
如需改变 HTML 元素的内容，请使用这个语法：

document.getElementById(id).innerHTML=new HTML

实例1：

本例改变了 <p> 元素的内容：

        <html>
        <body>

        <p id="p1">Hello World!</p>

        <script>
        document.getElementById("p1").innerHTML="New text!";
        </script>

        </body>
        </html>

参考：demo2.html

实例2：

本例改变了 <h1> 元素的内容：

    <!DOCTYPE html>
    <html>
    <body>

    <h1 id="header">Old Header</h1>

    <script>
    var element=document.getElementById("header");
    element.innerHTML="New Header";
    </script>

    </body>
    </html>

参考：demo3.html

例子解释：
上面的 HTML 文档含有 id="header" 的 <h1> 元素
我们使用 HTML DOM 来获得 id="header" 的元素
JavaScript 更改此元素的内容 (innerHTML)



3.改变HTML属性

如需改变 HTML 元素的属性，请使用这个语法：

document.getElementById(id).attribute=new value

本例改变了 <img> 元素的 src 属性：

        <!DOCTYPE html>
        <html>
        <body>

        <img id="image" src="smiley.gif">

        <script>
        document.getElementById("image").src="landscape.jpg";
        </script>

        </body>
        </html>

参考：demo4.html

例子解释：
上面的 HTML 文档含有 id="image" 的 <img> 元素
我们使用 HTML DOM 来获得 id="image" 的元素
JavaScript 更改此元素的属性（把 "smiley.gif" 改为 "landscape.jpg"）









