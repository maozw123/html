# Javascript入门

行为

## 1. javascript 简介

简称  js  脚本语言  然后运行在前端 

特点 ：

- 语法简单
- 动态性
- 跨平台
- 弱类型
  - 弱类型  强类型 都是针对变量而言的，弱类型会根据环境改变类型
  - js vb php  1+1 1+‘1’ = ‘11’      1+‘asds'= '1asds'
  - c java python     1+1 1+‘1’ 

ECMScript：定义js的规范，js核心

DOM   文档对象模型，操作文档，设置 获取文档的属性 

BOM   浏览器对象模型，针对浏览器  

## 2. javascript 引入方式

- 行内式

  - 标签内写js

    ```
    <!--行内式-->
    <!--<button onclick="alert('你点我了')">点我</button>-->
    ```

    

- 内嵌式

  - 文档内部写   由script包围的js代码

  - ```
    <!--内嵌式-->
    <!--<script>-->
    <!--    alert("我是内嵌式");-->
    <!--</script>-->
    ```

    

- 外链式

  - 外部常见一个js目录  在里面写入js代码

  - 通过script 导入js代码

  - ```
        <script src="./js/1.js" type="text/javascript">
            //console.log("我是外链式");  这段代码不被执行
        </script>
    ```

    

## 3. javascript常用输出方式

```js
<p id="pid">我是一个p段落</p>

<script>
    // 1. 弹框
    // alert("我是弹框");
    // 2. 输出到控制台
    // console.log("我要到控制台")
    //3. DOM 的一种方法   write 可以向文档中写入内容 或者 js 代码
    // document.write("hello")
    //4. DOM的一种方法， 通过id 属性获取 标签元素   innerHTML  获取内容或者 将内容写入
    // document.getElementById("pid").innerHTML="hello world";

</script>

```







## 4. 基础语法

1. 变量的定义

- 变量的定义
  - 关键字  var 变量名  = value;
    - var 变量名 ;    申明一个变量
  - 定义变量区分大小写
- 变量名的选择    不能够以数字开头  可以包含  字符数字 _    $ 
  - 不能够使用关键字  预留字

- 注释  

  ```js
  //  单行
  /**/   多行
  ```

- 语法结构  是以 ; 结尾



2. 变量的类型

   - 数字型     number  

   - NAN number

   - 字符串   string 

   - 数组    object

   - boolean true 真  flase 假

   - 对象   object 

   - null  空

   - undefined   未定义

   - 函数    function

     // 关键字   函数名  参数

     function hello(){

     // 方法体

     }

3. 数据类型

   1. typeof   查看数据类型
   2. isNaN  判断是不是NAN类型   如果是 不是NAN 返回flase 如果是 返回true
   3. instanceof   检测一个实例是不是属于某个对象的

4. 数据类型的转换
   -  强转
     - Number  强制转换 遇到字母 返回的NAN int  float
     - String  转换为字符串非强转  
   - 非强转   parseInt遇到非数字  结束
     - parseFloat 增加了小数

5. 运算符

   1. 计算运算符

      ```
      + - += -= ++ -- / * %
      ```

   2. 赋值运算符

      ```
      = += -= *= /= %=
      ```

   3. 逻辑运算符

      ```
      python  and or not
      &&  ||  ！
      ```

   4. 比较运算符

      ```
      == 判断值是否相等
      ===  判断值和类型是否相等
      != 
      >
      <
      >=
      <=
      ```

      

## 5. 流程控制

1. 判断语句

   1. if else if else
   2. 三目运算符 ？
      1. var result = 条件 ？ 条件成立的时候执行：条件不成立的时候执行

   3.  switch case

      switch(条件)：

      ​	case 值：

      ​		 当条件的值  == case的值的时候执行

      ​	    break;

      ​	default:

      ​       当没有满足的条件的时候执行

   

2. 循环语句

   ```
       for (var i = 1;i<10;++i){
           console.log(i);
       }
       for循环中，第一个语句在开始之前执行
       		 第二个语句在执行代码块的条件
       		 每次在被执行后执行
   ```

   ```
   ++i  先计算  在赋值
   i++   先赋值  然后在计算
   ```





