---
layout: page
permalink: /blogs/completion/index.html
title: completion
---

## 完备空间

1. 空间完备即任意Cauchy列都收敛；任何不完备的赋范线性空间都有完备化。
2. 空间的完备化是在等距同构的意义下唯一的。
3. 该唯一性依赖于==稠密==。
## 稠密的重要性

$$X:=\left\{(x_1, x_2,...)\in \mathbb R^\infty,\ \sup_{n\in \mathbb N} |x_n|<\infty\right\}$$

$$X_1:=\left\{(x_1, x_2,...)\in \mathbb R^\infty,\ x_1=0\ or\ 1,\ \sup_{n\in \mathbb N} |x_n|<\infty\right\}$$

$$X_2:=\left\{(0,x_1, x_2,...)\in \mathbb R^\infty,\ \sup_{n\in \mathbb N} |x_n|<\infty\right\}$$

显然 $(X, d)$ 是一个完备空间且它是自身的一个完备化。易证 $(X_1,d)$ 也是 $(X, d)$ 的一个完备化空间。现定义

$$X_3:=\left\{(1,x_1, x_2,...)\in \mathbb R^\infty,\ \sup_{n\in \mathbb N} |x_n|<\infty\right\}$$

我们来证明 $(X_1,d)$ 和 $(X, d)$ 并非同胚。事实上 $(X_1,d)$ 并不是连通的[^1]。我们来证明它。关键在于证明 $X_2$ 和 $X_3$ 均为开集合。取 $x\in X_3,\ B(x,\frac 1 2)\cap X_1\subset X_3$ ，==这说明每个 $X_3$ 中的点都有一个开临域==。同理 $X_2$ 也是开集。又有 $X_2\cup X_3= X_1$ ，则后者不连通。

从上述证明，我们就能看出稠密性的重要性。实际上他所定义的“最小”给出了度量空间按照等距映射的一个序关系。但是这个序关系并不是全序的，所以有可能存在两个完全不相干的全序列，即可能存在两个不同的极小元。

**只有等距同构保证不了同胚性。**

[^1]:连通的集合不能被分割为两个不交开集合的并。


