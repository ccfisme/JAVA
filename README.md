# 怎么使用注解？  

![IMG_20211201_013531](https://user-images.githubusercontent.com/74129445/144098647-2a0f65d1-210e-4d68-b82c-941e1e28f511.jpg)


### 例：@component（创建容器），等同于bean标签  

1.写类，类里面加注解

![image](https://user-images.githubusercontent.com/74129445/144097023-096fc505-5175-46a1-abae-51d145a81a81.png)  

2.告诉类去哪里找注解，即在xml文件指定一个组件扫描器

![image](https://user-images.githubusercontent.com/74129445/144097937-b74f2b54-3bad-4c3d-82f9-5c57636a0c79.png)  

测试类与.xml相同  

![image](https://user-images.githubusercontent.com/74129445/144098214-f59bdc9c-fc73-4169-b8a2-b110be84c68d.png)

### @Repository    

![image](https://user-images.githubusercontent.com/74129445/144101622-63af1f93-d368-4c74-b1ab-2b1dd71fe254.png)  

### @Service    

![image](https://user-images.githubusercontent.com/74129445/144101873-e0a1beef-4f37-4957-8a0f-c47ef622e072.png)  

### @controller   

![image](https://user-images.githubusercontent.com/74129445/144102004-febfff6c-6fb9-4ac5-a94a-9ae5987e3c21.png)  

### @value  
  位置在属性上面，直接给当前属性赋值  
  ![image](https://user-images.githubusercontent.com/74129445/144433742-cfed69a0-abf7-4962-9e45-0b0c97de47ef.png)  
### @autowired（找容器里的所有的值）  

![image](https://user-images.githubusercontent.com/74129445/144436282-52e02d09-dc2f-4740-b68d-5420577dc01e.png)




