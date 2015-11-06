---
layout: post
title: hex format in mac
author:qfai
tags:others

---
## the way of edit and look hex code in mac[^1]
---
[^1]: qfai  <404630507@qq.com>

###1. use terminal

there is a commend name xxd.

typically use  *xxd out.txt>out2.txt*, the second file will be write in a hex format

###2. use vim


1. 首先以二进制方式编辑这个文件vi -b datafile
2. 使用xxd转换为16进制:%!xxd文本看起来像这样:

```       
0000000: 1f8b 0808 39d7 173b 0203 7474 002b 4e49  ....9..;..tt.+NI     
0000010: 4b2c 8660 eb9c ecac c462 eb94 345e 2e30  K,.`.....b..4^.0     
0000020: 373b 2731 0b22 0ca6 c1a2 d669 1035 39d9  7;'1.".....i.59. 
```

现在你可以随心所欲地阅读和编辑这些文本了。 Vim 把这些信息当作普通文本来对待。

3. 转换16进制回来vi:%!xxd -r
4. 保存:wq

###3. by the way
a useful tutorial of kd-tree is [here](http://blog.csdn.net/qll125596718/article/details/8426458)



