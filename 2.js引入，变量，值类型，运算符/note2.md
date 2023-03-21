# 引入
1. 页面级js 内部文件
<script type='text/javascript'>
</script>
放html head或body
里面写代码

2. 外部文件
<script type='text/javascript' src=““>
</script>

一般用外部文件
结构 行为 样式 相分离
html js  css
1. 看起来清晰
2. 好维护

# 编程


# 变量（variable
~~~
var a = 10,
    c,
    e; //变量声明
a = 100; //变量赋值
var b = a; //
document.write(a,b,c,d,e)
<!-- '='赋值符号 -->
~~~
1. 变量名开头 $,_,英文
2. 变量名其它 开头+数字
3. 不可以用系统关键字保留字做变量名
4. 运算大于赋值

# 动态语言-解释性语言-脚本语言
## 动态语言
    生成变量只用 var
    浮点型


## 数据类型
1. 原始值
放在stack filo
Number Boolean String undefined null
undefined一般代表没赋值
null空的但没值 空值
不可改变：进去就改不了了

2. 引用值
heap
array Object function ... date RegExp
e.g.
    var arr = [1,2,3,]

区别 e.g.
var a = 3;
var b = a;//b拷贝a的值
a = 1;
这个时候 b 等于3

var arr = [1,2];
var arr2 = arr;//拷贝地址
arr.push(3);
这个时候arr2值也变 引用值相当于一个pointer
arr = [1,3];//赋值指向新地址 地址在stack里

# js语法
一句一分号
运算符号两遍加空格
## 错误
1. 低级错误（语法错误）
var a = 10:
一行不会执行
2. 逻辑错误
document.write(b)
b没被生成 会执行到这行

不管什么错误不影响到其它块儿

# 运算符号
先括号
乘除
从左往右
1. +
    数学预算
    任何数据+字符串都是字符串
2. -， *，/, %
    1/0 = infinity
    0/0 = NaN
3. ++,--，+=
    document.write(a ++) //先输入a在++
    document.write(++a)  //先++在输出
    b = a++后
    a也会变

赋值顺序从右向左 运算从左向右















