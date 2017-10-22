## Ubuntu命令终端查看使用过的命令

1. 使用**history**命令

   `cyf@ubuntu:~$ history`

   但是这样会显示出所有使用过的命令，可以在history后加上less

   `cyf@ubuntu:~$ history | less`

   会显示出类似vim编辑器的形式，再使用类vim中的操作，查找使用过的命令

   `:/sed	//查找使用过的sed相关的命令`

   也可以直接使用**grep**进行过滤

   `cyf@ubuntu:~$ history | grep 'sed‘`

2. 在命令终端中按**Ctrl+R**，系统会提示：

   `(reverse-i-search)：`

   现在你输入“sed”，可能会提示：

   ```
   (reverse-i-search)`sed': sed -i 's/old/new/g' test.txt
   ```

   按下回车键，命令会自动变成`"sed -i 's/old/new/g' test.txt"`并开始执行。

3. 可以用**上下键**来切换最近输入的命令，按回车也可以执行。