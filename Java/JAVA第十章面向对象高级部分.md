# JAVA面向对象高级：

![image-20220319124228013](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220319124228013.png)

#### 类变量：

![image-20220319125115999](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220319125115999.png)

![image-20220319125336404](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220319125336404.png)

```
//    定义一个类变量，是一个静态变量，static修饰
//    该变量最大的特点是会被Child 类的所有对象实例共享
static变量是所有对象共享的（同一个类的所有对象）
```

类变量内存解析：

![image-20220319130219222](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220319130219222.png)

![image-20220319131457571](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220319131457571.png)

```
//count存放在内存堆空间中（单独空间），类加载的时候会在堆中创建对应的class对象
//内存方法区中有一个空间是静态域，静态属性在静态域中
多种说法，*根据不同jdk版本存放不同的位置
//静态变量是所有对象实例共享的
//静态变量（static变量）是在类加载的时候生成创建
类变量是随着类的加载而创建，所以没有创建实际对象也可以访问
static变量是所有对象共享的（同一个类的所有对象）
```

![image-20220319132014085](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220319132014085.png)

```
类变量的访问，必须遵守，相关的访问权限
```

![image-20220320213431514](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220320213431514.png)

![image-20220320214159383](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220320214159383.png)

#### 类方法：

![image-20220320214606135](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220320214606135.png)

![image-20220320215637894](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220320215637894.png)

![image-20220321222003516](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220321222003516.png)

![image-20220321222322272](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220321222322272.png)

![image-20220322004654597](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220322004654597.png)

![image-20220322004811408](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220322004811408.png)

![image-20220322005423253](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220322005423253.png)

![image-20220322005542593](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220322005542593.png)

#### 代码块：

![image-20220322005646483](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220322005646483.png)

