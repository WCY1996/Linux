
目录 | 应放置文件内容
---|---
/usr/X11R6/ |为X Windows系统重要数据所放置的目录，之所以取名为X11R6是因为最后的X版本为第11版，且该版的第6次释出之意
/usr/bin/ | 绝大多数的用户可使用命令都放在这里。请注意到它与/bin的不同之处（是否与开机过程有关）
/usr/include/ | C/C++等程序语言的头文件（header）与包含文件（include）放置处，当我们以tarball方式（*.tar.gz的方式安装软件）安装某些数据时，会使用到里头的许多包含文件
/usr/lib/ | 包含各应用软件的函数库、目标文件（object file），以及不被一般用户管用的执行文件或脚本（script）。某些软件会提供一些特殊的命令来进行服务器的设置，这些命令也不会经常被系统管理员操作，那就会摆放到这个目录下。要注意的是，如果你是要的是X86_64的Linux系统，那可能会有/usr/lib64/目录产生
/usr/local/ | 系统管理员在本机自行安装自己下载的软件（非distribution默认提供者），建议安装到此目录，这样会比较便于管理。举例来说，你的distribution提供的软件比较久，你想安装新的软件但又不想删除旧版，此时你可以将新版软件安装于/usr/local/目录下，可与原先的旧版软件有区别。你可以自行到/usr/local去看看，该目录下也是具有bin，etc，include，lib的子目录
/usr/sbin/ |非系统正常运行所需要的系统命令。最常见的就行某些网络服务器软件的服务命令（daemon）
/usr/share/ | 放置共享文件的地方，在这个目录下放置的数据几乎是不分硬件架构均可读取的数据，因为几乎都是文本文件。在此目录下常见的还有这些子目录：/usr/share/man:在线帮助文件 /usr/share/doc:软件杂项的文件说明 /usr/share/zoninfo:与时区有关的时区文件
/usr/src/ | 一半源码建议放置到这里，src有source的意思。至于内核源码则建议放置到/usr/src/linux/目录下