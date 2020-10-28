---
title: Hello World
---
Welcome to [Hexo](https://hexo.io/)! This is your very first post. Check [documentation](https://hexo.io/docs/) for more info. If you get any problems when using Hexo, you can find the answer in [troubleshooting](https://hexo.io/docs/troubleshooting.html) or you can ask me on [GitHub](https://github.com/hexojs/hexo/issues).

## Quick Start

### Create a new post

``` bash
$ hexo new "My New Post"
```

More info: [Writing](https://hexo.io/docs/writing.html)

```

import math
#1、s=”fdfdfds@#@#234”,以#符号为标准，将字符串分隔成两部分
s = "fdfdfds@#@#234"
print(s.split('#',1))

#2、字符串拆分的方法有哪些，请比较异同
'''
partition:不能不传入参数 ，返回是元组
splitlines：不传输参数，默认以\n分割 传入参数，keepends=True 取到\n 默认keepend = False 返回列表类型
split：不传输参数，默认以空格分割，传入参数，返回列表类型
'''

#3、字符串查找的方法有哪些，请比较异同
'''
find:返回从左第一个指定字符的索引，找不到返回-1
rfind:返回从右第一个指定字符的索引，找不到返回-1
index:返回从左第一个指定字符的索引，找不到报错
rindex:返回从右第一个指定字符的索引，找不到报错

'''
#4、统计字符串中出现的单词个数
#str = "This is my brother"
str4 = "This is my brother"
print(len(str4.split(' ')))

#5、键盘录入字符串并遍历输出所有元素（用两种遍历方式）
str5 = 'abcdefghijklmnopqrstuvwxyz'
for i in str5:
    print(i,end=' ')
print()
for i in range(len(str5)):
    print(str5[i],end='~')
print()
#6、倒叙输出字符串‘1234567’，
str6 = '1234567'
print(str6[-1::-1])
#7、取出字符串 ‘123456789’中所有的奇数
str7 = '123456789'
print(str7[0:len(str7):2])

#8、使用for循环输出字符串‘123456789’中所有的偶数
for i in range(0,9,2):
    if i==0:
        continue
    else:
        print(i,end=' ')
print()
#9、将字符串‘this is test text test text test’中的前两个‘test’替换为’new_test’
str9 = "this is test text test text test"
print(str9.replace('test','new_test',2))

#10.判断一个数是否是回文数。例如：输入：121，输出也是121，像这样的数就是回文数
str10 = str(input('输入一个数，判断是否是回文:'))
Fstr10 = str10[len(str10)::-1]
if str10 == Fstr10:
    print(str10+'是回文数')
else:
    print(str10+'不是回文数')

#11、用format 的位置参数和关键字参数实现打印输出一段自我介绍，包括姓名，年龄，爱好
#位置参数
strName = 'xiaoming'
strAge = 24
strHobby = '爬山'
str11 = '我叫{},我今年{},我的爱好是{}'
print(str11.format(strName,strAge,strHobby))
# 关键字参数
msg = '大家好，我的姓名是{name},我的年龄是{age},我的爱好是{hobby}'
print(msg.format(name= 'xiaofang',age=21,hobby = '游泳'))
print()
#12、圆的半径是3/5，求圆的面积和周长，保留两位小数（使用format方法）
r = 3/5
mj=math.pi*r*r
zc=2*math.pi*r

print('圆的面积是{:.2f},圆的周长是{:.2f}'.format(mj,zc))
"""
#13、打印以下购物单
str13 = '菜单,苹果,水饺,可口可乐(1.25L),银桥酸奶(袋装),大地猫锅巴'.split(',')
num13 = '价格,20.00,10.50,11.50,1.00,2.50'.split(',')
print('='*35)
count = 0
for str,num in zip(str13,num13):
    s = 35-len(num)-len(str)
    if count==1:
        print ('-'*35)
    print(str+'%-4d' % num)
    count+=1
print('='*35)
```


