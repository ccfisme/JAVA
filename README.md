# 什么是IOC？  

![IMG_20211130_222847](https://user-images.githubusercontent.com/74129445/144066020-e7362bef-1021-4890-b7f3-07a27c220c2c.jpg)  

# 例：在Test中通过.xml创建一个对象  
1.导入依赖  

2.写.xml文件  

![image](https://user-images.githubusercontent.com/74129445/144100138-c6ed4ac6-b642-4fbb-b4dd-097b3db5ae28.png)  

3.指定.xml文件，创建applicacontext接口的实例对象，只有在此实例对象中才能调用spring创建的对象（也就是.xml的bean）  

![image](https://user-images.githubusercontent.com/74129445/144100517-eb2e33d4-7e43-455f-ac5b-c873c217b2ed.png)  

4.从.xml中的bean找到对象


