先F12检查，在密码框代码的下边，发现进行验证的token  
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/token%E9%98%B2%E7%88%86%E7%A0%B41.png)  
对于有token的的验证，适用于已经知道账号的情况，或者账号和密码一一对应的情况  
攻击目标选择password以及token，攻击方式选择Pitchfork    
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/token%E9%98%B2%E7%88%86%E7%A0%B42.png)  
来到payloads模块,password设置和之前一样，上传爆破字典  
接着来到Settings模块，往下滑找到Gerp-Extract  
点击add，接着选中token  
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/token%E9%98%B2%E7%88%86%E7%A0%B43.png)  
再回到payloads模块，在第二个位置处选择Secursive grep，并将token粘贴到下面的框里  
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/token%E9%98%B2%E7%88%86%E7%A0%B44.png)  
开始攻击即可
