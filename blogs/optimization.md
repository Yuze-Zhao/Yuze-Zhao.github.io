---
layout: page
permalink: /blogs/optimization/index.html
title: optimization
---

# Convex Optimization Problems

## Lagrange Multiplier Method

### Lagrangian Function
Provides a formulation for constrained optimization (in the sense of $C^1$ ), but in high-dimensional cases the computational workload is huge, so one usually turns to solving the dual problem.

## Slater’s Condition

Slater’s condition ensures that the solution of the primal problem in the Lagrangian formulation can be transformed into the solution of the dual problem (sufficiency), and also guarantees the existence of a saddle point.

## KKT Conditions

The KKT conditions guarantee that the saddle point is exactly the solution we are looking for (sufficiency).  
Under the restriction of a convex feasible set, the KKT conditions are both necessary and sufficient.

$$
\inf_{x \in X} \sup_{\lambda} \mathcal{L}(x,\lambda)
= \sup_{\lambda} \inf_{x \in X} \mathcal{L}(x,\lambda)
$$

*PS: When the Lagrangian function is convex, a local minimum is also a global minimum.*

## Dual Proposition

The key to the dual proposition is to identify the relationship between the variables and the dual variables, then substitute this relationship back into the Lagrangian function. Their relationship is given by:

$$
\frac{\partial \mathcal{L}}{\partial x}.
$$

<!-- # 凸优化问题

## 拉格朗日乘子法

### 拉格朗日函数：给出了约束优化的（在C1的意义下），但高维数条件下工作量巨大，采取计算对偶问题的方法。

## Slater条件

### Slater条件保证了拉格朗日函数的原问题的解可以转化为对偶问题的解（充分性），且保证了鞍点的存在。

## KKT条件

### KKT条件保证了鞍点就是我们要找的解（充分性），当在凸可行域的限制下，KKT是充要条件。

$$
\inf_{x\in X}\sup_{\lambda}\mathcal L(x,\lambda)=\sup_{\lambda}\inf_{x\in X}\mathcal L(x,\lambda)
$$

PS:当拉格朗日函数是凸函数的时候局部最小值是全局最小值。

## 对偶命题

### 对偶命题的关键是找出变量与对偶变量的关系，然后带入Largrange函数即可。而他们的关系由 $\frac{\partial \mathcal L}{\partial x}$ 给出。 -->







