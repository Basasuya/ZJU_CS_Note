# 5.1 传输层提供的服务

#### 1.传输层的功能

* 传输层提供进程之间的逻辑通信，是端口到端口的通信
* 分为有连接可靠传输TCP,无连接不可靠传输UDP

> TCP首部20字节，UDP首部字节8字节

#### 2.端口的作用

* 数据链路层的SAP是MAC地址,网络层的SAP是IP地址,传输层的SAP是端口
* 套接字是 由IP地址和端口组织的
* 熟知端口号0-1023,其他更大
* FTP 21 HTTP 80 SMTP 25 TELNET 23



# 5.2 UDP 协议

#### 1.UDP数据报

* 四个部分，源端口，目的端口，长度，校验和
* 校验和是用UDP首部和数据以及一些IP数据报的信息进行二进制反码相加而得，最后还需要取反