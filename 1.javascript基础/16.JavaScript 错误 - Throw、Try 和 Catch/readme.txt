
目录：
1.异常简介
2.try{}catch(error){}
3.throw



1.异常简介

try 语句测试代码块的错误。
catch 语句处理错误。
throw 语句创建自定义错误。

错误一定会发生
当 JavaScript 引擎执行 JavaScript 代码时，会发生各种错误：
可能是语法错误，通常是程序员造成的编码错误或错别字。
可能是拼写错误或语言中缺少的功能（可能由于浏览器差异）。
可能是由于来自服务器或用户的错误输出而导致的错误。
当然，也可能是由于许多其他不可预知的因素。

JavaScript 抛出错误
当错误发生时，当事情出问题时，JavaScript 引擎通常会停止，并生成一个错误消息。
描述这种情况的技术术语是：JavaScript 将抛出一个错误。

JavaScript 测试和捕捉
try 语句允许我们定义在执行时进行错误测试的代码块。
catch 语句允许我们定义当 try 代码块发生错误时，所执行的代码块。
JavaScript 语句 try 和 catch 是成对出现的。


2.try{}catch(error){}

语法
try
  {
  //在这里运行代码
  }
catch(err)
  {
  //在这里处理错误
  }

在下面的例子中，我们故意在 try 块的代码中写了一个错字。
catch 块会捕捉到 try 块中的错误，并执行代码来处理它。

        <!DOCTYPE html>
        <html>
        <head>
        <script>
        var txt="";
        function message()
        {
        try
          {
          adddlert("Welcome guest!");
          }
        catch(err)
          {
          txt="There was an error on this page.\n\n";
          txt+="Error description: " + err.message + "\n\n";
          txt+="Click OK to continue.\n\n";
          alert(txt);
          }
        }
        </script>
        </head>

        <body>
        <input type="button" value="View message" onclick="message()">
        </body>

        </html>

    参考：demo1.html

3.throw 语句

Throw 语句
throw 语句允许我们创建自定义错误。
正确的技术术语是：创建或抛出异常（exception）。
如果把 throw 与 try 和 catch 一起使用，那么您能够控制程序流，并生成自定义的错误消息。

语法

throw exception

异常可以是 JavaScript 字符串、数字、逻辑值或对象。

实例
本例检测输入变量的值。如果值是错误的，会抛出一个异常（错误）。catch 会捕捉到这个错误，并显示一段自定义的错误消息：

        <script>
        function myFunction()
        {
        try
          {
          var x=document.getElementById("demo").value;
          if(x=="")    throw "empty";
          if(isNaN(x)) throw "not a number";
          if(x>10)     throw "too high";
          if(x<5)      throw "too low";
          }
        catch(err)
          {
          var y=document.getElementById("mess");
          y.innerHTML="Error: " + err + ".";
          }
        }
        </script>

        <h1>My First JavaScript</h1>
        <p>Please input a number between 5 and 10:</p>
        <input id="demo" type="text">
        <button type="button" onclick="myFunction()">Test Input</button>
        <p id="mess"></p>

参考：demo2.html

