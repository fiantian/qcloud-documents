### 操作场景
通过添加 A 记录可将域名指向一个 IP 地址，本文档指导您如何添加 A 记录。
### 操作步骤
1. 登录 [腾讯云云解析控制台](https://console.cloud.tencent.com/cns)。
2. 在“域名解析列表”中，选择需要进行 A 记录转发的域名，进入域名详情页面。
3. 单击【添加记录】，填写以下记录信息。
 ![1](//mc.qcloudimg.com/static/img/82400afe3c333b11ec5c35058fda4d61/image.png)
 - 主机记录：选择子域名。例如添加  www.123.com  的解析时，您在“主机记录”处选择 www 即可。若是想添加 123.com 的解析，您在“主机记录”处选择“@”即可。
 - 记录类型：选择“A”。
 - 线路类型：选择“默认”类型，否则会导致部分用户无法解析。
例如，您需要将联通用户指向8.8.8.8，所有非联通用户都指向10.10.10.10。您可以通过添加线路类型为默认、记录值为10.10.10.10和线路类型为联通、记录值为8.8.8.8的两条 A 记录来实现。
 - 记录值：只可以填写 IPv4 地址。
 - MX优先级：不需要填写。
 - TTL：为缓存时间，数值越小，修改记录各地生效时间越快，默认为600秒。
4. 单击【保存】，完成添加。


