---
layout: page
permalink: /blogs/completion/index.html
title: completion
---

## Complete Spaces

1. A space is complete if every Cauchy sequence converges; any incomplete normed linear space has a completion.  
2. The completion of a space is unique in the sense of isometric isomorphism.  
   - In categorical terms, the completion is unique up to a unique isometric isomorphism: for any two completions of a given normed space, there exists a unique isometric isomorphism between them that restricts to the identity on the original space.  
3. This uniqueness relies on **density**.  

## The Importance of Density

$$X:=\left\{(x_1, x_2,...)\in \mathbb R^\infty,\ \sup_{n\in \mathbb N} |x_n|<\infty\right\}$$

$$X_1:=\left\{(x_1, x_2,...)\in \mathbb R^\infty,\ x_1=0\ \text{or}\ 1,\ \sup_{n\in \mathbb N} |x_n|<\infty\right\}$$

$$X_2:=\left\{(0,x_1, x_2,...)\in \mathbb R^\infty,\ \sup_{n\in \mathbb N} |x_n|<\infty\right\}$$

Clearly, $(X, d)$ is a complete space, and it is its own completion. It is easy to prove that $(X_1, d)$ is also a completion of $(X, d)$. Now define

$$X_3:=\left\{(1,x_1, x_2,...)\in \mathbb R^\infty,\ \sup_{n\in \mathbb N} |x_n|<\infty\right\}$$

We aim to prove that $(X_1, d)$ and $(X, d)$ are not homeomorphic. In fact, $(X_1, d)$ is not connected[^1]. Let us prove this. The key is to show that both $X_2$ and $X_3$ are open sets. Take $x\in X_3$, then $B(x,\tfrac 1 2)\cap X_1\subset X_3$ — **this shows that every point in $X_3$ has an open neighborhood**. Similarly, $X_2$ is also open. Since $X_2\cup X_3= X_1$, the latter is not connected.  

From this proof, we can see the importance of density. In fact, the definition of “minimal” gives a partial order of metric spaces under isometries. However, this order is not total, so it is possible to have two completely unrelated chains, i.e., two different minimal elements.  

**Isometric isomorphism alone does not guarantee homeomorphism.**

[^1]: A connected set cannot be split into the union of two disjoint open sets.
