# 类型转换

## 隐性类型转换
1.  isNaN(demo)
    判断是不是NaN
    先Number(demo)
    在判断是不是NaN
    e.g. NaN, "abd", undefined => true
    其它 false
2.  demo++， +demo， -demo
    先Number(demo)
    再++
    即使转不成数字（NaN), typeof 也是number
3. demo1 +demo2
    有一个是string结果是string
4. demo1 * / - % demo2 
    得number类型的结果
    先Number(demo)
5. &&  ||  !
6. demo1> < <= >=demo2
    其中一个是number 都转换成数字比
    两个string 比 ascii code
7. demo1 == != demo2 
    先Number(demo1) demo2
    undefined == null 与其它任何比较都是false
    NaN啥都不懂连自己都不懂
8. === !==
    不发生类型转换的等于和不等于

没有定义的变量 在typeof（）里会返回“undefined”字符串
            其它情况都会报错


    

## 显性

1. Number(demo)
    Number(true) =>1
    Number(null) =>0
    Number(undefined/"asdk") => NaN
2. parseInt(demo, radix)
    demo = "123" => 123
    demo = 12.9 => 12
    demo = true => NaN
    demo = “z" => NaN
    demo = “123abc” = 123
    radix：把输入作为一个多少进制的数
    输出一个十进制的数
    radix： 2-36
3. parseFloat(demo)
    基本跟parseInt 一样，除了转化为float
4. String(demo)
    都转换为字符串
5. Boolean(demo)
    除了六个值：
    其它都是true
6. demo.toString(radix)
    除了undefined 和 null
    把demo作为10进制转换为radix进制


    


