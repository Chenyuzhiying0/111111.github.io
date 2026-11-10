在两个框内输入<script>alert(document.cookie)</alert>来构建payload  
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/xss%E7%9B%B2%E6%89%931.png)  
输入完后点击提交  
之后访问http://127.0.0.1/pikachu/vul/xss/xssblind/admin_login.php 网址来登录后台  
输入用户名admin和密码123456进入  
进入后弹出了一个弹窗  
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/xss%E7%9B%B2%E6%89%932.png)  
表明xss漏洞存在  
