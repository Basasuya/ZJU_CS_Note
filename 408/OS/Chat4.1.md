# 4.1文件系统基础

#### 1.文件逻辑结构(一个文件内部关系)

* 无结构文件(流式文件)
* 有结构文件(记录式文件)

> 顺序文件，索引文件，索引顺序文件(这两个都是由索引表和逻辑文件组成的)，散列表
>
>  顺序文件相比流式文件而言，一种是以时间为单位的串形结构，一种是以关键字排列的顺序结构 

* 对于顺序文件 有n条记录，平均访问量为$n/2$
* 索引顺序文件n条记录，平均访问量为$\sqrt n/2$

#### 2.目录结构(文件之间的关系)

* 文件逻辑结构是一个文件内部的内容，而目录结构是文件的排布规律
* 文件的信息储存在fcb里面，文件的索引结构存储在索引节点

> 在unix当中，会把一些不太重要的信息存储在索引节点上，索引节点一起存在另外的地方

* 目录结构分为 单层目录结构，二层，多层目录结构(unix)

#### 3.文件共享

* 硬连接产生直接连接，软连接产生相对地址，还需要一步一步找，所以硬连接的速度会更快
* 目录和文件可以产生链接
* 硬链接 +:所有加1 -:所有减1
* 软链接 +:直接复制 -:不变

#### 4.文件保护

* 通过口令保护，加密保护，访问控制
* 对于文件的访问通常有 文件访问权限和文件属性 共同决定
* 文件受损经常使用备份的方法进行保护
* 访问控制必须由系统实现，而加密保护一般由用户实现，更有灵活性




***

#### 易错点

* 打开文件是将文件放入目录库，读取文件才会将文件内容写入目录
* 文件系统的目的是为了实现对文件的按名存取
* 输入输出文件是 特殊文件
* 文件系统采用多级目录是为了解决命名冲突 