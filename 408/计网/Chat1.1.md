# 1.1计算机网络概述

#### 1.计算机网络组成

* 从组成部分上看分为 硬件，软件，协议
* 从功能组成上看分为通信子网和资源子网

#### 2.计算机网络的功能

* **数据通信**，资源共享，分布式处理，提高可靠性，负载均衡

#### 3.计算机网络分类

* WAN,MAN,LAN,PAN，广域网，城域网，局域网，个人区域网

> 广域网使用交换技术，局域网和城域网使用广播技术，广域网和局域网的链接通过路由器互联实现的,以太网是局域网技术

* 拓扑结构上来看广域网是网状结构
* 广播式网络不需要网络层，不存在路由选择，但数据链路层使用物理层的服务必须通过服务访问节点来实现
* 按照交换技术分类为 电路交换，报文交换，分组交换

> 报文交换是一个整体的传输，所以说大小是不一定的，而分组交换相当于对此进行了标准化以及分块化，降低了平均所占缓冲区大小，也是当今的主流

#### 4.性能指标

* 带宽(最大可传输) 吞吐率(实际传输) 
* 时延分为：发送时延，传播时延，处理时延(交换节点进行差错处理的时间),排队时延(中转站排队)




***

#### 易错点

* ARPAnet是最早的计算机网络，是因特网的前身
* 局域网和广域网之间连接通过路由器
* 设带宽为b，数据大小为x，分组为n，一共k条链路，每个传播时延为d，报文启动s，那么

> 报文总时延 $s+x/b+kd$
>
> 分组总时延 $kd + (k-1)p/b+np/b$
>
> 所以说传播时延一般放一起算，但是发送时延牵涉到分组的情况下，需要按照思想重新算