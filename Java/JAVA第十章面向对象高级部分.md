#  JAVA面向对象高级：

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

![image-20220322232503126](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220322232503126.png)

![image-20220322233314009](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220322233314009.png)

![image-20220322234849659](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220322234849659.png)

![image-20220323232505910](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220323232505910.png)

![image-20220323233002429](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220323233002429.png)

![image-20220323234424224](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220323234424224.png)

#### 单例设计模式：

![image-20220323234559732](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220323234559732.png)

![image-20220323234730849](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220323234730849.png)

#### 单例（单个的实例）

![image-20220323234842128](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220323234842128.png)

```
构造器私有化，防止直接new
饿汉式：有可能还没有用到对象，对象就被创建好了，在类加载的时候对创建了
使用单例模式的对象通常都是重要级的对象，饿汉式可能造成创了对象但是没有使用
```

![image-20220323235932984](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220323235932984.png)

```
懒汉式：在使用的时候创建对象
懒汉式：只用在当用户使用getInstance，才返回cat对象
```

![image-20220324001200941](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220324001200941.png)

![image-20220324001708121](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220324001708121.png)

#### final关键字：

![image-20220324001739274](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220324001739274.png)

![image-20220324231943852](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220324231943852.png)

![image-20220324232915461](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220324232915461.png)

![image-20220324234235367](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220324234235367.png)

![image-20220327161412869](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220327161412869.png)

![image-20220327161514823](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220327161514823.png)

![image-20220327161525444](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220327161525444.png)

![image-20220327161653143](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220327161653143.png)

![image-20220327161958631](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220327161958631.png)

![image-20220327162331525](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220327162331525.png)

![image-20220327162742283](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220327162742283.png)

![image-20220327163531231](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220327163531231.png)

![image-20220327174819272](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220327174819272.png)

![image-20220327183513953](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220327183513953.png)

![image-20220327223723371](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220327223723371.png)

![image-20220327224442296](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220327224442296.png)

![image-20220327224751682](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220327224751682.png)

![image-20220327224913196](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220327224913196.png)

![image-20220406134534642](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406134534642.png)

![image-20220406135533049](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406135533049.png)

![image-20220406153642958](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406153642958.png)

![image-20220406154313838](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406154313838.png)

![image-20220406154728719](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406154728719.png)

![image-20220406163930061](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406163930061.png)

5.内部类

#### 内部类：

![image-20220406172539903](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406172539903.png)

![image-20220406173302256](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406173302256.png)

![image-20220406173649894](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406173649894.png)

![image-20220406190853780](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406190853780.png)

![image-20220406190919326](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406190919326.png)

1.本质是类，

2.内部类

3.没用类名

![image-20220406195708850](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406195708850.png)

![image-20220406202347281](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406202347281.png)

![image-20220406202713853](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406202713853.png)

![image-20220406203307564](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406203307564.png)

![image-20220406204038313](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406204038313.png)

![image-20220406205105720](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406205105720.png)

![image-20220406215249941](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406215249941.png)

![image-20220406215855290](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406215855290.png)

![image-20220406221157221](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220406221157221.png)

 

![image-20220407123605652](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407123605652.png)

![image-20220407125206431](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407125206431.png)

![image-20220407130426311](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407130426311.png)

#### 枚举：

![image-20220407131135379](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407131135379.png)

![image-20220407144542397](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407144542397.png)

![image-20220407144630301](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407144630301.png)

![image-20220407144735512](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407144735512.png)

![image-20220407144751257](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407144751257.png)

![image-20220407145632032](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407145632032.png)

枚举第二种方式：

![image-20220407145726761](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407145726761.png)

![image-20220407151250652](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407151250652.png)

Javap 反编译：把class文件编译成java文件

![image-20220407151206384](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407151206384.png)

![image-20220407193558474](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407193558474.png)

![image-20220407200313078](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407200313078.png)

![image-20220407200330617](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407200330617.png)

#### 注解：

![image-20220407201831938](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407201831938.png)

![image-20220407202000167](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407202000167.png)

![image-20220407202132375](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407202132375.png)

```
//     @Override放在say方面上面表示子类重写了父类的say方法
//    这里如果没有写 @Override的注解 那么他还是重新了父类方法
//    如果写了 @Override 编译器就会去检查该方法是否真的重写了父类的某方法
//    如果的确重写了则编译通过，如果没有构成重写则编译错误
    /*
       如果看到 @interface 表示一个 注解类
     @Target(ElementType.METHOD)
     @Retention(RetentionPolicy.SOURCE)
        public @interface Override {
    }
    */
```

![image-20220407203303555](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407203303555.png)

![image-20220407203518220](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407203518220.png)

![image-20220407204049178](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220407204049178.png)

```
//@Deprecated 修饰一个元素表示该元素已经过时了
// 既不在推荐使用，但是仍然可以使用
```

![image-20220408153302213](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220408153302213.png)

![image-20220408153615024](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220408153615024.png)

![image-20220408154342676](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220408154342676.png)

![image-20220408154733624](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220408154733624.png)

![image-20220408171647727](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220408171647727.png)

![image-20220408172009993](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220408172009993.png)

![image-20220408172023294](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220408172023294.png)

![image-20220408172226245](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220408172226245.png)

![image-20220408181554828](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220408181554828.png)

![image-20220408181744736](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220408181744736.png)

![image-20220408181845382](../Picture_saving_address/JAVA第十章面向对象高级部分/image-20220408181845382.png)

