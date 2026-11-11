使用kobe账号登录网页，然后点击修改个人信息，使用burpsuite进行拦截  
将拦截到的东西发送到repeater  
右键点击engagement tools，然后选中Generate CSRF PoC  
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/CSRF(get)1.png)  
修改内容，然后点击copy html  
将内容复制到记事本里并将后缀改为html  
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/CSRF(get)2.png)  
此时切换为lucy账号  
如图所示，目前的信息如下  
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/CSRF(get)3.png)  
点击生成的html  
此时查看lucy的账号，发现其信息已经被修改  
![!](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/CSRF(get)4.png)  
此时lucy的邮箱已经变成kobe的了  
