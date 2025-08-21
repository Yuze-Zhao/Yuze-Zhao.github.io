---
layout: page
permalink: /blogs/afPre/index.html
title: afPre
---

# What is Functional Analysis
1. Functional analysis is analysis (mathematical analysis or advanced algebra) on infinite-dimensional spaces.  
2. Origin (background): Specific analytical problems in mathematical physics.  
3. Research method: Abstract specific analytical problems into problems of analysis on spaces with topological (metric) and/or algebraic structures.  
4. Current status: Rich in content, widely applied, an essential tool for mathematicians.  

| Calculus & Linear Algebra | Finite-dimensional $\mathbb{R}^n (\mathbb{C}^n)$ | Matrices and Functions | Eigenvalues | Zeros |
| :-----------------------: | :---------------------------------------------: | :--------------------: | :---------: | :---: |
| Functional Analysis       | Infinite-dimensional spaces                      | $l^p$ , $C[a,b]$       | Operators   | Spectrum |

## Incomplete Normed Linear Spaces

1. Polynomials $P[0,1]$, $\|P\|_{P[0,1]}:=\max_{t\in[0,1]}{| P(t)|}$, its completion is $C[0,1]$.  
2. $\|f\|_{C[0,1]}:=\int^1_{0}|f|\,dx$, its completion is $L^1[0,1]$.  

## Definition of Operator Norm

$$\|T\|_{\mathcal{L}(\mathcal X,\ \mathcal Y)}=\sup_{x\in\mathcal X\backslash\{0\} }\frac{\|Tx\|}{\|x\|}$$