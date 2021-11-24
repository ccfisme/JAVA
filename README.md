  很显然，直观上看，Java和c语言的编译器根本没有什么关系(其实有关系，Java的编译器是c和c++编写的)，但从原理上，我却嗅到了一丝相似的关系。  
  
  下面，可以看一下两者加载代码机制的图片对比  
  
  * Java加载机制  

  ![image](https://user-images.githubusercontent.com/74129445/143231155-c524cf3c-cb11-4194-987e-6231eee9ec74.png)  
  
  * c语言加载机制  

  ![image](https://user-images.githubusercontent.com/74129445/143231420-e505b6a3-e1f8-4ba2-86f6-3fdf82810f1e.png)  
  
  很明显，在中间的几步是相似的，所以说，Java的类就相当于是对Java函数体的一个包装，没什么别的意思，就是为了在加载的时候区分一下，知道这是要找的那个地方。
  

参考：https://www.cnblogs.com/WangXianSCU/p/15316732.html
