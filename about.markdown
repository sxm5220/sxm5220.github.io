---
layout: page
title: About
permalink: /about/
---

Eg:博客使用Jekyll（Blog生成器）

1.sudo gem install jekyll 2.sudo gem install jekyll bundler 3.新建Blog 运行jekyll new xxx(Blog名字) 4.进入xxxBlog目录下 运行 sudo jekyll serve （如果运行失败查看 sudo jekyll serve --trace，遇到的提示是： Address already in use - bind(2) for 127.0.0.1:4000 (Errno::EADDRINUSE)，说明端口被占用） 解决方法：1.查看4000端口举例：查看占用4000端口的服务 sudo lsof -wni tcp:4000

结果如下： COMMAND PID USER FD TYPE DEVICE SIZE/OFF NODE NAME ruby 15149 Yunis 8u IPv4 0xb0723eb7e38e11c5 0t0 TCP 127.0.0.1:terabase (LISTEN)

杀掉占用端口的进程（sudo kill -9 PID） sudo kill -9 15149

再次启动 jekyll 服务正常

5.本地运行起来后会看到 Server address: http://127.0.0.1:4000/ 6.浏览器中运行http://127.0.0.1:4000/ 就会看到新建Blog
