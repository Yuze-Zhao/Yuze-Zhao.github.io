# 2 Properties of scalar and matrix Muckenhoupt weights

本节是全文的理论基础，主要讨论标量和矩阵 Muckenhoupt 权的定义、例子、结构性质、等价刻画、维数理论及 sharp indices。笔记只整理主要结果和 remark，不包含证明过程。

## 2.0 基本定义与预备内容

### 标量权与 $A_p$ 权

- 标量权是几乎处处正且局部可积的函数。
- 对 $p\in[1,\infty]$，定义 $A_p$ 标量权：
  - $p=1$ 时通过局部平均与本质下界刻画；
  - $1<p<\infty$ 时通过标准 Muckenhoupt 条件刻画；
  - $p=\infty$ 时通过指数平均刻画。
- Remark 2.1 指出，定义中的 cube 可等价替换为 ball。

### $A_1$ 的极大函数刻画

- Proposition 2.1：$w\in A_1$ 当且仅当 Hardy-Littlewood 极大函数满足 $M(w)\le Cw$ 几乎处处成立。

### $A_1$、$A_p$ 与 $A_\infty$ 的内在联系

- Proposition 2.2 和 Proposition 2.3 分别给出函数型与离散型的极限平均公式。
- 这些公式解释了：
  - $p\to1^+$ 时，$A_p$ 条件趋向 $A_1$ 条件；
  - $p\to\infty$ 时，$A_p$ 条件趋向 $A_\infty$ 条件。
- 文中强调指数函数在 $A_\infty$ 定义中出现的原因与 Euler 极限有关。

### 反 Hölder 类

- Definition 2.2 定义 $RH_q$ 类。
- Remark 2.2：标量情形有
  $$A_\infty=\bigcup_{p\in[1,\infty)}A_p=\bigcup_{q\in(1,\infty]}RH_q.$$

### 矩阵权与矩阵 $A_p$ 权

- 矩阵权是几乎处处正定且矩阵元素局部可积的矩阵值函数。
- Definition 2.3 定义矩阵 $A_p(\mathbb R^n,\mathbb C^m)$ 权：
  - $0<p\le1$ 与 $1<p<\infty$ 的定义形式不同；
  - 当 $m=1$ 时，该定义退化为标量 $A_{\max\{1,p\}}$。
- Proposition 2.4 给出 $0<p\le1$ 情形下矩阵 $A_p$ 的等价刻画。

### 矩阵 $A_{p,\infty}$ 权

- Definition 2.4 定义 $A_{p,\infty}$ 矩阵权，作为矩阵情形下 $A_\infty$ 的一种精细模拟。
- 当 $m=1$ 时，$A_{p,\infty}$ 退化为标量 $A_\infty$。

## 2.1 Examples of scalar and matrix Muckenhoupt weights

本小节通过大量例子说明标量权与矩阵权的细微差别，并展示某些结果的 sharpness。

### 标量权的 critical indices

- 定义 critical self-improvement index：
  $$r_s(w)=\inf\{r>1:w\in A_r\}.$$
- 定义 critical reverse Hölder index：
  $$r_h(w)=\sup\{r>1:w\in RH_r\}.$$

### 幂权例子

- Example 2.1：对 $w_a(x)=|x|^a$：
  - $w_a\in A_1$ 当且仅当 $a\in(-n,0]$；
  - $w_a\in A_p$ 当且仅当 $a\in(-n,n(p-1))$；
  - $w_a\in A_\infty$ 当且仅当 $a\in(-n,\infty)$。

### 带对数扰动的权

- Lemma 2.2 给出 $|x|^a[\log(2+|x|)]^b$ 及其近零型变体的平均估计。
- Example 2.2：对 $w_{a,b}$ 和 $\widetilde w_{a,b}$，完整刻画它们属于 $A_1$、$A_p$、$A_\infty$ 的条件，并给出 critical index $r_s$。
- Example 2.3：对应地刻画这些权属于 $RH_q$ 和 $RH_\infty$ 的条件，并给出 $r_h$。

### 从标量权构造矩阵权

- Lemma 2.3：若 $W=wI_m$，则：
  - $W\in A_p$ 当且仅当 $w\in A_{\max\{1,p\}}$；
  - $W\in A_{p,\infty}$ 当且仅当 $w\in A_\infty$。
- 这类例子是平凡矩阵例子，不能反映矩阵权的真正复杂性。

### 非平凡矩阵权例子

- Example 2.4 构造一类二维旋转型矩阵权 $W_{\alpha,\beta}$，并精确刻画其属于 $A_p$ 和 $A_{p,\infty}$ 的条件：
  - 对 $1<p<\infty$：$W_{\alpha,\beta}\in A_p$ 当且仅当 $\beta\in(-n,n(p-1))$ 且 $\alpha\ge |\beta|/p$；
  - 对 $0<p\le1$：$W_{\alpha,\beta}\in A_p$ 当且仅当 $\beta\in(-n,0]$ 且 $\alpha\ge -\beta/p$；
  - 对 $0<p<\infty$：$W_{\alpha,\beta}\in A_{p,\infty}$ 当且仅当 $\beta\in(-n,\infty)$ 且 $\alpha\ge |\beta|/p$。
- 该例子说明矩阵 Muckenhoupt 权不具备标量权那样的自改进性质。

### Bickel 等人的矩阵幂权例子

- Example 2.5 给出形如 $a_{ij}|x|^{\gamma_{ij}}$ 的矩阵权，并在 $A_2$ 情形下刻画其条件。
- Question 2.1：对这类矩阵幂权，如何刻画 $A_p$ 与 $A_{p,\infty}$ 条件仍是自然问题。

### 构造新权的方法

- Proposition 2.5：乘积型标量权 $w_{prod}(x)=\prod_i w_i(x_i)$ 的 $A_p$ 与 $RH_q$ 条件可逐坐标刻画，并给出 critical indices 的最大/最小关系。
- Theorem 2.1：Coifman-Rochberg 型构造说明极大函数的幂可产生 $A_1$ 权，并且每个 $A_1$ 权可由此形式表示。
- Theorem 2.2：Jones factorization：标量 $A_p$ 权可分解为两个 $A_1$ 权的乘积形式。
- Proposition 2.6：标量 $A_p$ 权在几何平均、和、最大值、最小值下具有稳定性。
- Theorem 2.3：矩阵版 Jones factorization：$W\in A_p$ 当且仅当存在两个可交换的 $A_1$ 矩阵权 $W_1,W_2$ 使 $W=W_1W_2^{1-p}$。
- Question 2.2：提出矩阵情形下关于 $A_q$ 替代 $A_1$、$A_{p,\infty}$ factorization，以及矩阵版构造定理的开放问题。

## 2.2 Properties of scalar Muckenhoupt weights

本小节整理标量权的经典性质、等价刻画和若干细节性结果。

### 加权 Lebesgue 空间

- Definition 2.5 定义 $L^p(w)$。

### $A_p$ 的基本刻画

- Proposition 2.7：$w\in A_p$ 当且仅当 $w^{1-p'}\in A_{p'}$，并给出特征常数关系。
- Proposition 2.8：$w\in A_p$ 当且仅当 $w\in A_\infty$ 且 $w^{1-p'}\in A_\infty$。
- Proposition 2.9：$A_p$ 可通过局部 $L^p(w)$ 归一化函数的平均估计刻画。

### $A_\infty$ 的等价刻画

- Proposition 2.10 汇总 $A_\infty$ 的多种等价刻画，包括：
  - 指数平均形式；
  - $\bigcup_{p<\infty}A_p$；
  - measure decay 条件；
  - Wilson 型 $A_\infty^*$ 常数；
  - 反 Hölder 条件；
  - 弱型分布估计形式。

### BMO、VMO、BLO 与权的关系

- Definition 2.6 定义 BMO。
- Definition 2.7 定义 VMO。
- Definition 2.8 定义 BLO。
- Proposition 2.11 给出标量权的一系列性质：
  - 平移、伸缩、常数倍不改变 $A_p$ 常数；
  - $[w]_{A_p}\ge1$，等号仅在常值权时成立；
  - $A_p$ 关于 $p$ 单调递增；
  - $A_p$ 类之间严格包含；
  - 幂次扰动的稳定性与自改进性质；
  - VMO、BMO、BLO 与 $\log w$ 的表示关系；
  - doubling 型估计。

### Remarks

- Remark 2.3：
  - 由 BLO 的刻画可得 $BLO\cup(-BLO)=\{\lambda\log w:\lambda\in\mathbb R,w\in A_1\}$；
  - $BLO\cup(-BLO)$ 是 BMO 的真子集，并给出典型例子说明。
- Remark 2.4：Corollary 2.1(i) 也可由 $A_p$ 的开性质推出。
- Remark 2.5：Theorem 2.4 中 sharp reverse Hölder inequality 的常数可取 2，且与权特征常数无关。

### $A_p$ 常数关于 $p$ 的连续性

- Proposition 2.12 给出下降重排下界估计。
- Proposition 2.13：对任意标量权，$[w]_{A_q}$ 在 $q\to1^+$、$q\to\infty$ 和 $q\to p$ 时具有相应极限。
- Corollary 2.1：$w\in A_p$ 可通过邻近 $A_q$ 常数的有界性刻画。

### Sharp reverse Hölder inequality

- Theorem 2.4：若 $w\in A_\infty$，则存在明确范围的 $r>1$ 使反 Hölder 不等式成立，并且常数为 2。

## 2.3 Properties of matrix Muckenhoupt weights

本小节研究第2.2节标量性质在矩阵情形中的对应版本，并指出哪些性质不能直接推广。

### Reducing operators

- Definition 2.9 定义 order $p$ 的 reducing operator $A_E$。
- Remark 2.6：reducing operator 的存在性由 Goldberg、Frazier-Roudenko 等结果保证。
- Proposition 2.14：reducing operator 可等价刻画矩阵均值范数。

### 矩阵 $A_p$ 与对偶权

- Lemma 2.6：
  - 对 $p>1$，$W\in A_p$ 当且仅当 $W^{1-p'}\in A_{p'}$；
  - 给出 $A_Q^{-1}$ 与 $W^{-1/p}$ 的局部积分/本质上确界/指数平均之间的等价关系。

### $A_p$ 与 $A_{p,\infty}$ 的关系

- Proposition 2.15：对 $p>1$，$W\in A_p$ 当且仅当 $W\in A_{p,\infty}$ 且 $W^{-p'/p}\in A_{p',\infty}$。
- Proposition 2.16：对 $0<p\le1$，$W\in A_p$ 可由 $A_{p,\infty}$ 条件和一个额外指数型本质上确界条件刻画。
- Proposition 2.17：当 $m=1$ 时，得到可视为 $A_1$ “对偶性”的标量刻画。
- Remark 2.7：从平均、指数平均和本质下界之间的等价关系解释 Proposition 2.17 的自然性。

### 函数测试型刻画

- Proposition 2.18：对 $0<p\le1$，矩阵 $A_p$ 可通过矩阵值测试函数族 $H_Q$ 刻画。
- Lemma 2.7 和 Remark 2.8：给出相关对偶型公式。
- Proposition 2.19：对 $p>1$，矩阵 $A_p$ 也可由测试函数族刻画。
- Remark 2.9：Propositions 2.18 与 2.19 在 $m=1$ 时退化为标量 Proposition 2.9。
- Proposition 2.20：$A_{p,\infty}$ 的测试函数刻画。
- Proposition 2.21：给出 $A_{p,\infty}$ 的多种等价刻画，包括 reducing operator、向量测试和矩阵测试形式。
- Proposition 2.22：当 $m=1$ 时，Proposition 2.21 退化为 $A_\infty$ 的等价刻画。

### $A_{p,\infty}$ 的自改进型性质

- Proposition 2.23：$W\in A_{p,\infty}$ 当且仅当存在 $u>0$ 使 reducing operator 形式的局部 $L^u$ 估计成立。
- Remark 2.10：当 $m=1$ 时，该结果退化为 $A_\infty=\bigcup_p A_p$。
- Proposition 2.24：给出 $A_{p,\infty}$ 的一系列类 $A_\infty$ 性质，包括：
  - scalarization 后的反 Hölder 型估计；
  - 小集合上的绝对连续性；
  - 分布函数估计；
  - 中位数型量 $m(W;Q)$ 与 $\widetilde m(W;Q)$ 的一致估计。

### Remarks

- Remark 2.11：
  - 当 $m=1$ 时，Proposition 2.24 的若干断言对应 Proposition 2.10 中 $A_\infty$ 的等价条件；
  - 矩阵情形中，这些断言是否都等价于 $W\in A_{p,\infty}$ 仍不清楚；
  - 将矩阵权 scalarization 可能损失矩阵信息；
  - Proposition 2.10 中部分 $A_\infty$ 刻画是否存在矩阵对应版本仍未知。

### 矩阵权类的基本性质

- Lemma 2.8 和 Lemma 2.9 是矩阵幂与范数估计的工具性结果。
- Proposition 2.25：矩阵 $A_p$ 权的主要性质：
  - 平移、伸缩、常数倍不改变 $A_p$ 常数；
  - $[W]_{A_p}\ge1$；
  - $A_p\subset A_q$ 且严格包含；
  - $\bigcup_{q<p}A_q$ 可以是真子集；
  - $W^\alpha$ 对 $0<\alpha<1$ 保持在 $A_p$ 中；
  - 对某些 $\alpha>1$，有 $W^\alpha\in A_{p\alpha}$。
- Remark 2.12：
  - 对 $0<p<1$，$A_p\subsetneqq\bigcap_{q>p}A_q$ 是否严格仍有待确认；
  - 某些结果在一维、$p>1$ 情形下退化为 Bownik 的已知结果；
  - VMO/BMO 与权对数的标量刻画不能简单推广到矩阵元素逐项属于 VMO/BMO 的形式；
  - 权的维数可改进某些 doubling 型估计。
- Proposition 2.26：矩阵 $A_{p,\infty}$ 的基本性质，包括单调性、与 $A_p$ 的关系、幂次稳定性及 strict inclusion。
- Proposition 2.27：刻画矩阵 $A_p$ 何时具有某种自改进性质，等价于存在更小的 $A_q$、存在 $W^\alpha\in A_p$ 等条件。
- Proposition 2.28：给出 $A_{p,\infty}$ 的类似自改进刻画。
- Question 2.3：矩阵 $A_q$ 或 $A_{q,\infty}$ 常数在 $q\to p^+$ 时是否收敛到对应 $p$ 常数仍是问题。
- Remark 2.13：由于矩阵权缺乏标量型自改进性质，$q\to p^-$ 的极限不再有意义；目前可得 liminf 型不等式，但 limsup 型不等式未知。

## 2.4 Dimensions of weights

本小节是矩阵权理论的核心技术部分。维数理论用于精确控制 reducing operators 在不同 cube 上的相对增长。

### $A_p$-dimension

- Definition 2.10：定义矩阵权具有 $A_p$-dimension $d$，记作 $W\in D_{p,d}$。
- Proposition 2.29：对 $0<p\le1$，给出 $D_{p,d}$ 的等价刻画。
- Proposition 2.30：$D_{p,d}$ 的基本结构：
  - $d<0$ 时为空；
  - $0\le d<n$ 时为 $A_p$ 的真子类；
  - $\bigcup_{d\in[0,n)}D_{p,d}=A_p$；
  - $d\ge n$ 时 $D_{p,d}=A_p$；
  - 维数关于 $d$ 单调递增；
  - $D_{p,d}\subset D_{q,d}$ for $q>p$。
- Remark 2.14：$[0,n)$ 是 $A_p$-dimension 的有效范围。

### reducing operators 与维数

- Proposition 2.31：$W\in D_{p,d}$ 当且仅当 $\|A_QA_{\lambda Q}^{-1}\|^p\lesssim\lambda^d$。
- 定义 critical dimension：
  $$d_p(W)=\inf\{d\in[0,n):W\in D_{p,d}\}.$$
- Proposition 2.32：critical value 本身可能是也可能不是实际维数。
- Proposition 2.33：通过 dyadic dilation 下的 reducing operators 增长率计算 $d_p(W)$。
- Proposition 2.34：交换 $Q$ 与 $\lambda Q$ 后，$p\le1$ 情形平凡，$p>1$ 情形与对偶权的维数有关。
- Proposition 2.35：给出 $\|A_QA_R^{-1}\|$ 的 sharp estimate，是后续函数空间估计的重要基础。

### $A_{p,\infty}$ 的 lower/upper dimensions

- Definition 2.11：定义 $A_{p,\infty}$-lower dimension 与 upper dimension，记作 $D^{lower}_{p,\infty,d}$ 和 $D^{upper}_{p,\infty,d}$。
- Proposition 2.36：两类维数的基本结构：
  - lower dimension 的有效范围是 $[0,n)$；
  - upper dimension 的有效范围是 $[0,\infty)$；
  - 二者都给出 $A_{p,\infty}$ 的分类；
  - 当 $0<p\le1$ 时，$A_p=D^{upper}_{p,\infty,0}$。
- Remark 2.15：强调 lower/upper dimensions 是 $A_{p,\infty}$ 的两种不同分类。
- Proposition 2.37：lower/upper dimensions 可分别通过 $\|A_QA_{\lambda Q}^{-1}\|$ 与 $\|A_{\lambda Q}A_Q^{-1}\|$ 控制。
- Proposition 2.38：critical lower/upper dimensions 的临界值可能被达到，也可能不被达到，四种情况都可能出现。
- Proposition 2.39：给出 lower/upper critical dimensions 的 dyadic 计算公式。
- Proposition 2.40：给出 $A_{p,\infty}$ 情形下 $\|A_QA_R^{-1}\|$ 的 sharp estimate。

### $A_p$ 与 $A_{p,\infty}$ 维数的关系

- Proposition 2.41：
  - 在 $W\in A_p$ 下，lower dimension 与 $A_p$-dimension 等价；
  - $0<p\le1$ 时 upper critical dimension 为 0；
  - $p>1$ 时 upper dimension 与对偶权 $W^{1-p'}$ 的 $A_{p'}$-dimension 相关。

### 标量情形中的解释

- Definition 2.12：定义标量 $A_\infty$ 的 lower/upper dimensions。
- Proposition 2.42 和 2.43：标量 $A_p$ 与 $A_\infty$ 维数的结构性质。
- Proposition 2.44：标量 lower dimension 对应 reverse doubling，upper dimension 对应 doubling。
- Proposition 2.45：通过 $w(Q)/w(2^iQ)$ 与 $w(2^iQ)/w(Q)$ 计算 lower/upper critical dimensions。
- Proposition 2.46：给出标量权在不同 cubes 上的 sharp 比值估计。

### Sharp indices 与维数的关系

- 本小节后半部分进一步将维数与 critical self-improvement index、critical reverse Hölder index 联系起来。
- 核心思想：维数描述权在尺度放大时的增长，而 sharp indices 描述权在 $A_p$ 或 $RH_q$ 层级中的临界位置。
- 对标量权而言，这些量与 doubling/reverse doubling 行为密切相关；对矩阵权而言，必须通过 reducing operators 表达。
