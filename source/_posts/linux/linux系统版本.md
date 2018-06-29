---
title: linux系统版本
date: 2018-06-19 14:17:02
categories:
- linux
---

稳定性 CentOS

界面好 Ubuntu

[Linux入门教程](http://www.92csz.com/study/linux/)


执行mongod时报错：

	/home/middleware/apphome/piccim/mongodb/bin/mongod: 
	error while loading shared libraries: libssl.so.10: 
	cannot open shared object file: No such file or directory

http://www.wanghualang.com/yum-error-libssl.html

https://blog.csdn.net/yifeng20xx/article/details/74896426

修改后继续报错
./bin/mongo: /lib64/libpthread.so.0: version `GLIBC_2.12' not found (required by ./bin/mongo)
./bin/mongo: /usr/lib64/libcrypto.so.10: no version information available (required by ./bin/mongo)
./bin/mongo: /usr/lib64/libssl.so.10: no version information available (required by ./bin/mongo)

[解决libc.so.6: version `GLIBC_2.14' not found问题](https://blog.csdn.net/cpplang/article/details/8462768)



