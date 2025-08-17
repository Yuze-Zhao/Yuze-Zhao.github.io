---
layout: page
permalink: /blogs/Fubini/index.html
title: Fubini
---

## Definition 
$x^j=(x_1,\dots,x_{j-1},x_{j+1},\dots,x_n)\in\mathbb R^{n-1}$ .
### Indices
Let $n\geq 2$ ,

$$0<p\leq \infty,\quad 1<q\leq \infty,\quad s>\sigma_p\ .$$

### Equivalent quasi-norm of $B^s_{pq}(\mathbb R^n)$
Let $0<p\leq\infty,\ 0<q\leq\infty$ and $s>\sigma_p$ . If $M$ is an integer such that $M>s$ , then

$$\|f|B^s_{pq}(\mathbb R^n)\|^{(1)}_M=\|f|L_p(\mathbb R^n)\|+\left(\int_{\mathbb R^n}|h|^{-sq}\sup_{\varrho\leq |h|,{\varrho\in\mathbb R^n}}\|\Delta^M_\varrho f|L_p(\mathbb R^n)\|^q\frac {\mathrm d h} {|h|^n}\right)^{\frac 1q}.$$

## Fubini Property for Besov and Triebel-Linzorkin spaces
Let $A^s_{pq}(\mathbb R^n)$ be either besov or triebel-Linzorkin spaces. Then  it has Fubini property if for all $f\in A^s_{pq}(\mathbb R^n)$ ,

$$\Vert f|A^s_{pq}(\mathbb R^n)\Vert\thicksim \sum^n_{j=1}\Vert{ \Vert f^{x^j}|A^s_{pq}(\mathbb R)\Vert|L_p(\mathbb R^{n-1})}\Vert.$$ 

## Theorem
The spaces $B^s_{pq}(\mathbb R^n)$ with indicies Fubini Property have the Fubini Property if, and only if, $p=q$ .

proof:
**step 1** We shall prove that another equivalent quasi-norm of $B^s_{pq}(\mathbb R^n)$ can be written as 

$$\|f|B^s_{pq}(\mathbb R^n)\|^{(1)}_M=\|f|L_p(\mathbb R^n)\|+\sum^n_{j=1}\left(\int_{\mathbb R}|h|^{-sq}\|\Delta^M_{h,j} f|L_p(\mathbb R^n)\|^q\frac {\mathrm d h} {|h|^n}\right)^{\frac 1q}.$$

According to Fubini Property and the Equivalent quasi-norm of $B^s_{pq}(\mathbb R^n)$ the second term of right-hand side, using polar coordinate transformation, can be written as 

$$\left(\int^\infty_0 r^{-sq}\sup_{|\varrho|\leq r}\|\Delta^M_\varrho f|L_p(\mathbb R^n)\|^q\frac {\mathrm d r}r\right)^\frac 1 q,$$

so it can be estimated from above by the supremum.

**step 2** Now we shall prove the other side, that is to say, we should prove there is a constant $c$ such that

$$\left(\int_{\mathbb R^n}|h|^{-sq}\|\Delta^{Mn}_h f|L_p(\mathbb R^n)\|^q\frac {\mathrm d h} {|h|^n}\right)^{\frac 1q}\leq c \sum^n_{j=1}\left(\int_{\mathbb R}|h|^{-sq}\|\Delta^M_{h,j} f|L_p(\mathbb R^n)\|^q\frac {\mathrm d h} {|h|^n}\right)^{\frac 1q}$$ 

holds for all $f\in B^s_{pq}(\mathbb R^n)$ .
There we use a special technique for decomposing. 

$$e^{ih\xi}-1=e^{ih_1\xi_1}-1+e^{ih_1\xi_1}(e^{ih_2\xi_2}-1)+\cdots+e^{i(h_1\xi_1+...+h_n\xi_n)}(e^{ih_n\xi_n}-1).$$ 

By taking Fourier transfomation of the above polynomial and reverse it, we can get 

$$\|\Delta^{Mn}_hf|L_p(\mathbb R^n)\|\leq c\sum^n_{j=1} \|\Delta^M_{h_j,j} f|L_p(\mathbb R^n)\|.$$

Futhermore

$$\begin{split}
&\int_{\mathbb R^n}|h|^{-sq}\|\Delta^{M}_{h_1,1} f|L_p(\mathbb R^n)\|^q\frac {\mathrm d h} {|h|^n}\\
=&\int_{\mathbb R} \|\Delta^{M}_{h_1,1} f|L_p(\mathbb R^n)\|^q\left(\int_{\mathbb R^{n-1}}(h_1^2+\dots+h_n^2)^{-\frac 1 2 (sq+n)}\mathrm d h_2\dots\mathrm d h_n\right)\mathrm dh_1\\
=&c\int_{\mathbb R}|h_1|^{-sq}\|\Delta^{M}_{h_1,1} f|L_p(\mathbb R^n)\|^q\frac {\mathrm d h_1} {|h_1|}.
\end{split}$$

And if we change the order of integration, we can get 

$$\sum^n_{j=1}\|\int_{\mathbb R}|h|^{-sp}\|(\Delta^M_{h,j}f)|L_p(\mathbb R)\|^p\frac{\mathrm d h}{|h|}|L_p(\mathbb R^{n-1})\|,$$

which proof it has Fubini Property for Besov and Triebel-Linzorkin spaces.