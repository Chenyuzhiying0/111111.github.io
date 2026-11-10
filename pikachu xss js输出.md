输入<scirpt>alert('xss')</script>提交后无反应  
查看sources发现其<script>的对应关系有问题  
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/xss%20js%E8%BE%93%E5%87%BA1.png)  
输入</script><script>alert('xss')</script>后提交  
其弹出警告弹窗  

输入';alert(`xss`);//后其出现弹窗  
第一个引号闭合了原本包裹变量的单引号  
第一个分号结束了原本的赋值语句 $ms='';  
第二个分号结束alert语句  
//把后端原本自带的那个结尾单引号（以及后面的代码）给注释掉了，防止页面报错
