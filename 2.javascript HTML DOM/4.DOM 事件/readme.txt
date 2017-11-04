

目录：
1.javaScript对事件做出反应
2.例子1
3.例子2
4.HTML事件属性
5.使用HTML DOM来分配事件
6.onLoad和onUnLoad事件(检测浏览器是否开启cookie)
7.onchange事件
8.onmouseover和onmouseout事件
9.onmousedown，onmouseup以及onclick事件
10.例子3(按下鼠标换图)
11.例子4(页面加载完时，显示提示框)
12.例子5(当输入字段获得焦点时，改变其背景色。)
13.例子6(鼠标移动改变字体颜色)
14.HTML DOM Event 更多方法


HTML DOM 使 JavaScript 有能力对 HTML 事件做出反应。


1.javaScript对事件做出反应

我们可以在事件发生时执行 JavaScript，比如当用户在 HTML 元素上点击时。
如需在用户点击某个元素时执行代码，请向一个 HTML 事件属性添加 JavaScript 代码：

onclick=JavaScript

HTML 事件的例子：
    当用户点击鼠标时
    当网页已加载时
    当图像已加载时
    当鼠标移动到元素上时
    当输入字段被改变时
    当提交 HTML 表单时
    当用户触发按键时

2.例子1：
在本例中，当用户在 <h1> 元素上点击时，会改变其内容：
<h1 onclick="this.innerHTML='谢谢!'">请点击该文本</h1>

参考：demo1.html

3.例子2：
本例从事件处理器调用一个函数：
        <!DOCTYPE html>
        <html>
        <head>
        <script>
        function changetext(id)
        {
        id.innerHTML="谢谢!";
        }
        </script>
        </head>
        <body>
        <h1 onclick="changetext(this)">请点击该文本</h1>
        </body>
        </html>

参考：demo2.html

4.HTML事件属性
如需向 HTML 元素分配 事件，您可以使用事件属性。

向 button 元素分配 onclick 事件：

<button onclick="displayDate()">点击这里</button>

参考：demo3.html

在上面的例子中，名为 displayDate 的函数将在按钮被点击时执行。



5.使用HTML DOM来分配事件

HTML DOM 允许您通过使用 JavaScript 来向 HTML 元素分配事件：
向 button 元素分配 onclick 事件：

<script>
document.getElementById("myBtn").onclick=function(){displayDate()};
</script>

参考：demo4.html

在上面的例子中，名为 displayDate 的函数被分配给 id=myButn" 的 HTML 元素。
当按钮被点击时，会执行该函数。


6.onLoad和onUnLoad事件(检测浏览器是否开启cookie)

onload 和 onunload 事件会在用户进入或离开页面时被触发。
onload 事件可用于检测访问者的浏览器类型和浏览器版本，并基于这些信息来加载网页的正确版本。
onload 和 onunload 事件可用于处理 cookie。

<body onload="checkCookies()">

参考：demo5.html


7.onchange事件
onchange 事件常结合对输入字段的验证来使用。
下面是一个如何使用 onchange 的例子。当用户改变输入字段的内容时，会调用 upperCase() 函数。

<input type="text" id="fname" onchange="upperCase()">

参考demo6.html


8.onmouseover和onmouseout事件
onmouseover 和 onmouseout 事件可用于在用户的鼠标移至 HTML 元素上方或移出元素时触发函数。
实例
一个简单的 onmouseover-onmouseout 实例：
参考：demo7.html


9.onmousedown，onmouseup以及onclick事件
nmousedown, onmouseup 以及 onclick 构成了鼠标点击事件的所有部分。
首先当点击鼠标按钮时，会触发 onmousedown 事件，当释放鼠标按钮时，
会触发 onmouseup 事件，最后，当完成鼠标点击时，会触发 onclick 事件。
参考：demo8.html


10.例子3(按下鼠标换图)
参考：demo9.html


11.例子4(页面加载完时，显示提示框)
参考：demo10.html


12.例子5(当输入字段获得焦点时，改变其背景色。)
参考：demo11.html


13.例子6(鼠标移动改变字体颜色)
参考：demo12.html

14.HTML DOM Event 更多方法
http://www.w3school.com.cn/jsref/dom_obj_event.asp

