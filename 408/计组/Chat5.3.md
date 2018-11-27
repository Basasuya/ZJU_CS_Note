# 5.3 数据通路的功能和基本结构

* CPU的数据通路有三种类型，内部单总线，内部三总线，非内部专用数据通路，专用数据通路的效率更高的，但是代价也是最高的

#### 1.指令执行过程中的数据传输

* 注意一些常识比如 $(A) \to (B)$指的是A寄存器中的数存到B寄存器中的数为地址的地方上去
* 再比如$ADD R1, (R2)= (R1) + ((R2)) \to R1$ 


* 求执行阶段一般指的是间址周期和执行周期


* 取指周期

> $(PC) \to MAR  \quad PCout,MARin$
>
> $M(MAR) \to MDR \quad MeMR,MARout,MDRinE$
>
>  $(MDR) \to IR \quad MDRout,IRin$
>
> 指令译码
>
> $(PC)+1 \to PC$

* 间址周期，完成取数操作

> $(R_{0}) \to MAR \quad R0out,MARin$
>
> $M(MAR) \to MDR \quad MeMR,MARout,MDRinE$
>
> $(MDR) \to Y$

* 执行周期

> $(R1) + (Y) \to Z \quad R1out,ALUin,add$
>
> $(Z) \to MDR \quad Zout,MDRin$ 
>
> $(MDR) \to M(MAR) \quad MemR,MDRoutE$



***

* 学会画数据通路，简单来说就是数据流向的方向
* ad(IR)指的地址码
* 一个时钟周期总线只能被占有一次，但是比方说PC可以同时向总线发两个方向