# Math.Chapter1



#### 1.函数概念

* 函数基本概念

> $f[x] = y \quad x\in N$
>
> $R = \{ y = f(x), x \in N  \}$

x 为自变量，y因变量，N定义域，R值域，f对应法则

* 反函数

> $y = f(x) \quad x = f^{-1}(y)$

第一，原函数的单调性无法保证反函数单调性，如$y = x^2$

第二，原函数与反函数在图像中关于 $y = x$ 对称

* 复合函数

> $y = f[g(x)] \quad x \in D$

* 基本初等函数

> $y = x^u$
>
> $y = a^x (a > 0, a \neq 1)$
>
> $y = log_{a}^{x}  (a > 0, a \neq 1)$
>
> $sinx \quad cosx \quad tanx \quad cotx$
>
> $sex(x) = \frac{1}{cosx}$
>
> $csc(x) = \frac{1}{sinx}$
> $arcsinx \quad arccosx \quad arctanx \quad arccotx$

* 其他函数模型

分段函数

> $U = max\{f(x), g(x)\} \quad V = min\{f(x), g(x)\}$
>
> $U = \frac{1}{2}[f(x)+g(x)+|f(x)-g(x)|] \quad V = \frac{1}{2}[f(x)+g(x)-|f(x)-g(x)|]$

幂指函数

> $u(x)^{v(x)} = e^{v(x)lnu(x)}$



#### 2.函数四种特性

* 有界性

> 设$f(x)$定义域为$D$，并且$I \subset D$ 如果存在某个**正数**M满足，对任意$x \in I, |f(x)|\leq M$ 则称$f(x)$在$I$有界

* 单调性

> 设$f(x)$定义域为$D$，并且$I \subset D$ 如果对于区间$I$上的任意两点满足当，$x1<x2$ 恒有 $f(x1) < f(x2)$
>
> 则称$f(x)$ 在$I$上递增，反之亦然
>
> 注意往往也有定义法解决单调性问题，如
>
> $(x1-x2)[f(x1)-f(x2)]>0$   f(x)是单调增函数

* 奇偶性

> $F(x) = f(x)-f(-x)$ 奇函数 $F(x) = f(x)+f(-x)$ 偶函数

* 周期性

> $f(x+T) = f(x)$



#### 3.常用基础知识

> $\sum_{k=1}^{n}k^{3} = [\frac{n(n+1)}{2}]^{2}$

> $\sin^{2} 2x = \frac{1}{2}(1-\cos2a) \quad \sin^{2} 2x = \frac{1}{2}(1+\cos2a)$ 



#### 4.泰勒公式

> $e^{x} = \sum^{\infty}_{n=0}\frac{x^{n}}{n!}$
>
> $\frac{1}{x+1} = \sum^{\infty}_{n=0}(-1)^{n}x^{n}$
>
> $\frac{1}{1-x} = \sum^{\infty}_{n=0}x^{n}$
>
> $ln(x+1) = \sum^{\infty}_{n=1}\frac{(-1)^{n-1}x^{n}}{n}$
>
> $sinx = \sum^{\infty}_{n=1}\frac{(-1)^{n-1}x^{2n+1}}{(2n+1)!}$ $arcsinx = \sum^{\infty}_{n=1}\frac{x^{2n+1}}{(2n+1)!}$
>
> $cosx = \sum^{\infty}_{n=0}\frac{(-1)^{n}x^{2n}}{(2n)!}$
>
> $tanx = \sum^{\infty}_{n=0}\frac{x^{2n+1}}{2n+1}$ $arctanx = \sum^{\infty}_{n=0}\frac{(-1)^{n-1}x^{2n+1}}{2n+1}$
>
> $(1+x)^{a} = \sum^{\infty}_{n=0}\frac{x^{n}*a!}{n!*(a-n)!}$