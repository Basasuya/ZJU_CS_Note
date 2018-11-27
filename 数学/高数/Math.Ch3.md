# 第三讲 一元微分学

#### 1.导数概念 

>  $f'(x_{0}) = lim_{x \to 0}\frac{f(x_{0}+\Delta x)-f(x_{0})}{\Delta x}$ ，涵盖了两边都可导，也就是说这个$\Delta x$必须可正可负的，比如$x^{2}$就不行

* 仅当极限存在时，称函数在$f(x)$在$x_{0}$可导

> $f'_{-}(x_{0}) = lim_{x \to 0^{-}}\frac{f(x_{0}+\Delta x)-f(x_{0})}{\Delta x}$

> $f'_{+}(x_{0}) = lim_{x \to 0^{+}}\frac{f(x_{0}+\Delta x)-f(x_{0})}{\Delta x}$

* 两侧导数皆存在并相等才意味着可导，可导也意味着原函数连续(但是反过来就不行)

#### 2.微分概念

> $\Delta y = A \Delta x + o(\Delta x)$ 

* $A$是与$x$无关的常数，$o$是$\Delta x \to 0$的比$\Delta x$高阶的无穷小

> $\Delta y = f(x_{0} + \Delta x)-f(x_{0})$ 
>
> $A = f'(x_{0})$
>
> $lim_{\Delta x \to 0}\frac{\Delta y - A \Delta x }{\Delta x}$ 极限趋向于0，说明此点可微

* 可微与可导互为充要条件(仅限一元函数)




***

* 导数存在，则函数必连续，


* 左右导数 和 导数的左右极限不一样，左右导数才是该点可导

> $f'_{-}(x_{0}) \quad \lim_{x \to x_{0}^{-}}f'(x)$