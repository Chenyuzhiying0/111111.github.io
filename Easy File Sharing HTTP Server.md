--   
在物理机上打开简单文件HTTP服务器  
![easy file share](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/Easy%20File%20Sharing%20Web%20Server%20interface.png)   
<br>
<br>
<br>
<br>  

--   
在kali中 对物理机进行扫描 发现其80端口开放并且运行着Easy File Sharing Web Server   
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/nmap%20easy%20file%20sharing.png)   
<br>
<br>
<br>
<br>

--
启用Metasploit 搜索easy file sharing  
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/search%20easy%20file%20sharing.png)  
<br>
<br>
<br>
<br>

--   
使用exploit/windows/http/easyfilesharing_seh模块进行攻击 设置好RHOST LHOST 和 RPORT  
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/easyfilesharing_seh.png)  
<br>
<br>
<br>
<br>

--  
运行  
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/run%20easyfilesharing_seh.png)  
如图所示 已获得Meterpreter 实现了对目标主机的远程控制  
