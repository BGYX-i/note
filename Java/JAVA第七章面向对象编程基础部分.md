## 面向对象编程基础部分

![image-20220105224148978](E:\Self_study_notes\Picture_saving_address\typora-user-images\image-20220105224148978.png)

![image-20220105224158918](E:\Self_study_notes\Picture_saving_address\typora-user-images\image-20220105224158918.png)

![image-20220105225819452](E:\Self_study_notes\Picture_saving_address\typora-user-images\image-20220105225819452.png)

#### 类与对象的概述：

![image-20220105230122473](E:\Self_study_notes\Picture_saving_address\typora-user-images\image-20220105230122473.png)

```
1.对象主要是由:属性和行为组成的
```

![image-20220105231049071](E:\Self_study_notes\Picture_saving_address\typora-user-images\image-20220105231049071.png)

```
1.类也是一种数据类型（自定义的数据类型）
2.对象就是一个具体的实例（事务）（通过类来创建一直具体的对象（一只具体的猫））
例如：人类（类） 对应具体的人，小明，小红，小刚（对象）
3.对象也是引用数据类型
4.String是引用数据类型
```

#### 类和对象的区别：

![image-20220106224518256](E:\Self_study_notes\Picture_saving_address\typora-user-images\image-20220106224518256.png)

## 对象在内存中的存在形式：

![image-20220106225305313](E:\Self_study_notes\Picture_saving_address\typora-user-images\image-20220106225305313.png)

![image-20220106230810835](E:\Self_study_notes\Picture_saving_address\typora-user-images\image-20220106230810835.png)

```
1.在new的过程，会把我们类的信息加载到方法区
  加载Cat类信息：1.属性信息
  				//属性可以是基本数据类型，也可以是引用数据类型（对象和数组）
  		       2.行为（方法信息）
 2.真正的对象在堆中（包括方法区的数据），栈中的cat只是对象引用或对象名
 3.对象的默认值，与数组的一致
```

![image-20220106231544248](E:\Self_study_notes\Picture_saving_address\typora-user-images\image-20220106231544248.png)

![image-20220106225510077](E:\Self_study_notes\Picture_saving_address\typora-user-images\image-20220106225510077.png)

#### 属性和成员变量的概念：

![image-20220106225658066](E:\Self_study_notes\Picture_saving_address\typora-user-images\image-20220106225658066.png)

field 字段

#### 属性的注意事项：

![image-20220106230101081](E:\Self_study_notes\Picture_saving_address\typora-user-images\image-20220106230101081.png)

```
访问修饰符是控制属性的方位范围：
有4中访问修饰符，public ，proctected，private，默认
```

#### 创建对象的两种方式：

![image-20220106232124152](E:\Self_study_notes\Picture_saving_address\typora-user-images\image-20220106232124152.png)

#### 如何访问属性：

![image-20220106232152848](E:\Self_study_notes\Picture_saving_address\typora-user-images\image-20220106232152848.png)

