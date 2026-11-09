在输入框中输入' onclick=alert('xss')>  
其数据来源变成了 URL 参数  
地址栏的内容也变成了http://127.0.0.1/pikachu/vul/xss/xss_dom_x.php?text=%27onclick%3Dalert%28%27xss%27%29%3E  
这意味着，攻击者只需要构造一个带有恶意 payload 的链接，发给受害者，受害者只要点开这个链接，不需要任何额外操作，XSS 就会自动触发  
