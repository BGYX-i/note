# **数组介绍**

![image-20211202222239080](../Picture_saving_address/JAVA-第六章/image-20211202222239080.png)

```
package java_study;

public class ArrayTest {
    public static void main(String[] args) {
        //定义一个数组
        //double[]  表示duoble类型的数组，数组的名称是 hens
        //{3,5,1,3.4,2,50}  表示数组的值/元素,一次表示数组的第几个元素
        double[] hens={3,5,1,3.4,2,50};
//        变量数组得到数组的所有元素的和，使用for
//        通过数组hes[下标]来访问数组的元素
//        下标是从0开始编号的，比如第一个元素是hes[0]，第二个就是hes[1],以此类推
//        通过for循环可以循环的访问 数组的元素/值
//        在java中，可以通过数组名称.length 得到数组的大小长度
        double totalWeight=0;
        for(int i=0;i<6;i++){
            totalWeight+=hens[i];
        }
        System.out.println("总体重是："+totalWeight);
        System.out.println("平均体重是："+(totalWeight/6));
    }
}
```

## **数组的使用方式**：

#### **使用方法1-动态初始化**

![image-20211202224353456](../Picture_saving_address/JAVA-第六章/image-20211202224353456.png)

```
1.中括号可以写在数据类型后面或者是写在数组名后面
2.初始化的内容根据不同数据类型使用不同的默认值 int：0 double：0.0 等等
3.数组的下标是从0开始的

        double[] chengJ=new double[5];
        Scanner scanner = new Scanner(System.in);
        for(int index=0;index<chengJ.length;index++){
            System.out.println("请输入第"+(index+1)+"个成绩");
            chengJ[index]=scanner.nextDouble();
        }
        for(int index=0;index<chengJ.length;index++){
            System.out.println("第"+(index+1)+"个成绩为："+chengJ[index]);
        }
    }
}
```

![image-20211202224807661](../Picture_saving_address/JAVA-第六章/image-20211202224807661.png)

#### 使用方式2-动态初始化

![image-20211212104626493](../Picture_saving_address\typora-user-images\image-20211212104626493.png)

```
int[] a;  先声明数组在new分配空间
a=new int[5];

```

![image-20211215214820939](../Picture_saving_address/JAVA-第六章数组/image-20211215214820939.png)

#### 使用方式2-静态初始化

![image-20211215215221282](../Picture_saving_address\typora-user-images\image-20211215215221282.png)

#### 数组的使用细节：

![image-20211215215458382](../Picture_saving_address\typora-user-images\image-20211215215458382.png)

 

```
//        1.数组是多个相同类型的数据的组合，实现对这些数据的统一管理
        double[] arr1={2,3,4,5,1.1 };
//        2.数组中的元素可以是任何数据类型，包括基本数据类型和引用数据类型，但是不能混用
//        3.数组创建后，如果没有复制，有默认值
//        int 0，short 0，byte 0，,long 0,
        short arr[]=new short[3];
        for (int i=0;i<arr.length;i++){
            System.out.println(arr[i]);
        }
//        double 0.0，float 0.0;
//        char \u0000
//        boolean fales;
//        String null;
//        4.使用数组的步骤：先声明数组并开辟空间，给数组个个元素赋值，使用数组
//        5.数组的下标都是从0开始
//        6.数组的下标必须在制定的范围使用，否则会报 下标越界  最大下标 数组的长度-1
        System.out.println(arr[3]);
//        7.数组属于引用数据类型，数组型数据是对象（Object）
```

#### 数组的赋值机制

![image-20211215224625335](../Picture_saving_address\typora-user-images\image-20211215224625335.png)

 

```
int[] arr1={1,2,3};
int[] arr2=arr1;//吧arr1赋给arr2;
arr2[0]=10;
值（值拷贝）传递和引用传递（地址拷贝）的区别：
jvm内存：jvm中内存分3个部分，栈 堆 方法区
基本数据类型存储在栈中（存储值）  值拷贝
引用数据类型在栈中存储一个地址，地址指向堆中空间内的数据 

在内存里面只要分配了一个空间，一定会对应一个地址
基本数据类型拷贝具体的数据，引用数据类型拷贝的是地址
```

![image-20211216230142851](../Picture_saving_address\typora-user-images\image-20211216230142851.png)

#### 数组拷贝：

![image-20211220231228341](../Picture_saving_address\typora-user-images\image-20211220231228341.png)

![image-20211220234833921](../Picture_saving_address\typora-user-images\image-20211220234833921.png)

#### 数组添加

![image-20211223224214109](../Picture_saving_address\typora-user-images\image-20211223224214109.png)

#### 排序的介绍：

![image-20211226212948370](../Picture_saving_address\typora-user-images\image-20211226212948370.png)

#### 二位数组：

```
//什么是二位数组：
//1.从定义形式上看 int[][]
//2.相当于你原来的一维数组的，每个元素是又是一个一维数组，就构成了二维数组
```

#### 二位数组的使用方式：![image-20211227231634106](../Picture_saving_address\typora-user-images\image-20211227231634106.png)

```
第一个中括号大小代表：包含几个一维数组
第二个中括号大小代表：每一个一维数组里面有几个元素
```

![image-20211227232316414](../Picture_saving_address\typora-user-images\image-20211227232316414.png)

###### 数组在内存中的存储：

![image-20211227232845031](../Picture_saving_address\typora-user-images\image-20211227232845031.png)

#### 二位数组使用方式(第二章)：动态初始化

![image-20211229223015329](../Picture_saving_address\typora-user-images\image-20211229223015329.png)

```
int arr[][];
arr=new int[2][3];
```

#### 二位数组使用方式（第三种）：动态初始化-列数不确定

在java中二维数组中的每一个一维数组的个数不一致（列数不确定）

#### 二位数组第四种使用方法：静态初始化

![image-20211229224912611](../Picture_saving_address\typora-user-images\image-20211229224912611.png)

#### 二位数组的使用细节：

![image-20211230222553884](../Picture_saving_address\typora-user-images\image-20211230222553884.png)

本章作业：

![image-20220103221404408](../Picture_saving_address\typora-user-images\image-20220103221404408.png)

![image-20220103222013700](../Picture_saving_address\typora-user-images\image-20220103222013700.png)

```
在ArrayTest02类中有
```

#### 数组内容回顾：

![image-20220105222108143](../Picture_saving_address\typora-user-images\image-20220105222108143.png)

![image-20220105222405368](../Picture_saving_address\typora-user-images\image-20220105222405368.png)

![image-20220105222433511](../Picture_saving_address\typora-user-images\image-20220105222433511.png)

![image-20220105222445577](../Picture_saving_address\typora-user-images\image-20220105222445577.png)

![image-20220105222452589](../Picture_saving_address\typora-user-images\image-20220105222452589.png)

![image-20220105222647738](../Picture_saving_address\typora-user-images\image-20220105222647738.png)

![image-20220105222820232](../Picture_saving_address\typora-user-images\image-20220105222820232.png)

![image-20220105223003045](../Picture_saving_address\typora-user-images\image-20220105223003045.png)

![image-20220105223008543](../Picture_saving_address\typora-user-images\image-20220105223008543.png)

![image-20220105223024164](../Picture_saving_address\typora-user-images\image-20220105223024164.png)

![image-20220105223101909](../Picture_saving_address\typora-user-images\image-20220105223101909.png)

  
