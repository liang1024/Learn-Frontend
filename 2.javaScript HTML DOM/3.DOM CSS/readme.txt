
目录：
1.改变HTML样式
2.例子1
3.例子2
4.设置元素是否显示
5.HTML DOM STYLE对象更多方法



HTML DOM 允许 JavaScript 改变 HTML 元素的样式。



1.改变HTML样式

如需改变HTML元素的样式，请使用这个语法

document.getElementById(id).style.property=new style


2.例子1

下面的例子会改变 <p> 元素的样式：

<p id="p2">Hello World!</p>

<script>
document.getElementById("p2").style.color="blue";
</script>

参考：demo1.html


3.例子2

本例改变了 id="id1" 的 HTML 元素的样式，当用户点击按钮时：

<h1 id="id1">My Heading 1</h1>

<button type="button" onclick="document.getElementById('id1').style.color='red'">
点击这里
</button>

参考：demo2.html




4.设置元素是否显示

参考：demo3.html




5.HTML DOM STYLE对象更多方法

http://www.w3school.com.cn/jsref/dom_obj_style.asp


