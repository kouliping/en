# Backend Service Signature


The key pair of backend signature adopts JD Cloud User AK/SK(Access Key/Access Key Secret), which will protect your backend through verification of backend signature when the gateway requests your real backend.

您将京东云用户AK/SK密钥绑定到 API分组 上后，当网关请求这个分组下的 API 时，会添加并出示该AK/SK，您的后端通过验证签名字符串来验证网关的身份。

点击左侧 后端签名，进行后端签名的配置和绑定。



## Operational Steps

Click **Backend Signature** at left side to perform the configure and associate

1. Enter the page of backend signature list

![Backend signature list](https://github.com/jdcloudcom/cn/blob/edit/image/Internet-Middleware/API-Gateway/hdqm-list.png)


2. Add backend signature

![Add backend signature](https://github.com/jdcloudcom/cn/blob/edit/image/Internet-Middleware/API-Gateway/hdqm-add.png)


3. Bind the signature to group

![Associate signature](https://github.com/jdcloudcom/cn/blob/edit/image/Internet-Middleware/API-Gateway/hdqm-bd.png)



  
