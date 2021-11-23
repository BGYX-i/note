**JAVA-控制结构：**

![image-20211121195046284](../Picture_saving_address/JAVA-第五章程序控制结构/image-20211121195046284.png)

**程序流程控制介绍：**

![image-20211121195153969](../Picture_saving_address/JAVA-第五章程序控制结构/image-20211121195153969.png)

**顺序控制：**

![image-20211121195309010](../Picture_saving_address/JAVA-第五章程序控制结构/image-20211121195309010.png)

**分支控制：**

![image-20211121195530349](../Picture_saving_address/JAVA-第五章程序控制结构/image-20211121195530349.png)

1.单分支：分支控制if-else：

![image-20211121195708122](../Picture_saving_address/JAVA-第五章程序控制结构/image-20211121195708122.png)

2.双分支：分支控制if-else

![image-20211121201140288](../Picture_saving_address/JAVA-第五章程序控制结构/image-20211121201140288.png)

3.多分支：分支控制if-else if-else：

![image-20211121204224769](../Picture_saving_address/JAVA-第五章程序控制结构/image-20211121204224769.png)

![image-20211121204452213](../Picture_saving_address/JAVA-第五章程序控制结构/image-20211121204452213.png)

特别说明：1.多分支可以没有else，如果所有的条件表达式都不成立，则一个执行入口都没有

​					2.如果有elsel语句，如果所有的条件表达式都不成立，则默认执行else代码块

3.switch分支结构：

![image-20211121213709228](../Picture_saving_address/JAVA-第五章程序控制结构/image-20211121213709228.png)

 Switch快速入门

![image-20211122214653278](../Picture_saving_address/JAVA-第五章程序控制结构/image-20211122214653278.png)

```
在java中，只有有值返回，就是一个表达式
```

switch分支细节讨论：

![image-20211122215702748](../Picture_saving_address/JAVA-第五章程序控制结构/image-20211122215702748.png)

```
case字句中的值必须是常量不能是变量
```

```
//switch 表达式中的返回值必须是：
// ('char、byte、short、int、Character、Byte、Short、Integer、String 或枚举')
```

```
//default子句是可选的，当没有匹配case时执行default
```

```
//break语句是执行完一个case分支后使程序跳出switch语句块，如果没有写break，程序会顺序执行到switch结尾
```

![image-20211122232902256](../Picture_saving_address/JAVA-第五章程序控制结构/image-20211122232902256.png)

fot循环控制：

![image-20211123212732625](../Picture_saving_address/JAVA-第五章程序控制结构/image-20211123212732625.png)