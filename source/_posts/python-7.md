---
title: python(7)
date: 2020-10-28 09:35:39
tags:articles
---

### title:python 笔记（七）-模块

Welcome to [Hexo](https://hexo.io/)! This is your very first post. Check [documentation](https://hexo.io/docs/) for more info. If you get any problems when using Hexo, you can find the answer in [troubleshooting](https://hexo.io/docs/troubleshooting.html) or you can ask me on [GitHub](https://github.com/hexojs/hexo/issues).

> 昨日作业 代码参考

```bash
# 7、写函数，检查传入字典的每一个value的长度，如果大于2，那么仅仅保留前两个长度的内容，并将新内容返回给调用者
# dic = {“k1”: "v1v1","k2":[11,22,33]}
# ps:字典中的value只能是字符串或列表

def v_2(dic1):
#定义一个空字典
dic={}
#同步遍历字典的键和值
for k,v in dic1.items():
if len(v)>2:
dic[k]=v[0:2]
else:
dic[k]=v
return dic
dic={"k1": "v1v1","k2":[11,22,33]}
print(v_2(dic))

```

```bash
#5、写一个函数，传入一个字符串，求字符串中出现次数最多的字符
#定义函数
def count_str(str):
#字典用来存放 出现的字符 和 对应的次数
dic={}
for i in str:
#如果字符不在字典中，添加到字典中
if i not in dic:
#dic[i]是字符出现的次数，str.count(i)用来统计字符i出现的次数
#增加字符和次数
dic[i]=str.count(i)
#寻找字典中的值的最大值，也就是最大次数
max_count=max(dic.values())
for k,v in dic.items():
if v==max_count:
print("出现次数最多的字符是",k,"出现的次数为",v)

str=input("请输入字符串:\n")
count_str(str)
```
