# 3.5 介质访问

* 所谓划分是在半双工情况下考虑的，如果全双工，哪来的划分

#### 1.静态划分信道

* FDM(频分复用),TDM(时分复用),WDM(波分复用),CDM/CDMA(码分复用)
* FDM一般用于模拟信号，TDM一般用于数字信号
* 由于无法处理计算机系统的突发性，所以静态划分已经被动态划分所替代
* 码分多址(CDMA)复用，不同站的码向量互相正交，用复合向量和相应站的向量内积之后除以n就是相应的代码

#### 2.动态划分

* ALOHA(xjbc),时隙ALOHA(只能在每个时间块开始传输)
* CSMA 协议

> 1-坚持 CSMA(每个时间隙都侦测) 非坚持 CSMA(等随机时间再侦测) p-坚持 CSMA(每个时间隙都进行侦测，但是p概率进行传输)

* CSMA/CD

> 以太网端到端的往返时间称为争用期

> 最小帧长 = 总线传播时延 * 数据传输速率 * 2 

* 指数退避算法

> 在n次碰转之后，随机$[0,2^{n}-1]$的数k，按照2rk(r为单程周期)之后进行下次检测，n不会超过**10**

* CSMA/CA

> 发送数据之前先进行广播让其他节点不要进行传输

* CA,CD的区别，CA在发送的同时不能帧测信道上是否有冲突，CA主要用于无线局域网(全双工，一般不需要检测冲突)，CD主要用于以太网(有线局域网)
* 令牌传递协议

> 令牌在环形上游荡，有令牌的才能进行传输，适合负载高的网络





***

#### 易错点

* TDM要求介质的位速率大于单个信号的位速率
* 以太网规定最短帧长是64B
* CSMA/CA中含有ACK确认帧
* P96 3,4