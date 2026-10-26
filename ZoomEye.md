1.
  与ZoomEye类似的搜索引擎还有所属于美国的Shodan，其是最早的物联网设备搜索引擎，擅长搜索服务器、摄像头、数据库等设备banner。  
同时还有FOFA Censys Quake Hunter FullHunt等与ZoomEye功能类似的搜索引擎。  

2.
  ![ZoomEye搜索结果](https://raw.githubusercontent.com/Chenyuzhiying0/111111.github.io/main/image/ZoomEye%20search%20result.png)  
在ZoomEye中搜索"app:Apache"，结果如图片所示。  

从搜索结果可以看到，平台展示了 HTTP 状态码、响应头以及服务器软件标识等信息。  
这些内容可以帮助我们初步了解目标公开服务的技术特征。  

HTTP 状态码：  
结果中的 HTTP/1.1 200 OK 表示服务器成功处理了本次 HTTP 请求。  
它只能说明这次请求获得了成功响应，不能证明服务器没有安全漏洞。  

Content-Type 和 Content-Length：  
content-type: text/html;charset=UTF-8 表示响应内容的媒体类型为 HTML，字符编码为 UTF-8。  
content-length: 2 表示响应正文的长度为 2 字节。它与响应头本身的长度不同。  

Server 字段：  
本次结果中的 server 字段非常长，其中出现了 Apache、nginx、Jetty、LiteSpeed 等多种服务器软件名称，还包含一些网络设备和应用组件的标识。  
正常情况下，Server 响应头通常用于提供服务器软件的标识。但本次结果中的内容明显较为复杂，不能直接认定这些软件全部运行在同一台服务器上。  
这种情况可能与原始响应内容、数据采集、指纹识别或平台展示方式有关。仅凭当前截图无法确定具体原因，还需要核对原始 HTTP 响应。  

Cookie 与其他响应头：  
结果中还出现了 set-cookie、x-cache、x-generator 和 x-jenkins 等字段。  
其中，set-cookie 用于要求浏览器保存 Cookie；x-cache 通常用于表示缓存处理情况；x-generator 可以提供网站生成工具的线索；x-jenkins 则可能暴露与 Jenkins 相关的技术信息。  
这些字段可以帮助分析服务使用的技术和部分配置特征，但字段的存在并不能直接证明目标存在漏洞。  

3.    
  子域名收集  
①利用公开证书信息：  
网站在使用 HTTPS 时，可能会通过数字证书公开相关域名信息。可以查询公开的证书透明度记录，寻找与指定域名相关的子域名线索。   
②利用 DNS 信息:  
DNS 是域名系统，负责将域名解析为相应的网络地址。通过查询自己管理的域名的 DNS 记录，可以了解已配置的相关主机名和解析信息。  
③利用网络空间搜索引擎:  
ZoomEye 等平台可以用于查询与指定域名有关的公开资产信息。搜索结果可能包含主机名、IP 地址、端口和服务指纹等数据。  
![子域名搜索](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/subdomain%20search.png)
通过对查询结果进行整理，可以进一步了解域名关联的公开服务。不过，历史数据可能已经过时，查询到的 IP 地址也可能属于 CDN 或其他代理服务，不能直接认定为网站的真实源服务器。  





