单独输入'，页面会报错，提示You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near ''''' at line 1   
判断为字符型注入  
输入 ' or '1'='1，点击查询，如图所示，获得了所有人的信息  
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/%E5%AD%97%E7%AC%A6%E5%9E%8B%E6%B3%A8%E5%85%A51.png)  
剩下的步骤就和数字型注入一样了，通过构建payload来获得用户名和密码  
