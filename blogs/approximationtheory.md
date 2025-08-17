---
layout: page
permalink: /blogs/approximationtheory/index.html
title: approximationtheory
---

## 确定 $\int^1_{-1}f(x)\ dx=A_0x_0+A_1x_1$ 拥有最高的代数精度

只需要解决方程

$$
\begin{cases}
A_0+A_1=b-a=2\\
A_0x_0+A_1x_1=0
\end{cases}
$$

带入 $x_0=-1,\ x_1=1$ 显然可以解出 $A_0=A_1=1$ 。

积分公式为梯形积分公式，符合我们的期望，它的代数精度只有1。若代数精度 $m>1$ ，

$$
\begin{cases}
A_0+A_1=2\\
A_0x_0+A_1x_1=0\\
A_0x_0^2+A_1x_1^2=\frac 2 3
\end{cases}
$$

易见该方程是无解的。至此证明了该积分公式具有最高的代数精度。