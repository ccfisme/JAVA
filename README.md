## 类似`@RestController`这种东西什么意思？pom.xml文件又是干啥的？  

  首先，我对两者进行查询，发现它们有一个共同的特点，就是都是[元数据](https://www.zhihu.com/question/20679872)（装逼词语，不用管）,作用是用pom.xml文件对用到的jar包（java代码压缩文件）进行版本统计、导入jar包，后面用到这些jar包的时候就用@来初始化，这是一个spring执行后的首要任务，即先看@    

  而"位于resources目录下的.properties文件与@的关系"与"pom.xml文件和@的关系"很类似，区别只是.properties文件是配置类内属性的  

  图为.properties文件配置数据库连接

![image](https://user-images.githubusercontent.com/74129445/143769207-ea19a169-88cd-4082-98ea-59c82de57a66.png)  

  然后用@注入属性；.yml文件是.properties文件的浓缩版，更简洁；.xml文件之前也可以配置文件，后面可能解耦合了，就把这个功能删了。  




![image](https://user-images.githubusercontent.com/74129445/143768012-6d7d7d58-8899-48df-a8e7-b53c06827c04.png)  


参考文章：  
[Spring注解配置和xml配置优缺点比较](https://cloud.tencent.com/developer/article/1592029)  

[注解与依赖注入](https://blog.csdn.net/u012070360/article/details/76358512)  

[依赖注入是什么？如何使用它？](https://chinese.freecodecamp.org/news/a-quick-intro-to-dependency-injection-what-it-is-and-when-to-use-it/)  

[Java反射机制详解上篇](https://developer.aliyun.com/article/556706)  

[xml文件实例介绍](https://www.liaoxuefeng.com/wiki/1252599548343744/1309301243117601#0)  

[Java注解之运行时注解](https://juejin.cn/post/6844903879524483085)  

[spring boot配置详解](https://blog.csdn.net/achenyuan/article/details/79912744)  

主要参考文章：  
[看完所有的之后再看就会豁然开朗](https://juejin.cn/post/6844903841972879373)  

参考视频:  
[什么是注解和反射](https://www.bilibili.com/video/BV1p4411P7V3?p=2&spm_id_from=pageDriver)  
[spring框架](https://www.bilibili.com/video/BV1nz4y1d7uy?p=9&spm_id_from=pageDriver)
