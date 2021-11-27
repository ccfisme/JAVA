继承我理解为就是一个类完全复制另一个类的结构，包括函数，变量，可以改变复制的原生类的结构，可以拥有自己的属性和方法，即子类可以对父类进行扩展，子类可以用自己的方式实现父类的方法  


出现原因：代码臃肿，对单个子类修改时不好改  

![FireShot Capture 009 - Java 继承 - 菜鸟教程 - www runoob com (1)](https://user-images.githubusercontent.com/74129445/143683222-ef5ce6a1-b18e-44ce-9c5b-e8bf066742f8.png)  

## 继承有两种类型，生一个，生多个  

* 一生多：extends  

![image](https://user-images.githubusercontent.com/74129445/143687675-43303b47-bcb5-4cf2-988e-7a817a3f2797.png)  

![image](https://user-images.githubusercontent.com/74129445/143687617-2a9611e7-354e-4e67-9ed7-4e2d742dbbc1.png)  

有例外，比如如果父类的构造函数有参数，那么在使用父类构造函数初始化子类时就要用super函数  
![image](https://user-images.githubusercontent.com/74129445/143690485-e749f2e6-eafb-461b-be93-56859fb5762c.png)  


* 多生一：implements  
![image](https://user-images.githubusercontent.com/74129445/143688695-37f07462-4177-46c6-92c8-f19eab4e59a9.png)  


![image](https://user-images.githubusercontent.com/74129445/143687683-813400c7-baca-4716-9a41-f0cc5bce6f70.png)  



