# 第二章 极限

#### 1.函数极限意义

* 定义

> 设函数$f(x)$在点$x _{0}$的某一**去心领域**内有定义，若存在常数$A$,对于任意给定的$\epsilon>0$(不管它多小)
>
> 总存在正数$\delta$,使得当$0<|x-x_{0} |< \delta$时，对应的函数值$f(x)$都满足不等式$|f(x)-A|<\epsilon$,
>
> 则A就叫做函数$f(x)$当$ x\rightarrow x_{0}$ 时的极限，记为
>
> $ \lim_{x\rightarrow x_{0}f(x)=A}$ 或 $f(x) \rightarrow A(x \rightarrow x_{0})$ 

* 极限存在的充要条件

> $ \lim_{x \rightarrow x_{0}}f(x)=A \Leftrightarrow \lim_{x \rightarrow x_{0}^{-}}f(x)=A$ ,且$\lim_{x \rightarrow x_{0}^{+}}f(x)=A$ 

* 函数极限性质

> 局部有界性：如果$ lim_{x \rightarrow x_{0}}f(x)=A$，则存在正常数$M$和$\delta$使得 $0<|x-x0|< \delta$ 有$|f(x)|\leq M$

> 局部保号性：如果$ f(x) \rightarrow A(x \rightarrow x_{0})$ ，且$A>0(or A<0)$ 那么存在常数$\delta$ 有$0<|x-x_{0}|< \delta$,
>
> 有$ f(x)>0(or f(x)<0)$



#### 2.求极限技巧

* 洛必达原理

> 必须分子分母同为无穷大或者无穷小，这是先觉条件

* 等价无穷小(只能在乘除里面用)

> $sin \sim x \quad tanx \sim x \quad arcsinx \sim x \quad arctanx \sim x \quad ln(1+x) \sim x \quad $
>
> $e^{x}-1 \sim x \quad a^{x}-1 \sim xlna \quad 1-cosx \sim \frac{1}{2}x^{2} \quad (1+x)^{a}-1 \sim ax \quad log_{a}^{(1+x)} = \frac{ln(1+x)}{lna} \sim \frac{x}{lna}$

* 等价代换

> 变量代换$ 0 \to \infty$ ；分子有理化；当$x \to \infty$对于化成$\frac{1}{x}$形式
>
> $\infty^{0}/ 0^{0}:e^{vlnu}$   |   $1^{\infty}:e^{(u-1)v}$

* 泰勒公式（一般需要凑次数）
* 夹逼定理

> $1*u_{max}\le F \leq n*u_{max}$当元素差异化很大的时候
>
> $n*u_{min}\le F \leq n*u_{max}$

* 分解法解题   $lim(A+ B) = limA + limB \quad lim\frac{A}{B} = \frac{limA}{limB} \quad limAB = limA*limB$ 

>  必须A，B极限存在，所以可以分解法来计算有些极限(极限不存在先洛必达几次就存在了)

####3 数列
* 数列的收敛性证明有两种，证明递减有下界，或者递增有上届

#### 易错点

* $ lim_{x \to a} h(x) = null \quad lim_{x \to a}g(x)=null$ 推不出 $lim_{x \to a}(h(x)*g(x)) = null$

> 比如$ h(x) = x>0?1:-1 \quad g(x)=x>0?-1:1$

* $ \infty*0$是未定式
* $lim_{x \to x_{0}}f(x)>lim_{x \to x_{0}}g(x) \Rightarrow \exists \phi>0,0<|x-x_{0}|<\phi,f(x)>g(x)$
* $\exists \phi>0,0<|x-x_{0}|<\phi,f(x)>g(x),lim_{x \to x_{0}}f(x) \exists,lim_{x \to x_{0}}g(x) \exists \Rightarrow lim_{x \to x_{0}}f(x)\ge lim_{x \to x_{0}}g(x) $

> 这个式子的关键在于$lim_{x \to x_{0}}f(x) = lim_{x  \to {x_{0}}}g(x)$时候的$f(x)$,$g(x)$的大小关系在领域是不知道的，所以在一个结论中等号就不能加

* $\exists x_{n},lim_{n \to \infty}x_{n}= x_{0},lim_{n \to \infty}f(x_{n})= \infty$