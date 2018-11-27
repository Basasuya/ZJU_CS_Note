# 4.3磁盘组织与管理

#### 1.磁盘结构

* 柱面，磁道(一圈)，扇区(圆心角)

#### 2.磁盘调度算法

* 磁盘调度算法分为FCFS，SSTF(最短寻道),SCAN(走到底再返回)，C-SCAN(走到底再从头来),LOOK(和SCAN一样，但是后面没有就不走了),CLOOK


* 磁盘读取时间一般分为下面几个部分，寻找时间，延迟时间，传输时间
* 当磁头读完一部分的时候，会超出下一个的一半，这也是为什么经常旋转延迟需要一般的周期时间
* 旋转延迟是$\frac{T}{2}$,读取延迟为$\frac{T}{n}$