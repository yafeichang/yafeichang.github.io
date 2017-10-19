### Linux下使用远程ssh命令运行其他机器上的代码

想在机器A上远程运行机器B上的一条命令，如运行B上的ls，则可使用命令：

`cyf@A:~$ ssh cyf@B 'ls'`

如果想在机器A上远程运行机器B上的多条命令，可使用分号将多条命令分开，如：

`cyf@A:~$ ssh cyf@B 'cd test; ls'`

当然也可以运行机器B上的shell脚本，如机器B上的cyf用户目录下有一个test.sh的脚本，则可以：

`cyf@A:~$ ssh cyf@B './test.sh'`

或

`cyf@A:~$ ssh cyf@B 'bash test.sh'`

但是在远程运行机器B上的java程序Test的时候，出现了问题：

`cyf@A:~$ ssh cyf@B 'java Test'`

提示

`bash: java: 未找到命令`

而直接ssh cyf@B之后，再运行java Test正常

如果执行

`cyf@A:~$ ssh cyf@B ‘env’`

会发现没有java环境变量

这是因为ssh执行命令时是个短链接，没有打开终端，所以不会去加载**.bashrc**环境变量从而导致不识别java命令

解决方法：修改***/etc/environment***，在其中添加java路径

`PATH="usr/local/sbin:/usr/local/bin:/sbin:/bin:/usr/sbin:/usr/bin:/usr/local/jdk/bin"`

再次执行java程序Test，发现可以了

[^关键字]: Linux; ssh; 远程命令; Java; ash