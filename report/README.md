在pos-carts中的checkout方法中，利用restTemplate调用pos-order模块的方法生成一个order，并清空购物车。pos-order中，每生成一个order，就向pos-delivery模块发送一个消息，pos-delivery接受到消息后就生成一个delivery。

展示如下：

首先创建一个购物车
![image](cart.png)

然后checkout
![image](checkout.png)

可看到delivery信息
![image](delivery.png)