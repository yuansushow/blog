# JS中的逻辑运算符踩坑

&& 与 || 不是相同的优先级！！！（& 和 | 也不是）<br>
1 || 0 && 0  结果是 1 

同时，对于 ||  和  &&  而言。并非是将两侧的变量转换成布尔类型再进行逻辑运算，而是：<br>
先将左侧的变量转换成布尔类型，然后判断真假。<br>
对于 || ，而言 左侧为真返回左侧的数据（不一定是布尔类型），左侧为假则返回右侧的数据。
即  
```javascript
'aaa' || 'bbb' //  ->   'aaa'
0 || '222'     //  ->   '222'
77 || 99       //  ->   77
```
同理，对于&&也是类似的情况。

位运算 `  |   &  ~   ^  <<   >> `<br> >>>只对整数起作用，不是整数则尝试转换成整数。浮点数截断小数部分，字符串则尝试转换成整数，失败则视为0。
