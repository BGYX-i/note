# Java-面向对象中级编程

#### IDEA（集成开发环境）：

![image-20220214213315103](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220214213315103.png)

#### Eclipse（集成开发工具）：

![image-20220214213426822](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220214213426822.png)

####  IDEA常用快捷键：

![image-20220215225902546](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220215225902546.png)

![image-20220215232315611](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220215232315611.png)

![image-20220215234007239](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220215234007239.png)

![image-20220216222512590](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220216222512590.png)

#### 包概念：

![image-20220216223207449](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220216223207449.png)

#### 包的三大作用：

![image-20220216223231111](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220216223231111.png)

![image-20220216223646160](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220216223646160.png)

#### 包的命名规则和规范：

![image-20220216225257188](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220216225257188.png)

#### Java中常用的包：

![image-20220216225755816](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220216225755816.png)

#### 如何引入包：

![image-20220216230031404](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220216230031404.png)

#### 包的使用细节：

![image-20220216231021812](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220216231021812.png)

#### 访问修饰符：

![image-20220218221016022](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220218221016022.png)

![image-20220218221239050](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220218221239050.png)

#### 面向对象的三大特征：

![image-20220218224620546](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220218224620546.png)

#### 封装：

![image-20220218224637761](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220218224637761.png)

#### 封装的好处：

![image-20220218225004540](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220218225004540.png)

![image-20220218225617789](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220218225617789.png)

![image-20220218225756069](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220218225756069.png)

![image-20220219171120405](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220219171120405.png)

#### 继承：

![image-20220219174148779](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220219174148779.png)

#### 继承的基本介绍：

![image-20220219174551049](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220219174551049.png)

![image-20220219175337577](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220219175337577.png)

#### 继承的便利：

![image-20220219185523832](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220219185523832.png)

```
在父类中增加一个方法，那么继承它的子类都会继承这个方法
```

#### 继承的细节：

![image-20220219185849459](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220219185849459.png)

![image-20220219191559025](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220219191559025.png)

![image-20220220165620971](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220220165620971.png)

```
super();关键字只能在构造方法中使用
```

![image-20220220171227129](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220220171227129.png)

```
8：构造器一直追溯到顶级父类
先执行Object 的构造器，在执行a的构造器，在执行b的构造器，最后执行c的构造器
```

![image-20220220172132459](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220220172132459.png)

#### 继承的本质：

![image-20220220172636865](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220220172636865.png)

```
package src.com.hspedu.extend_;
//继承的本质
public class ExtendsTherory {
    public static void main(String[] args) {
        Son son = new Son();//内存到底发生了什么
    }

}
class GanPa{
    String name="大头爷爷";
    String hobby="旅游";
}
class Father extends GanPa{//父类
    String name="大头爸爸";
    int age=39;
}
class  Son extends Father {//子类
    String name="大头儿子";
}
//如下图
1.第一个加载的是object类
2.第二个加载的是GanPa类
3.第三个加载的是Father类
4.最后加载Son类             他们之间会有一个关联关系，在方法区形成类和类的继承关系
5.在堆中分类内存空间，首先会给GanPa类分配空间，分配属性
6.再给Father类分配空间分配属性
7.最后给Son类分配空间分配属性
7.主空间分配给代码中的对象引用       在堆中分配空间，同名属性不冲突，整个对象还是叫Son

当子类对象引用访问对象中的属性的时候，是用什么规则访问的
```

![image-20220220174428678](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220220174428678.png)

```
//	访问属性，按照查找关系来返回信息
//   1.首先看子类的属性，看子类是否有该属性
//   2.如果子类有这个属性，并且可以访问，则返回信息
//   3.如歌子类没有这个属性，就看父类有没有这个属性（父类如果有并且可以访问，则返回信息）
//   4.如果父类没有，这按照3的规则继续找上一级父类，知道Object
```

#### super关键字：

![image-20220220222723819](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220220222723819.png)

#### super的使用细节：

![image-20220220223709665](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220220223709665.png)

![image-20220220225309091](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220220225309091.png)

![image-20220220225845995](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220220225845995.png)

![image-20220220230120985](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220220230120985.png)

#### 方法重写：

![image-20220222215124752](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220222215124752.png)

#### 方法重写的注意事项：

![image-20220222220131086](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220222220131086.png)

```
    子类方法返回类型和父类方法返回类型一致；
//  方法的返回数据类型是父类返回类型的子类  比如：父类返回object 子类返回 String也构成方法重写
```

![image-20220223214148698](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220223214148698.png)

#### 面向对象编程多态：

![image-20220224220716072](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220224220716072.png)

```
//多态提高代码的复用性
```

![image-20220228223817878](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220228223817878.png)

![image-20220228224528686](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220228224528686.png)

![image-20220228231012864](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220228231012864.png)

####  多态的使用细节：

向上转型：

![image-20220301220132421](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220301220132421.png)

```
父类引用指向子类对象，就是想上转型
Animal animal = new Dog();
可以的调用父类的所有方法但是需要遵守访问权限，但是不能调用子类特有的成员（方法和属性）
因为在编译阶段，能调用成员（方法和属性）是由编译类型来决定的
最终运行效果看子类的具体实现
```

向下转型：

![image-20220301223312799](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220301223312799.png)

```
Cat cat=(Cat) animal;
编译类型是 Cat 运行类型是 Cat
父类的引用必须指向的是当前目标类型的对象
```

![image-20220301225434954](../Picture_saving_address/JAVA-第七章面向对象中级编程/image-20220301225434954.png)

```
public class Polydetail02 {
    public static void main(String[] args) {
        Base base=new sub();
        System.out.println(base.count);//10
        sub sub=new sub();
        System.out.println(sub.count);//20

    }
}
class Base{
    int count=10;
}
class sub extends Base{
    int count=20;
}
//访问属性直接看编译类型

```

```
public class PolyDetail03 {
    public static void main(String[] args) {
        BB bb = new BB();
        System.out.println(bb instanceof BB);//true
        System.out.println(bb instanceof AA);//true
//    编译类型是AA  运行类型是 BB  instanceof 判断对象的运行类似是否为某某类型货某某类型的子类
        AA aa = new BB();
        System.out.println(aa instanceof AA);
        System.out.println(aa instanceof BB);

    }
}
class AA{

}
class BB extends AA {

}
```

