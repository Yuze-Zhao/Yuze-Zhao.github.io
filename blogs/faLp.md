---
layout: page
permalink: /blogs/faLp/index.html
title: faLp
---

### measure space 
A measure space is a set $X$ equipped with a $\sigma$ -algebra of subsets of it and a function $\mu$ form the $\sigma$ -algebra to $[0.\infty]$ that satisfies $\mu(\emptyset) = 0$ and 

$$\mu\left(\bigcup^{\infty}_{j=1}B_j\right)=\sum^{\infty}_{j=1}B_j$$

for any sequence $B_j$ of pairwise disjoint elements of the $\sigma$ -algebra. The function $\mu$ is called a (positive) measure on $X$ and elements of the $\sigma$ -algebra of $X$ are called measure sets.

Measure spaces will be assumed to be complete, i.e., subsets of the σ-algebra of measure zero also belong to the σ-algebra. (**sets have a measure of zero are all measurable sets.**)

### $\sigma$ -finite
 A measure space $X$ is called σ-finite if there is a sequence of measurable subsets $X_n$ of it such that

 $$X=\bigcup^{\infty}_{n=1}X_n$$

 and $\mu(X_n)<\infty$ .

### finite simple functions
A finitely simple function has the form

$$\sum^{N}_{j=1}c_j X_{B_j}$$

where $N<\infty$ , $c_j\in\mathrm{C}$ , and $B_j$ are pairwise disjoint measurable sets with $\mu(B_j)<\infty$ . If $N=\infty$ , this function is *countable simple functions*.
