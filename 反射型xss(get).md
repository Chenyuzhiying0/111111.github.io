在输入框输入，发现其输入的最大长度为20  
按F12，找到mexlength，将其改为100  
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/%E5%8F%8D%E5%B0%84%E5%9E%8Bxss(get)1.png)  
返回输入框，输入<script>alert('xss')</script>，页面弹出了一个显示 "xss" 的警告框。
表明XSS漏洞存在  
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/%E5%8F%8D%E5%B0%84%E5%9E%8Bxss(get)2.png)  
