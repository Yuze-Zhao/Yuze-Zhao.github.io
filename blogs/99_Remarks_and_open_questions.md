# Remarks and open questions 汇总

本文在各节中穿插了若干 remarks 和 open questions。这里按章节顺序汇总，便于后续写综述或准备报告。

## 第2节：权的结构理论

### Remarks

- **Remark 2.1**：$A_p$ 标量权定义中的 cube 可替换为 ball。
- **Remark 2.2**：标量权有 $A_\infty=\bigcup_{p<\infty}A_p=\bigcup_{q>1}RH_q$。
- **Remark 2.3**：
  - BLO 可由 $A_1$ 权的对数表示；
  - $BLO\cup(-BLO)$ 是 BMO 的真子集。
- **Remark 2.4**：Corollary 2.1(i) 可由 $A_p$ 类的开性质推出。
- **Remark 2.5**：sharp reverse Hölder inequality 中常数可取 2，且不依赖于权特征常数。
- **Remark 2.6**：reducing operators 的存在性已有文献保证。
- **Remark 2.7**：从三种平均量的等价性解释 $A_1$ 的“对偶型”刻画。
- **Remark 2.8**：Lemma 2.7 的局部结论可推广为全空间版本。
- **Remark 2.9**：矩阵 $A_p$ 的测试函数刻画在 $m=1$ 时退化为标量刻画。
- **Remark 2.10**：矩阵 $A_{p,\infty}$ 的自改进型结果在 $m=1$ 时退化为 $A_\infty=\bigcup A_p$。
- **Remark 2.11**：
  - Proposition 2.24 中若干矩阵结论在标量情形对应 $A_\infty$ 的等价刻画；
  - 这些矩阵结论是否都等价于 $A_{p,\infty}$ 仍不清楚；
  - scalarization 可能损失矩阵信息；
  - 某些标量 $A_\infty$ 刻画尚无矩阵对应版本。
- **Remark 2.12**：
  - 对 $0<p<1$，$A_p\subsetneqq\bigcap_{q>p}A_q$ 是否严格仍不清楚；
  - BMO/VMO 与权对数的标量刻画不能简单推广为矩阵元素逐项版本；
  - 权的维数可改进 doubling 型估计。
- **Remark 2.13**：矩阵权缺乏标量型自改进性质，因此 $q\to p^-$ 的极限通常不适合讨论；$q\to p^+$ 的 limsup 问题仍未知。
- **Remark 2.14**：$[0,n)$ 是 $A_p$-dimension 的有效范围。
- **Remark 2.15**：$A_{p,\infty}$ 的 lower/upper dimensions 给出两套不同分类，有效范围分别为 $[0,n)$ 与 $[0,\infty)$。

### Open questions

- **Question 2.1**：对 Bickel 等人构造的矩阵幂权，如何刻画其属于 $A_p$ 和 $A_{p,\infty}$ 的条件？
- **Question 2.2**：
  1. 矩阵 Jones factorization 中是否可用 $A_q$（$q<1$）替代 $A_1$？
  2. 对 $A_{p,\infty}$ 是否存在 Jones factorization 型结果？
  3. 是否可建立矩阵版本的乘积构造、凸组合/最大最小稳定性、Coifman-Rochberg 构造？
- **Question 2.3**：对矩阵权，是否有
  $$\lim_{q\to p^+}[W]_{A_q}=[W]_{A_p},\qquad \lim_{q\to p^+}[W]_{A_{q,\infty}}=[W]_{A_{p,\infty}}?$$

## 第3节：算子不等式

### Remarks

- **Remark 3.1**：Hardy-Littlewood 极大算子相关估计中的指数具有 sharpness。
- **Remark 3.2**：非退化卷积 Calderón-Zygmund 算子的标量加权估计中，$[w]_{A_p}^{\max\{1,1/(p-1)\}}$ 的指数 sharp。

### Open questions

- **Question 3.1**：是否可为 $p=1$ 引入合适的标量权类 $A_1^*$，刻画权相关极大算子从 $L^1$ 到弱 $L^1$ 的有界性？
- **Question 3.2**：是否存在合适的矩阵权类 $A_p^*$，刻画矩阵权相关极大算子 $M_{W,p}$ 从 $L^p$ 到 $L^{p,\infty}$ 的有界性？
- **Question 3.3**：Calderón-Zygmund 算子的弱型估计与 maximal truncation 估计中，某些 sharp bounds 仍待明确。
- **Question 3.4**：当 $p\in(1,2)\cup(2,\infty)$ 时，矩阵加权 Calderón-Zygmund 估计中的 sharp bound 仍未知。
- **Question 3.5**：若干矩阵加权 sparse/Calderón-Zygmund 型不等式中的 sharp bounds 是什么？
- **Question 3.6**：矩阵分数极大算子与分数积分算子的定量 bound 是否 sharp？

## 第4节：矩阵加权函数空间

### Remarks

- **Remark 4.1**：矩阵加权 Besov-Triebel-Lizorkin 型空间在特殊参数下退化为若干已有空间。
- **Remark 4.2**：若假设 $W\in A_p$，almost diagonal operator 的有界性条件中某些指数可通过 $A_p$-dimension 及对偶维数改进。

### Open questions

- **Question 4.1**：Theorem 4.6 是否在 $q\in(0,\min\{1,p\})$ 时仍成立？作者给出猜测，但目前尚未解决。

## 总体观察

1. 文章的 open questions 主要集中在矩阵情形与标量情形差异最大的位置：自改进、sharp constants、factorization 和 low-integrability 参数范围。
2. 矩阵 $A_{p,\infty}$ 是许多问题的关键对象，但其与标量 $A_\infty$ 的完全平行理论尚未建立。
3. 权的维数理论是解决矩阵加权函数空间问题的重要工具，也为刻画 reducing operators 的增长提供了统一语言。
4. Calderón-Zygmund 算子的矩阵加权 sharp estimates 是当前理论中最突出、也最能体现矩阵现象本质差异的问题之一。
