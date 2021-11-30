# 怎么使用注解？  

![IMG_20211201_013531](https://user-images.githubusercontent.com/74129445/144098647-2a0f65d1-210e-4d68-b82c-941e1e28f511.jpg)


### 例：@component（可创建对象），等同于bean标签  

1.写类，类里面加注解

![image](https://user-images.githubusercontent.com/74129445/144097023-096fc505-5175-46a1-abae-51d145a81a81.png)  

2.告诉类去哪里找注解，即在xml文件指定一个组件扫描器

![image](https://user-images.githubusercontent.com/74129445/144097937-b74f2b54-3bad-4c3d-82f9-5c57636a0c79.png)  

测试类与.xml相同  

![image](https://user-images.githubusercontent.com/74129445/144098214-f59bdc9c-fc73-4169-b8a2-b110be84c68d.png)

### @Repository （可创建对象）   

![image](https://user-images.githubusercontent.com/74129445/144101622-63af1f93-d368-4c74-b1ab-2b1dd71fe254.png)  

### @Service  （可创建对象）  

![image](https://user-images.githubusercontent.com/74129445/144101873-e0a1beef-4f37-4957-8a0f-c47ef622e072.png)  

### @controller  （可创建对象）  

![image](https://user-images.githubusercontent.com/74129445/144102004-febfff6c-6fb9-4ac5-a94a-9ae5987e3c21.png)  



