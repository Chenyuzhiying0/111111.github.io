在框内随便输入数据，然后使用burpsuite进行拦截  
将name=后面的内容改为  
1%df' or 1=1 #  
当输入一个'时程序会自动在前面加一个反斜杠  
有些汉字的第一个字节刚好是%df  
\被转义成了%5c  
%df和%5c共同组成了一个汉字  
这样单引号就成功逃逸了  
这样即可显示所有的数据  
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/wide%20byte%E6%B3%A8%E5%85%A51.png)  
剩下的操作就和之前一样了
