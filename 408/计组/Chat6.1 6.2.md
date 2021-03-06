# 6.1概述

#### 1.总线概念

* 分时 一个时刻允许一个部件向总线发送信息
* 共享 总线上可以挂接多个部件
* 使用总线结构减少了信息传输的条数
* 地址线用于指定内存以及I/O设备接口电路的地址

#### 2.总线的分类

* 片内总线，CPU内部寄存器与ALU的总线
* 系统总线： 数据总线，地址总线，控制总线
* 通信总线，计算机系统之间的线路

#### 3.系统总线结构

* 单总线，双总线(I/O分开)，三总线(I/O，DMA，主存总线)


> 单总线不是只有一条线，下面还是可以细分为数据，地址，控制

* 突发传输:一个总线周期里面可以传输多个存储地址的数据
* 并行传输:多个数据位同时在设备之间进行传输
* 串行传输:指数据以位为单位按时间顺序进行逐位传输
* 同步传输:按照同一个时钟周期进行传输






***

#### 易错点

* 总线的数据线上不可能发生 握手信号的传输
* $kb = 1000b$
* 单周期处理器不能使用单总线结构



# 6.2总线仲裁

#### 具体看p246的表，一清二楚

* 链式查询3,设备允许，设备请求，总线忙，计数器定时查询log2n+2，无总线允许线，有设备地址线，独立请求，2*n+1,只有一个根总线忙线


* 计数器定时查询方式有两种变种，第一种每次从0开始计时，那么这样的话设备优先级是固定的，第二种是从上次结束的地方开始计数，那么优先级是随机的
* 总线忙的建立者是活得总线控制权的设备