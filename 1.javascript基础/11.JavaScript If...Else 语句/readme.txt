
目录：
1.条件语句简介
2.if语句
3.if...else语句
4.if...else if...else 语句


条件语句用于基于不同的条件来执行不同的动作。


1.条件语句简介

通常在写代码时，您总是需要为不同的决定来执行不同的动作。您可以在代码中使用条件语句来完成该任务。
在 JavaScript 中，我们可使用以下条件语句：
        if 语句 - 只有当指定条件为 true 时，使用该语句来执行代码
        if...else 语句 - 当条件为 true 时执行代码，当条件为 false 时执行其他代码
        if...else if....else 语句 - 使用该语句来选择多个代码块之一来执行
        switch 语句 - 使用该语句来选择多个代码块之一来执行


2.If 语句

只有当指定条件为 true 时，该语句才会执行代码。

if (条件)
  {
  只有当条件为 true 时执行的代码
  }

注意：请使用小写的 if。使用大写字母（IF）会生成 JavaScript 错误！

当时间小于 20:00 时，生成一个“Good day”问候：

if (time<20)
  {
  x="Good day";
  }

x 的结果是：

Good day

参考：demo1.html

请注意，在这个语法中，没有 ..else..。您已经告诉浏览器只有在指定条件为 true 时才执行代码。





3.If...else 语句

请使用 if....else 语句在条件为 true 时执行代码，在条件为 false 时执行其他代码。

if (条件)
  {
  当条件为 true 时执行的代码
  }
else
  {
  当条件不为 true 时执行的代码
  }

当时间小于 20:00 时，将得到问候 "Good day"，否则将得到问候 "Good evening"。

if (time<20)
  {
  x="Good day";
  }
else
  {
  x="Good evening";
  }

x 的结果是：

Good day

参考：demo2.html



4.If...else if...else 语句

使用 if....else if...else 语句来选择多个代码块之一来执行。

if (条件 1)
  {
  当条件 1 为 true 时执行的代码
  }
else if (条件 2)
  {
  当条件 2 为 true 时执行的代码
  }
else
  {
  当条件 1 和 条件 2 都不为 true 时执行的代码
  }

如果时间小于 10:00，则将发送问候 "Good morning"，否则如果时间小于 20:00，则发送问候 "Good day"，否则发送问候 "Good evening"：

if (time<10)
  {
  x="Good morning";
  }
else if (time<20)
  {
  x="Good day";
  }
else
  {
  x="Good evening";
  }

x 的结果是：

Good day

参考：demo3.html


