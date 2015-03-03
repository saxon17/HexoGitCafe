title: law Spider
date: 2015-02-10 20:14:36
categories: python
tags:
---

<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width=330 height=86 src="http://music.163.com/outchain/player?type=2&id=387837&auto=1&height=66"></iframe>
#写的越快越好
```python
import urllib  
import urllib2  

url = 'http://www.someserver.com/register.cgi'  
  
values = {'name' : 'WHY',  
          'location' : 'SDU',  
          'language' : 'Python' }  

data = urllib.urlencode(values) # 编码工作
req = urllib2.Request(url, data)  # 发送请求同时传data表单
response = urllib2.urlopen(req)  #接受反馈的信息
the_page = response.read()  #读取反馈的内容
```