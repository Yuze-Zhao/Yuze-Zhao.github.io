# 4 Matrix-weighted function spaces

本节综述矩阵加权函数空间，包括 Sobolev 空间、BMO 空间、Besov-Triebel-Lizorkin 型空间，以及其他近期发展方向。重点是矩阵权对经典函数空间结构、对偶、交换子、有界性和实变量刻画的影响。

## 4.0 本节结构

- **4.1 Matrix-weighted Sobolev spaces**：矩阵加权 Sobolev 空间与 Poincare 型不等式。
- **4.2 Matrix-weighted BMO spaces**：矩阵加权 BMO、交换子有界性与 two-weight theory。
- **4.3 Matrix-weighted Besov-Triebel-Lizorkin-type spaces**：矩阵加权 Besov-Triebel-Lizorkin 型空间、$\varphi$-transform、almost diagonal operators 和分解刻画。
- **4.4 Further remarks**：周期矩阵权、Bourgain-Morrey 空间、调制空间和 Banach 值权。

## 4.1 Matrix-weighted Sobolev spaces

### 两类矩阵加权 Sobolev 空间

- Definition 4.1：定义 degenerate matrix-weighted Sobolev space。其基本思想是用矩阵权控制函数及其弱导数。
- Definition 4.2：定义另一类矩阵加权 Sobolev 空间 $W^{1,p}(W,\Omega)$，通常由光滑函数完备化得到。
- 当 $m=1$ 或矩阵权退化为标量权时，这些空间与经典加权 Sobolev 空间相联系。

### 空间之间的关系

- Proposition 4.1：对 $p\in[1,\infty)$、$W\in A_p$，给出两类矩阵加权 Sobolev 空间之间的关系。
- 文中指出在适当条件下，这些空间可相互嵌入或等价；但矩阵情形通常需要更细致的权条件。

### Poincare 型不等式与正则性

- Theorem 4.1：对 $p\in(1,\infty)$、$W\in A_p$，建立矩阵加权 Poincare 型不等式。
- 该结果可进一步导出 reverse Meyers-Hölder inequality。
- Isralowitz-Moen 的结果还可用于退化椭圆方程弱解的正则性研究。

### 本小节阅读重点

- 矩阵权 Sobolev 空间不是简单的逐分量加权 Sobolev 空间。
- Poincare 不等式是连接矩阵加权函数空间与 PDE 正则性的关键。
- 矩阵权与 gradient 的相互作用是主要难点。

## 4.2 Matrix-weighted BMO spaces

### 背景

- 矩阵值 BMO 是标量 BMO 的自然非交换推广。
- 它在加权不等式、非交换调和分析、PDE 正则性以及算子空间理论中都具有作用。

### Two-weight matrix BMO

- Definition 4.3：对 $p,q\in(1,\infty)$ 和矩阵权 $U,V\in A_{p,q}$，定义 two matrix-weighted BMO space $BMO^{p,q}_{U,V}$。
- 当 $p=q$ 时记作 $BMO_{U,V}$；当 $U=V=W$ 时记作 $BMO_W$。
- 当 $m=1$ 且权为常数时，退化为经典 BMO。

### 交换子与 BMO

- 标量情形中，Coifman-Rochberg-Weiss 型结果表明 Calderón-Zygmund 交换子 $[b,T]$ 的有界性等价于 $b\in BMO$。
- 矩阵情形中，交换子定义为 $[B,T]f=B T f-T(Bf)$，其中 $B$ 为矩阵值函数。
- Theorem 4.2：给出矩阵加权 two-weight BMO 与 Calderón-Zygmund 交换子有界性的关系。
  - 若 $B\in BMO^{p,q}_{U,V}$，则交换子有界；
  - 在非退化条件下，交换子有界性可反过来控制 $BMO$ 范数。

### 相关发展

- Isralowitz 研究了 two matrix-weighted setting 下交换子有界性与 $H^1$-$BMO$ 对偶。
- Cruz-Uribe 和 Isralowitz 将该理论发展到更定量的 two-weight matrix BMO，并研究分数积分相关的 BMO-type 空间。
- Bu 等人的工作还涉及 vector-valued matrix-weighted Hardy spaces 与 vector-valued matrix-weighted BMO spaces。

## 4.3 Matrix-weighted Besov-Triebel-Lizorkin-type spaces

本小节是函数空间部分的核心，讨论矩阵加权 Besov-Triebel-Lizorkin 型空间的定义、序列空间、$\varphi$-transform、almost diagonal operators 和后续分解刻画。

### 历史背景

- Besov 空间源于 Bernštein、Zygmund、Nikol'skii 和 Besov 的工作。
- Triebel-Lizorkin 空间由 Triebel、Lizorkin 等发展。
- Frazier-Jawerth 的 $\varphi$-transform 为这些空间提供了统一的离散化工具。
- Frazier-Roudenko 将该框架推进到矩阵加权 Besov 与 Triebel-Lizorkin 空间。

### 矩阵加权 Besov-Triebel-Lizorkin 型空间

- Definition 4.4：定义齐次矩阵加权 Besov-Triebel-Lizorkin 型空间 $\dot A^{s,\tau}_{p,q}(W)$。
- 其中参数包括：
  - 光滑度 $s$；
  - Morrey 型参数 $\tau$；
  - 指数 $p,q$；
  - 矩阵权 $W\in A_{p,\infty}$。
- Remark 4.1：该空间在特定参数下可退化为若干经典空间或已有矩阵加权空间。

### 序列空间与 $\varphi$-transform

- Definition 4.5：定义对应的矩阵加权 Besov 型序列空间。
- Theorem 4.3：建立 $\varphi$-transform characterization。
  - 连续函数空间与离散序列空间之间通过分析算子和综合算子建立等价。
  - 这是后续分子分解、波let分解和算子有界性的基础。

### Almost diagonal operators

- Definition 4.6：定义 $(D,E,F)$-almost diagonal matrix。
- Theorem 4.4：给出 almost diagonal operators 在矩阵加权序列空间上的有界性。
- Remark 4.2：若进一步假设 $W\in A_p$，Theorem 4.4 中部分指数项可用 $A_p$-dimension 及对偶维数改进。

### 进一步结果

- Theorem 4.5：在 Besov 型序列空间上，满足条件的 almost diagonal operators 有界。
- Theorem 4.6：在 Triebel-Lizorkin 型序列空间上，满足条件的 almost diagonal operators 有界。
- Question 4.1：猜测 Theorem 4.6 在 $q\in(0,\min\{1,p\})$ 时仍成立，但目前尚未解决。
- 应用：Bu 等人进一步利用 $\varphi$-transform 和 almost diagonal estimates 得到：
  - molecules characterization；
  - wavelet characterization；
  - pseudo-differential operators 的有界性；
  - trace operators 的有界性；
  - pointwise multipliers；
  - Calderón-Zygmund operators 在这些空间上的有界性。
- 非齐次版本也成立。

### 本小节阅读重点

1. $A_{p,\infty}$ 是定义最一般矩阵加权 Besov-Triebel-Lizorkin 型空间的自然权类。
2. 权的维数控制不同 dyadic cubes 上 reducing operators 的相对增长，是 almost diagonal estimates 的核心。
3. $\varphi$-transform 将函数空间问题转化为序列空间问题。
4. Almost diagonal operators 是建立分解刻画和算子有界性的统一工具。

## 4.4 Further remarks

本小节总结其他矩阵加权函数空间方向。

### 周期矩阵权与三角系统

- Nielsen 研究周期矩阵权及其在函数空间中的应用。
- 重点包括：
  - 向量值三角系统在矩阵加权 $L^p(W,\mathbb T)$ 中形成 Schauder basis 的条件；
  - quasi-greedy bases；
  - transference methods；
  - 周期矩阵权与非周期矩阵权之间的联系。

### Bourgain-Morrey spaces

- 文中提到矩阵加权 Bourgain-Morrey 空间是近期发展方向之一。
- 这类空间结合 Bourgain 型局部结构与 Morrey 型尺度控制，适合研究更精细的局部-全局行为。

### Modulation spaces

- 调制空间与时频分析相关。
- 矩阵加权调制空间将矩阵权引入频率-空间联合局部化框架，是矩阵权理论向时频分析扩展的方向。

### Banach-valued weights

- 文中提到从矩阵权向 Banach 值权的推广。
- 这表明矩阵权理论可以看作更一般算子值或 Banach 值加权理论的有限维模型。

## 本节阅读重点

- 第4节从 Sobolev、BMO 到 Besov-Triebel-Lizorkin 型空间，展示矩阵权理论在函数空间中的多层次应用。
- Sobolev 部分偏向 PDE 与 Poincare 不等式。
- BMO 部分偏向交换子和 two-weight theory。
- Besov-Triebel-Lizorkin 部分偏向实变量方法、离散化、分解和算子理论。
- Further remarks 说明该方向仍在快速扩展，特别是周期情形、Morrey 型结构、调制空间和 Banach 值推广。
