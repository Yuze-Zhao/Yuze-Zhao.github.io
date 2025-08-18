---
layout: page
permalink: /blogs/approximationtheory/index.html
title: approximationtheory
---

## Determine that \(\int_{-1}^1 f(x)\, dx = A_0x_0 + A_1x_1\) has the highest algebraic degree of precision

We only need to solve the system of equations:

$$
\begin{cases}
A_0 + A_1 = b - a = 2, \\
A_0x_0 + A_1x_1 = 0
\end{cases}
$$

Substituting $x_0 = -1,\ x_1 = 1$ , it is clear that we obtain $A_0 = A_1 = 1$ .

Thus, the integration formula is the trapezoidal rule, which matches our expectation. Its algebraic degree of precision is only 1. If we suppose the algebraic degree of precision $m > 1$ , then we would have to satisfy:

$$
\begin{cases}
A_0 + A_1 = 2, \\
A_0x_0 + A_1x_1 = 0, \\
A_0x_0^2 + A_1x_1^2 = \tfrac{2}{3}
\end{cases}
$$

It is evident that this system has no solution. Therefore, we conclude that this quadrature formula attains the highest possible algebraic degree of precision.