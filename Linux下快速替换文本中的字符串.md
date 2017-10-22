## Linux下快速替换文本中的字符串

### 替换单个文本中的所有字符串

方法1：

1. 使用vim打开文本文件

   `cyf@ubuntu:~$ vim test.txt`

2. 使用vim中的替换命令
  `:%s/原字符串/替换字符串/gg`

方法2：

`cyf@ubuntu:~$ sed -i 's/原字符串/替换字符串/g' filename //替换文件中的所有匹配项`

### 替换文件夹下所有文本中的字符串
```
cyf@ubuntu:~$ sed -i 's/原字符串/替换字符串/g' `ls | grep -E 'test.txt'`
```

