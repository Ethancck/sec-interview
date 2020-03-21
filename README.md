# sec-interview
以下为信息安全各个方向涉及的面试题，星数越多代表问题出现的几率越大，没有填答案是希望大家如果不懂能自己动手找到答案，祝各位都能找到满意的工作:)

注:做这个List的目标不是全，因为无论如何都不可能覆盖所有的面试问题，更多的还是希望由点达面，查漏补缺。

## TODO LIST

- [x] Web安全
- [x] PHP安全
- [ ] Java安全
- [x] Linux相关
- [ ] Windows相关
- [ ] 内网渗透
- [x] 安全研发
- [ ] 甲方安全运营

## Web安全相关

- 介绍一下自认为有趣的挖洞经历（或CTF经历）(★★★)
- CSRF的成因及防御措施（不用token如何解决) (★)
- SSRF的成因及防御措施 (★★)
- SSRF如何探测非HTTP协议(★)
- 简述一下SSRF的绕过手法(★★)
- 简述一下SSRF中DNSRebind的绕过原理及修复方法(★)
- 介绍 SQL 注入漏洞成因，如何防范？注入方式有哪些？除了拖取数据库数据，利用方式还有哪些？(★★)
- 如何通过sql注入写shell,写shell的前提条件是什么?(★★)
- 介绍一下XSS漏洞的种类，dom型XSS和反射XSS的区别是什么?(★★)
- 如何防范 XSS 漏洞，在前端如何做，在后端如何做，哪里更好，为什么？(★★)
- 讲述一下找回密码可能涉及的逻辑漏洞(★)
- 假设你是甲方的一名安全工程师，应该如何降低逻辑漏洞的出现率?(★★)

## PHP安全

- PHP中如何使用`phar://`伪协议触发反序列化，利用场景以及前提条件有哪些?(★★)
- 如何绕过`php.ini`中`disable_function`的限制，有哪些方法，其中成功率最高的方法是哪个，为什么?(★★★)
- 文件上传中`%00`截断的原理是什么，官方是如何设计修复方案的?(★★)
- 实现一个一句话webshell，绕过RASP的方式有哪些，绕过机器学习检测的方式有哪些，绕过AST-Tree的方式有哪些(★★)
- PHP伪协议的攻击场景有哪些？(★★)

## 安全研发相关

- 简要介绍自己常用的扫描器和其实现上的特点(★★)
- 如果让你设计一个HIDS，应该如何设计(★)
- 介绍一下Python中的迭代器、生成器、装饰器(★)
- 介绍自己常用的python库(★)
- 讲一讲celery的特点以及原理(★)
- 简述Python中的GIL锁，以及如何打破GIL锁的限制(★★)
- masscan号称世界上最快的扫描器，快的原因是什么，如何实现一个自己的masscan?(★★)

## Linux相关

- Linux 中让命令在后台运行的方法有哪些？(★)
- 查看当前端口连接的命令有哪些？netstat 和 ss 命令的区别和优缺点 (★)
- Linux 服务器的安全运维操作有哪些？如何保护 SSH？(★★)
- 入侵 Linux 服务器后需要清除哪些日志？(★★)
- 反弹 shell 的常用命令？一般常反弹哪一种 shell？为什么？(★★★)
- 从主机的层面，反弹shell如何监控 (★★★)
- Rootkit的种类有哪些，针对不同种类的Rootkit应该如何防护以及检测 (★★)
- A账户创建了权限为766的文件夹`adir`，该文件夹中有B账户的文件`password.txt`，权限为B账户的700，请问B账户能否读取到`adir/password.txt`文件的内容


## 其他安全相关
- redis未授权访问如何利用，利用的前提条件是？(★★★)
- RSA加解密流程(★)
- HTTPS是如何实现的(★★)
- 如何防护运营商的DNS劫持/链路劫持(★★)
- 如何防范羊毛党？(★)
- 一个大范围影响的0day被曝光，作为甲方安全工程师，应该如何处理(★★)
- CSP应该如何使用及配置，有哪些绕过CSP的方式(★★)
