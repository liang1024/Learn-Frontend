
目录：
1.javaScript循环简介
2.For循环
3.for/In循环


循环可以将代码块执行指定的次数。


1.javaScript循环简介

如果你希望一遍又一遍的运行相同的代码，并且每次的值都不同，那么使用循环是很方便的，我们可以这样输出数组的值：

document.write(cars[0] + "<br>");
document.write(cars[1] + "<br>");
document.write(cars[2] + "<br>");
document.write(cars[3] + "<br>");
document.write(cars[4] + "<br>");
document.write(cars[5] + "<br>");

不过通常我们这样写：

for (var i=0;i<cars.length;i++)
{
document.write(cars[i] + "<br>");
}

参考：demo1.html

不同类型的循环
    JavaScript 支持不同类型的循环：
    for - 循环代码块一定的次数
    for/in - 循环遍历对象的属性
    while - 当指定的条件为 true 时循环指定的代码块
    do/while - 同样当指定的条件为 true 时循环指定的代码块


2.For循环

for 循环是您在希望创建循环时常会用到的工具。

下面是 for 循环的语法：

for (语句 1; 语句 2; 语句 3)
  {
  被执行的代码块
  }

语句 1 在循环（代码块）开始前执行
语句 2 定义运行循环（代码块）的条件
语句 3 在循环（代码块）已被执行之后执行

for (var i=0; i<5; i++)
  {
  x=x + "The number is " + i + "<br>";
  }

参考：demo2.html


写法2：

for (var i=0,len=cars.length; i<len; i++)
{
document.write(cars[i] + "<br>");
}

写法3：

var i=2,len=cars.length;
for (; i<len; i++)
{
document.write(cars[i] + "<br>");
}

写法4：

var i=0,len=cars.length;
for (; i<len; )
{
document.write(cars[i] + "<br>");
i++;
}

3.For/In 循环

JavaScript for/in 语句循环遍历对象的属性：

var person={fname:"John",lname:"Doe",age:25};

for (x in person)
  {
  txt=txt + person[x];
  }

参考：demo3.html




