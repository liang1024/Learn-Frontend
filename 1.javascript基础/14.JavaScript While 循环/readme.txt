
目录：
1.while循环
2.do/while循环
3.比较for和while


1.while循环

while循环会在指定条件为真时循环执行代码块

while (条件)
  {
  需要执行的代码
  }


本例中的循环将继续运行，只要变量 i 小于 5：

while (i<5)
  {
  x=x + "The number is " + i + "<br>";
  i++;
  }

提示：如果您忘记增加条件中所用变量的值，该循环永远不会结束。该可能导致浏览器崩溃。



2.do/while循环

do/while 循环是 while 循环的变体。该循环会执行一次代码块，在检查条件是否为真之前，然后如果条件为真的话，就会重复这个循环。

do
  {
  需要执行的代码
  }
while (条件);

下面的例子使用 do/while 循环。该循环至少会执行一次，即使条件是 false，隐藏代码块会在条件被测试前执行：

do
  {
  x=x + "The number is " + i + "<br>";
  i++;
  }
while (i<5);

参考：demo2.html





3.比较for和while

如果您已经阅读了前面那一章关于 for 循环的内容，您会发现 while 循环与 for 循环很像。

for 语句实例

本例中的循环使用 for 循环来显示 cars 数组中的所有值：

cars=["BMW","Volvo","Saab","Ford"];
var i=0;
for (;cars[i];)
{
document.write(cars[i] + "<br>");
i++;
}

参考:  demo3.html




4.while 语句实例

本例中的循环使用使用 while 循环来显示 cars 数组中的所有值：

cars=["BMW","Volvo","Saab","Ford"];
var i=0;
while (cars[i])
{
document.write(cars[i] + "<br>");
i++;
}

参考：  demo4.html


