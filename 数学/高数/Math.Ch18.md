# 第十八章 第二型曲线积分 第二型曲面积分

* 特别注意，对于这种积分的区间是否为0的判断，必须要将所有变量转化为正规变量(dxdy之内的)，按照点的轨迹判断正负，尽可能多的进行分割积分

#### 1.第二型曲线积分

* 物理意义上是**有方向**的变力做功，所以积分一定要从物理意义上分段积分
* 不具有轮转对称性，具有平常相反的**奇偶性**，方向上来说，逆时针为正
* 计算方法有直接计算和格林公式

> $\int Pdx + Qdy + Rdz = \int P*x'_{t} +  Q*y'_{t} +  R*z'_{t}dt$
>
> 二维格林公式 $\int Pdx+Qdy = \iint \frac{\sigma Q}{\sigma x}-\frac{\sigma P}{\sigma y}d \sigma$
>
> 三维斯托克公式 $\int Pdx + Qdy + Rdz = \iint |\matrix{dydz & dzdx & dxdy \\ \frac{\sigma}{\sigma x} &  \frac{\sigma}{\sigma y} &  \frac{\sigma}{\sigma z} \\ P & Q &R} |$
>
> 必须保证P,Q,R在片内连续才可以使用这两个公式，所以必须学会如何进行**补片**

* 曲面积分与路径无关理论

> 平面单连通区域相比平面有界区域多了一个$\frac{\sigma P}{\sigma y}=\frac{\sigma Q}{\sigma x} $处处成立

#### 2.第二型曲面积分

* 物理意义是向量函数通过邮箱曲面的通量
* 不具有轮转对称性，具有相反的奇偶性，方向上来说，与坐标轴方向相同为正，外部为正
* 计算方法有直接计算，高斯公式，，一二型转化

> $\iint R(x,y,z)dxdy=\pm \iint R(x,y,z(z,y))dxdy \quad \iint R(x,y,z)dxdz=\pm \iint R(x,y,z(z,y))(-\frac{\sigma z}{\sigma x})dxdy$
>
> $\iint Pdydz+Qdxdz+Rdxdy = \iiint\frac{\sigma P}{\sigma x} +\frac{\sigma Q}{\sigma y}+\frac{\sigma R}{\sigma z}dv$
>
> $\iint Pdydz+Qdxdz+Rdxdy = \iint (Pcosa + Qcosb + Rcosc)dS$