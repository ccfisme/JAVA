  一直不明白，什么是类（指的是.java文件里class中的一个），想探究其中的原理，却找不到对应的汇编，因为java的编译流程和c语言根本不同，不过好在我发现了java和c++之间竟然有着许许多多相同的地方，所以我认为，可以和c++对照着学习  

  那么，c++是如何定义类的呢？我找到一篇[极好的文章](https://bbs.pediy.com/thread-269611.htm)来理解，这个文章的汇编不仅可以用来学c++，同样也是可以用来对照学java  
  
  文中指出，c++的类和结构体十分类似，区别只在于类的变量有private修饰，那么private是干什么用的呢？  
  
  一开始我以为是某种含有指针的结构体，后来发现，private在编译时根本没在汇编中体现，这是一个说明符，告诉编译器只知道类里面变量名字的不能访问，得知道地址才能访问，而在java里面，是通过三种方法访问。构造函数、set函数、get函数。  
  
  set和get函数好理解，是通过指针直接访问的，那么，构造函数是什么东西？  
  
  说实话，查了之后我仍然不理解为什么有。这个东西就像是结构体变量，比如struct一个结构体ccf，然后ccf.aq = 0,ccf.gr = 0......这样赋初值，那么结构体里面也有构造函数吗？  
  
  ![image](https://user-images.githubusercontent.com/74129445/143681670-fc5ed021-b42f-40e4-a934-df7f648c2b67.png)  
  
  mmp，还真有，是我的错了，为什么C语言结构体没有呢？  
  
  ![image](https://user-images.githubusercontent.com/74129445/143681886-264a7c00-8603-4698-9923-bf165b77fb2c.png)  
  
  ![image](https://user-images.githubusercontent.com/74129445/143682004-cfa2f459-b214-4a64-a484-d8fff8a84c92.png)  
  
  
  我明白了，之前的C语言使用结构体时如果不初始化，那么就是随机值，很傻逼，所以工作者就设置了默认的构造函数，用来全部初始化为0，如果想改一两个初始化的值，还可以在构造函数自己设置  
  
  当然，这里面的设置初值和改变初值仅对于一个变量而言，因为没有数据库，所以对一个数据的多次set仅仅是覆盖原值  
  
  另外，如果写有参构造函数，那么默认构造函数会去掉，改为有参构造函数的参数特定初始化，没特定的就按默认  
  
  ![image](https://user-images.githubusercontent.com/74129445/143687971-68b5b7fc-9741-4fec-bbbc-b4e040c14c5d.png)  
  
  ![image](https://user-images.githubusercontent.com/74129445/143687978-c484af2e-c7e2-4508-8c14-beb8418b072e.png)
