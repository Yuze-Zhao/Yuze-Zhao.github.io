# 3 Weighted inequalities associated with operators

本节讨论与 Hardy-Littlewood 型极大算子、Calderón-Zygmund 算子以及其他重要算子相关的加权不等式。重点是比较标量情形与矩阵情形的差异，尤其是 sharp bound 的变化。

## 3.0 本节结构

本节分三部分：

- **3.1 Hardy-Littlewood maximal operator**：回顾标量极大算子的定量加权估计，以及矩阵情形中的 Christ-Goldberg 极大算子、弱型不等式和相关开放问题。
- **3.2 Calderón-Zygmund operators and $A_2$ conjecture**：回顾标量 $A_2$ conjecture 的解决，以及矩阵情形中 sharp power 与标量情形不同的现象。
- **3.3 Further remarks**：讨论分数极大算子、分数积分算子、$A_{p,q}$ 权以及相关矩阵加权结果。

## 3.1 The Hardy-Littlewood maximal operator

### 标量强型估计

- Theorem 3.1：Buckley 型结果。
  - 对 $1<p<\infty$，$M$ 在 $L^p(w)$ 上有界当且仅当 $w\in A_p$。
  - 定量估计中 $[w]_{A_p}^{1/(p-1)}$ 是 sharp 的。
- 该结果是定量加权理论的基本模型。

### 标量弱型估计

- Definition 3.2 定义加权弱 Lebesgue 空间 $L^{p,\infty}(w)$。
- Theorem 3.2：Hardy-Littlewood 极大算子的弱型估计。
  - 对 $p\ge1$，$M$ 从 $L^p(w)$ 到 $L^{p,\infty}(w)$ 有界与 $w\in A_p$ 相关。
  - 给出相应定量依赖。

### Sawyer 型与 two-weight 观点

- Theorem 3.3：给出与 $M$ 的加权弱型和强型估计相关的进一步定量结果。
- Remark 3.1：指出 Theorem 3.3(ii) 中指数的 sharpness，强调 $p$ 与 $A_p$ 常数之间的最优依赖。

### Scalar auxiliary maximal operator

- Theorem 3.4：引入或使用某种权相关极大算子 $M_{w,p}$，并刻画其从 $L^p$ 到 $L^{p,\infty}$ 的有界性与某个权类 $A_p^*$ 的关系。
- Question 3.1：$p=1$ 情形是否可引入合适的 $A_1^*$ 权类，使类似刻画成立，仍是开放问题。

### 矩阵加权极大算子

- 矩阵情形中，直接将 $M$ 作用到 $|W^{1/p}f|$ 通常不能给出完整理论，需要引入矩阵加权极大算子。
- Theorem 3.5：对矩阵权 $W$，给出相应极大算子的有界性刻画。
- Theorem 3.6：对 $W\in A_p$，给出矩阵加权极大算子的强型和弱型定量估计。
- Question 3.2：受 Theorem 3.4 启发，是否存在合适的矩阵权类 $A_p^*$，使 $W\in A_p^*$ 当且仅当矩阵权相关极大算子从 $L^p$ 到 $L^{p,\infty}$ 有界，仍有待研究。

## 3.2 Calderón-Zygmund operators and $A_2$ conjecture

### Calderón-Zygmund 算子的定义

- Definition 3.1：定义 Calderón-Zygmund 算子，包括核的大小条件、光滑性条件以及在 $L^2$ 上的有界性。
- 卷积型 Calderón-Zygmund 算子是一般 Calderón-Zygmund 算子的特殊情形。

### 标量 $A_2$ conjecture 与 sharp bound

- Theorem 3.7：对 $1<p<\infty$、$w\in A_p$ 和 Calderón-Zygmund 算子 $T$，有 sharp quantitative bound：
  $$\|T\|_{L^p(w)\to L^p(w)}\lesssim [w]_{A_p}^{\max\{1,1/(p-1)\}}.$$
- 该结果包括著名的 $A_2$ conjecture，最终由 Hytönen 解决。
- Remark 3.2：对非退化卷积 Calderón-Zygmund 算子，上述指数 sharp。

### Extrapolation

- Theorem 3.8：给出标量加权 extrapolation 定理。
  - 若某个算子在一个指数 $p_0$ 上对所有 $A_{p_0}$ 权满足定量估计，则可推广到所有 $p$。
  - 该工具在由 $p=2$ 推出全范围 $p$ 估计时非常重要。

### 弱型与 sharp maximal truncation

- Theorem 3.9：给出 Calderón-Zygmund 算子的弱型加权估计。
- Theorem 3.10：给出 maximal truncated operator 的相应加权估计。
- Question 3.3：围绕弱型估计和 truncation 估计的 sharpness 或最优常数提出问题。

### 矩阵加权 Calderón-Zygmund 估计

- 矩阵情形中，Calderón-Zygmund 算子的定量估计与标量情形显著不同。
- Goldberg 首先研究了矩阵加权下 Hardy-Littlewood 极大算子和 Calderón-Zygmund 算子的有界性。
- Theorem 3.11：对 $1<p<\infty$、$W\in A_p$ 和 Calderón-Zygmund 算子 $T$，给出矩阵加权 $L^p(W)$ 上的有界性估计。
- Theorem 3.12：矩阵权 extrapolation 定理。若在某个 $p_0$ 上有矩阵加权估计，则可推广到其他指数。

### 矩阵 $A_2$ conjecture 的失败

- Theorem 3.13：当 $m\ge2$、$W\in A_2(\mathbb R,\mathbb C^m)$，Hilbert 变换满足估计，其中 sharp power 不是标量情形的 1，而是 $3/2$。
- 这一结果说明矩阵 $A_2$ conjecture 不能像标量情形那样成立。
- 该现象是全文最重要的对比之一：矩阵权理论不是标量理论的形式性升维。
- Question 3.4：当 $p\in(1,2)\cup(2,\infty)$ 时，相关矩阵加权估计中的 sharp bound 仍未知。

### Sparse domination 与改进估计

- Theorem 3.14：给出与 sparse operators 或 convex body-valued sparse domination 相关的矩阵加权估计。
- Question 3.5：若干矩阵加权 sparse/Calderón-Zygmund 型不等式中的 sharp bounds 仍有待确定。

## 3.3 Further remarks

本小节讨论除 Hardy-Littlewood 极大算子与 Calderón-Zygmund 算子之外的其他算子，尤其是分数极大算子与分数积分算子。

### 标量 $A_{p,q}$ 权与分数算子

- Definition 3.3：定义标量 $A_{p,q}$ 权。
- Theorem 3.15：对分数极大算子，若 $w\in A_{p,q}$，则存在从 $L^p(w^p)$ 到 $L^q(w^q)$ 的加权估计，并给出定量依赖。
- Theorem 3.16：对分数积分算子，给出对应 $A_{p,q}$ 加权估计。

### 矩阵 $A_{p,q}$ 权

- Definition 3.4：定义矩阵 $A_{p,q}$ 权。
- Theorem 3.17：矩阵分数极大算子的加权估计。
- Theorem 3.18：矩阵分数积分算子的加权估计。
- Question 3.6：相关矩阵分数积分/极大算子估计中的 bound 是否 sharp 仍是开放问题。

### 其他方向

- 文中还提到矩阵加权变量指数 Lebesgue 空间、rough singular integrals、sparse bounds 等方向。
- 这些结果表明矩阵权理论已经从经典 $L^p(W)$ 空间逐渐扩展到更复杂的函数空间和算子类别。

## 本节阅读重点

1. 标量 $A_p$ 理论中 Hardy-Littlewood 极大算子与 Calderón-Zygmund 算子的 sharp bounds 已较完整。
2. 矩阵情形中，极大算子理论可部分平行于标量情形，但 Calderón-Zygmund 算子出现本质差异。
3. 矩阵 $A_2$ conjecture 的失败说明矩阵加权理论具有独立结构。
4. 分数算子部分通过 $A_{p,q}$ 权连接经典势理论、矩阵权和现代稀疏控制方法。
