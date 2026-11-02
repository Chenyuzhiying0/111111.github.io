--使用curl --version查看版本   
![curl --version](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/curl%20--vesion.png)    



--获取网页内容  
使用curl https://www.baidu.com命令  
![curl https](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/curl%20https.png)    



--获取 HTTP 响应头  
使用curl -I https://www.bilibili.com命令  
![curl -I](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/curl%20-I%20%20.png)    



--带参数的 POST 请求  
使用 httpbin.org 这个测试网站  
命令为curl -X POST https://httpbin.org/post -d "username=test&password=123"  
![curl -X POST](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/curl%20-X%20POST.png)    



--测试公开的 API 并格式化输出  
使用curl -s https://api.github.com/users/octocat命令  
![curl -s](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/curl%20-s.png)    
