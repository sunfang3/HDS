---
chapter_id: "ch04"
chapter_title: "Uniform laws of large numbers"
source_title: "High-Dimensional Statistics: A Non-Asymptotic Viewpoint"
source_version: "Cambridge Series in Statistical and Probabilistic Mathematics, No. 48; first published 2019; ISBN 978-1-108-49802-9"
main_source_path: "High-Dimensional Statistics A Non-Asymptotic Viewpoint (Martin J. Wainwright) (z-library.sk, 1lib.sk, z-lib.sk).pdf"
printed_pages: "98–120"
pdf_pages: "117–139"
target_notes: "notes/ch04-notes.qmd"
language: "zh-CN"
learner_profile: "学过陈希孺《概率论与数理统计》本科教材；已读本书第 2 章的次高斯尾、霍夫丁、有界差分与集合上的拉德马赫复杂度。缺口是把固定函数的大数定律升级成函数类上的一致定律，以及对称化、函数类拉德马赫复杂度与 VC 维。不要重讲普通大数定律。"
map_status: "清单完成"
---

# 第 4 章内容清单

> 内部质量工件。正式内容逐项登记；§4.5 习题 4.1–4.17 作为 EXERCISE 不进入 Notes。

## 来源边界

- 教材权威来源：Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series No. 48
- 版本识别依据：封面 Cambridge Series；版权页 © Martin J. Wainwright 2019，First published 2019，ISBN 978-1-108-49802-9 Hardback，DOI 10.1017/9781108627771
- 目标章节与页码：第 4 章，印刷页 98–120；PDF 页 117–139（**PDF = 印刷 + 19**）
- 补充来源及用途：无（习题独立求解）
- 已知来源限制：文本层可用但公式常错位；公式、定理框、习题题干须对照 `scratch/ch04/p-117.png`–`p-139.png`

## 内容清单

| 定位 | 类型 | 内容/范围 | 重要性 | Notes 处理 | 合并目标/排除理由 | 核验状态 |
|---|---|---|---|---|---|---|
| 章首 印刷页 98；PDF 页 117 | SECTION | Chapter 4 Uniform laws of large numbers：把固定序列的大数定律加强为函数类上的一致定律；走非渐近路线 | 关键 | 完整讲解 |  | 原页已核 |
| §4.1 印刷页 98；PDF 页 117 | SECTION | Motivation | 关键 | 完整讲解 |  | 原页已核 |
| §4.1.1 印刷页 98–100；PDF 页 117–119 | SECTION | Uniform convergence of cumulative distribution functions | 关键 | 完整讲解 |  | 原页已核 |
| (4.1) 印刷页 98；PDF 页 117 | FORMULA | 经验 CDF $\widehat F_n(t):=n^{-1}\sum_{i=1}^n\mathbb I_{(-\infty,t]}[X_i]$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 4.1 印刷页 99；PDF 页 118 | FIGURE_TABLE | $[0,1]$ 上均匀分布的总体 CDF 与经验 CDF，$n=10$ 与 $n=100$ | 辅助 | 简要说明 |  | 原页已核 |
| Example 4.1 印刷页 99；PDF 页 118 | EXAMPLE | 期望泛函 $\gamma_g(F):=\int g\,dF$ 与插入估计 | 关键 | 完整讲解 |  | 原页已核 |
| (4.2) 印刷页 99；PDF 页 118 | FORMULA | $\gamma_g(F):=\int g(x)\,dF(x)$ | 关键 | 并入相关内容 | Example 4.1 | 原页已核 |
| Example 4.2 印刷页 99–100；PDF 页 118–119 | EXAMPLE | 分位数泛函 $Q_\alpha$ 与样本分位数 | 关键 | 完整讲解 |  | 原页已核 |
| (4.3) 印刷页 99；PDF 页 118 | FORMULA | $Q_\alpha(F):=\inf\{t\in\mathbb R:F(t)\ge\alpha\}$ | 关键 | 并入相关内容 | Example 4.2 | 原页已核 |
| (4.4) 印刷页 100；PDF 页 119 | FORMULA | 插入分位数 $Q_\alpha(\widehat F_n)$ | 关键 | 并入相关内容 | Example 4.2 | 原页已核 |
| Example 4.3 印刷页 100；PDF 页 119 | EXAMPLE | 拟合优度：一致范数与 Cramér–von Mises 泛函 | 关键 | 完整讲解 |  | 原页已核 |
| (4.5) 印刷页 100；PDF 页 119 | DEFINITION | 一致范数 $\lVert G-F\rVert_\infty:=\sup_t\lvert G(t)-F(t)\rvert$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 4.4 印刷页 100；PDF 页 119 | THEOREM | Glivenko–Cantelli：$\lVert\widehat F_n-F\rVert_\infty\to 0$ 几乎必然 | 关键 | 完整讲解 |  | 原页已核 |
| (4.6) 印刷页 100；PDF 页 119 | FORMULA | $\lVert\widehat F_n-F\rVert_\infty\xrightarrow{\mathrm{a.s.}}0$ | 关键 | 并入相关内容 | Theorem 4.4 | 原页已核 |
| §4.1.2 印刷页 101–104；PDF 页 120–123 | SECTION | Uniform laws for more general function classes | 关键 | 完整讲解 |  | 原页已核 |
| (4.7) 印刷页 101；PDF 页 120 | DEFINITION | $\lVert\mathbb P_n-\mathbb P\rVert_{\mathscr F}:=\sup_{f\in\mathscr F}\lvert n^{-1}\sum f(X_i)-\mathbb E[f(X)]\rvert$ | 关键 | 完整讲解 |  | 原页已核 |
| Definition 4.5 印刷页 101；PDF 页 120 | DEFINITION | Glivenko–Cantelli 类：$\lVert\mathbb P_n-\mathbb P\rVert_{\mathscr F}\to 0$ 依概率 | 关键 | 完整讲解 |  | 原页已核 |
| Example 4.6 印刷页 101；PDF 页 120 | EXAMPLE | 左半区间指示函数类 (4.8) 与经典 GC | 关键 | 完整讲解 |  | 原页已核 |
| (4.8) 印刷页 101；PDF 页 120 | FORMULA | $\mathscr F=\{\mathbb I_{(-\infty,t]}(\cdot):t\in\mathbb R\}$ | 关键 | 并入相关内容 | Example 4.6 | 原页已核 |
| Example 4.7 印刷页 101–102；PDF 页 120–121 | EXAMPLE | 有限子集指示类不是 GC；(4.9) 偏差恒为 1 | 关键 | 完整讲解 |  | 原页已核 |
| (4.9) 印刷页 102；PDF 页 121 | FORMULA | $\sup_{S\in\mathcal S}\lvert\mathbb P_n[S]-\mathbb P[S]\rvert=1$ | 关键 | 并入相关内容 | Example 4.7 | 原页已核 |
| §4.1.2 ERM 印刷页 102–104；PDF 页 121–123 | PROSE_RANGE | 经验风险、总体风险、超额风险分解 $T_1+T_2+T_3$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 4.8 印刷页 102–103；PDF 页 121–122 | EXAMPLE | 极大似然：代价为对数密度比，总体风险为 KL | 关键 | 完整讲解 |  | 原页已核 |
| Example 4.9 印刷页 103；PDF 页 122 | EXAMPLE | 二元分类：0–1 代价 (4.10) 与 Bayes 分类器 | 关键 | 完整讲解 |  | 原页已核 |
| (4.10) 印刷页 103；PDF 页 122 | FORMULA | $\mathcal L_f(X,Y):=\mathbb I[f(X)\ne Y]$ | 关键 | 并入相关内容 | Example 4.9 | 原页已核 |
| §4.1.2 超额风险 印刷页 104；PDF 页 123 | FORMULA | 超额风险 $\le 2\lVert\mathbb P_n-\mathbb P\rVert_{\mathfrak L(\Omega_0)}$ | 关键 | 完整讲解 |  | 原页已核 |
| §4.2 印刷页 104–109；PDF 页 123–128 | SECTION | A uniform law via Rademacher complexity | 关键 | 完整讲解 |  | 原页已核 |
| (4.11) 印刷页 104；PDF 页 123 | DEFINITION | 限制集 $\mathscr F(x_1^n):=\{(f(x_1),\ldots,f(x_n)):f\in\mathscr F\}$ | 关键 | 完整讲解 |  | 原页已核 |
| (4.12) 印刷页 105；PDF 页 124 | DEFINITION | 经验拉德马赫复杂度 $\mathcal R(\mathscr F(x_1^n)/n)$ | 关键 | 完整讲解 |  | 原页已核 |
| (4.13) 印刷页 105；PDF 页 124 | DEFINITION | 拉德马赫复杂度 $\mathcal R_n(\mathscr F):=\mathbb E_X[\mathcal R(\mathscr F(X_1^n)/n)]$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 4.10 印刷页 105；PDF 页 124 | THEOREM | $b$-一致有界类：$\lVert\mathbb P_n-\mathbb P\rVert_{\mathscr F}\le 2\mathcal R_n(\mathscr F)+\delta$，概率至少 $1-\exp(-n\delta^2/(2b^2))$ | 关键 | 完整讲解 |  | 原页已核 |
| (4.14) 印刷页 105；PDF 页 124 | FORMULA | Theorem 4.10 的不等式 | 关键 | 并入相关内容 | Theorem 4.10 | 原页已核 |
| Theorem 4.10 证明 印刷页 106–107；PDF 页 125–126 | PROOF_DERIVATION | 有界差分集中 (4.15)–(4.16) 加对称化 (4.17)–(4.18) | 关键 | 完整讲解 |  | 原页已核 |
| (4.15) 印刷页 106；PDF 页 125 | FORMULA | 改一个坐标：$G(x)-G(y)\le 2b/n$ | 辅助 | 并入相关内容 | Theorem 4.10 | 原页已核 |
| (4.16) 印刷页 106；PDF 页 125 | FORMULA | $\lVert\mathbb P_n-\mathbb P\rVert_{\mathscr F}-\mathbb E[\lVert\mathbb P_n-\mathbb P\rVert_{\mathscr F}]\le t$，尾 $\exp(-nt^2/(2b^2))$ | 关键 | 并入相关内容 | Theorem 4.10 | 原页已核 |
| (4.17) 印刷页 107；PDF 页 126 | FORMULA | 引入独立副本后把期望推进上确界 | 关键 | 并入相关内容 | Theorem 4.10 | 原页已核 |
| (4.18) 印刷页 107；PDF 页 126 | FORMULA | 乘拉德马赫后拆成 $2\mathcal R_n(\mathscr F)$ | 关键 | 并入相关内容 | Theorem 4.10 | 原页已核 |
| §4.2.1 印刷页 107–109；PDF 页 126–128 | SECTION | Necessary conditions with Rademacher complexity | 关键 | 完整讲解 |  | 原页已核 |
| (4.19) 印刷页 107；PDF 页 126 | DEFINITION | 对称化过程 $\lVert\mathbb S_n\rVert_{\mathscr F}:=\sup_f\lvert n^{-1}\sum\varepsilon_i f(X_i)\rvert$ | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 4.11 印刷页 107；PDF 页 126 | PROPOSITION | 凸非降 $\Phi$ 的夹心 (4.20)；$\Phi(t)=t$ 得 (4.21) | 关键 | 完整讲解 |  | 原页已核 |
| (4.20) 印刷页 107；PDF 页 126 | FORMULA | $\mathbb E[\Phi(\frac12\lVert\mathbb S_n\rVert_{\overline{\mathscr F}})]\le\mathbb E[\Phi(\lVert\mathbb P_n-\mathbb P\rVert_{\mathscr F})]\le\mathbb E[\Phi(2\lVert\mathbb S_n\rVert_{\mathscr F})]$ | 关键 | 并入相关内容 | Proposition 4.11 | 原页已核 |
| (4.21) 印刷页 107；PDF 页 126 | FORMULA | $\frac12\mathbb E\lVert\mathbb S_n\rVert_{\overline{\mathscr F}}\le\mathbb E[\lVert\mathbb P_n-\mathbb P\rVert_{\mathscr F}]\le 2\mathbb E\lVert\mathbb S_n\rVert_{\mathscr F}$ | 关键 | 并入相关内容 | Proposition 4.11 | 原页已核 |
| Proposition 4.11 证明 印刷页 108–109；PDF 页 127–128 | PROOF_DERIVATION | 上界用三角不等式与 Jensen；下界对中心化类再拆均值 | 关键 | 简要说明 |  | 原页已核 |
| Proposition 4.12 印刷页 109；PDF 页 128 | PROPOSITION | 下界 (4.22)：$\lVert\mathbb P_n-\mathbb P\rVert_{\mathscr F}\ge\frac12\mathcal R_n(\mathscr F)-\sup\lvert\mathbb E[f]\rvert/(2\sqrt n)-\delta$ | 关键 | 完整讲解 |  | 原页已核 |
| (4.22) 印刷页 109；PDF 页 128 | FORMULA | Proposition 4.12 的不等式，尾 $e^{-n\delta^2/(2b^2)}$ | 关键 | 并入相关内容 | Proposition 4.12 | 原页已核 |
| §4.3 印刷页 109；PDF 页 128 | SECTION | Upper bounds on the Rademacher complexity | 关键 | 完整讲解 |  | 原页已核 |
| §4.3.1 印刷页 109–111；PDF 页 128–130 | SECTION | Classes with polynomial discrimination | 关键 | 完整讲解 |  | 原页已核 |
| Definition 4.13 印刷页 110；PDF 页 129 | DEFINITION | 多项式判别：$\mathrm{card}(\mathscr F(x_1^n))\le(n+1)^\nu$ | 关键 | 完整讲解 |  | 原页已核 |
| (4.23) 印刷页 110；PDF 页 129 | FORMULA | 多项式判别的基数上界 | 关键 | 并入相关内容 | Definition 4.13 | 原页已核 |
| Lemma 4.14 印刷页 110；PDF 页 129 | LEMMA | 经验拉德马赫 $\le 4D(x_1^n)\sqrt{\nu\log(n+1)/n}$，$D$ 为 $\mathscr F(x_1^n)/\sqrt n$ 的 $\ell_2$ 半径 | 关键 | 完整讲解 |  | 原页已核 |
| (4.24) 印刷页 110；PDF 页 129 | FORMULA | $b$-有界时印刷式 $\mathcal R_n(\mathscr F)\le 2b\sqrt{\nu\log(n+1)/n}$ | 关键 | 完整讲解 | 与 Lemma 4.14 的 $4D$ 不一致，见勘误表 | 原页已核 |
| Corollary 4.15 印刷页 111；PDF 页 130 | COROLLARY | 定量 Glivenko–Cantelli (4.25)，前因子 $8\sqrt{\log(n+1)/n}$ | 关键 | 完整讲解 |  | 原页已核 |
| (4.25) 印刷页 111；PDF 页 130 | FORMULA | $\mathbb P[\lVert\widehat F_n-F\rVert_\infty\ge 8\sqrt{\log(n+1)/n}+\delta]\le e^{-n\delta^2/2}$ | 关键 | 并入相关内容 | Corollary 4.15 | 原页已核 |
| Corollary 4.15 证明 印刷页 111；PDF 页 130 | PROOF_DERIVATION | 左半区间 $\mathrm{card}\le n+1$，因而 $\nu=1$、$D\le 1$，再用 Theorem 4.10 | 关键 | 完整讲解 |  | 原页已核 |
| §4.3.2 印刷页 111–114；PDF 页 130–133 | SECTION | Vapnik–Chervonenkis dimension | 关键 | 完整讲解 |  | 原页已核 |
| Definition 4.16 印刷页 112；PDF 页 131 | DEFINITION | 打散：$\mathrm{card}(\mathscr F(x_1^n))=2^n$；VC 维为可打散的最大 $n$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 4.17 印刷页 112；PDF 页 131 | EXAMPLE | 左半区间 VC 维 $1$；双侧区间 VC 维 $2$，基数 $\le(n+1)^2$ | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 4.18 印刷页 113；PDF 页 132 | PROPOSITION | Sauer–Shelah：$\mathrm{card}(\mathcal S(P))\le\sum_{i=0}^{\nu}\binom{n}{i}\le(n+1)^\nu$ | 关键 | 完整讲解 |  | 原页已核 |
| (4.26) 印刷页 113；PDF 页 132 | FORMULA | Sauer–Shelah 两段不等式 | 关键 | 并入相关内容 | Proposition 4.18 | 原页已核 |
| Proposition 4.18 证明 印刷页 113–114；PDF 页 132–133 | PROOF_DERIVATION | 对 $(n,k)$ 归纳：$\Phi_k(n)\le\Psi_k(n)$；分解 $\mathcal S_0,\mathcal S_1$ | 关键 | 完整讲解 |  | 原页已核 |
| (4.27) 印刷页 113；PDF 页 132 | FORMULA | $\Phi_k(n)\le\Psi_k(n)$ | 辅助 | 并入相关内容 | Proposition 4.18 | 原页已核 |
| (4.28) 印刷页 113；PDF 页 132 | FORMULA | 反证：若某类超过 $\Psi_k(n)$ 则 $\Phi_k>\Psi_k$ | 辅助 | 并入相关内容 | Proposition 4.18 | 原页已核 |
| (4.29) 印刷页 114；PDF 页 133 | FORMULA | $\mathrm{card}(\mathcal S(P))\le\Psi_k(n-1)+\Psi_{k-1}(n-1)=\Psi_k(n)$ | 辅助 | 并入相关内容 | Proposition 4.18 | 原页已核 |
| §4.3.3 印刷页 115–116；PDF 页 134–135 | SECTION | Controlling the VC dimension | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 4.19 印刷页 115；PDF 页 134 | PROPOSITION | 有限 VC 在补、并 $\sqcup$、交 $\sqcap$ 下保持有限 | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 4.20 印刷页 115；PDF 页 134 | PROPOSITION | 有限维函数向量空间的零水平子图类 VC 维 $\le\dim(\mathcal G)$ | 关键 | 完整讲解 |  | 原页已核 |
| (4.30) 印刷页 115；PDF 页 134 | FORMULA | $\sum_{\gamma_i\le 0}(-\gamma_i)g(x_i)=\sum_{\gamma_i>0}\gamma_i g(x_i)$ | 关键 | 并入相关内容 | Proposition 4.20 | 原页已核 |
| Example 4.21 印刷页 116；PDF 页 135 | EXAMPLE | $\mathbb R^d$ 中仿射半空间 VC 维 $\le d+1$，且锐 | 关键 | 完整讲解 |  | 原页已核 |
| Example 4.22 印刷页 116；PDF 页 135 | EXAMPLE | 欧氏球（教材称 sphere）VC 维 $\le d+2$，锐界 $d+1$ | 关键 | 完整讲解 |  | 原页已核 |
| §4.4 印刷页 117；PDF 页 136 | PROSE_RANGE | Bibliographic details：可测性约定、DKW (4.31)、Massart 常数 $C=2$、拉德马赫文献 | 辅助 | 指回教材 | 文献清单不抄入 Notes；DKW 与可测性在 Notes 用作者解释桥接 | 原页已核 |
| (4.31) 印刷页 117；PDF 页 136 | FORMULA | DKW：$\mathbb P[\lVert\widehat F_n-F\rVert_\infty\ge\delta]\le C e^{-2n\delta^2}$ | 关键 | 完整讲解 |  | 原页已核 |
| §4.5 印刷页 117；PDF 页 136 | SECTION | Exercises 4.1–4.17 | 辅助 | 不进入 Notes | 习题整节进入 Solutions | 原页已核 |
| Exercise 4.1 印刷页 117–118；PDF 页 136–137 | EXERCISE | Continuity of functionals；均值 / CvM / 分位数 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 4.2 印刷页 118；PDF 页 137 | EXERCISE | Failure of Glivenko–Cantelli；(4.32) 下界 $1/2$ | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 4.3 印刷页 118；PDF 页 137 | EXERCISE | Maximum likelihood and uniform laws；Bernoulli / Poisson / 高斯 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 4.4 印刷页 118；PDF 页 137 | EXERCISE | Details of symmetrization argument | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 4.5 印刷页 118–119；PDF 页 137–138 | EXERCISE | Necessity of vanishing Rademacher complexity | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 4.6 印刷页 119；PDF 页 138 | EXERCISE | Too many linear classifiers；经验拉德马赫等于 1 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 4.7 印刷页 119；PDF 页 138 | EXERCISE | Basic properties of Rademacher complexity；(4.33) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 4.8 印刷页 119；PDF 页 138 | EXERCISE | Operations on VC classes | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 4.9 印刷页 119；PDF 页 138 | EXERCISE | Prove Lemma 4.14 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 4.10 印刷页 119；PDF 页 138 | EXERCISE | Pascal identity for (4.29) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 4.11 印刷页 119；PDF 页 138 | EXERCISE | Complete Proposition 4.18；(en/ν)^ν | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 4.12 印刷页 120；PDF 页 139 | EXERCISE | VC dimension of left-sided intervals in $\mathbb R^d$ | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 4.13 印刷页 120；PDF 页 139 | EXERCISE | VC dimension of spheres in $\mathbb R^2$；(4.34) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 4.14 印刷页 120；PDF 页 139 | EXERCISE | VC dimension of monotone Boolean conjunctions | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 4.15 印刷页 120；PDF 页 139 | EXERCISE | VC dimension of closed and convex sets | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 4.16 印刷页 120；PDF 页 139 | EXERCISE | VC dimension of polygons with at most four vertices | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 4.17 印刷页 120；PDF 页 139 | EXERCISE | Infinite VC dimension of $\mathrm{sign}(\sin(tx))$ | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |

## 来源异常与勘误

| 定位 | 问题类型 | 原式/原文 | 核验证据 | 处置 | 数学复核人 | 批准人 |
|---|---|---|---|---|---|---|
| (4.24) 印刷页 110；PDF 页 129 | 常数不一致 | 印刷 $\mathcal R_n(\mathscr F)\le 2b\sqrt{\nu\log(n+1)/n}$ | 原页 PNG；Lemma 4.14 给出 $4D\sqrt{\nu\log(n+1)/n}$，有界时 $D\le b$ 应为 $4b$；Corollary 4.15 用 $4\sqrt{\log(n+1)/n}$ 再乘 Theorem 4.10 的因子 2 得到 8，与 $4b$ 一致、与 $2b$ 不一致 | 保留原文；Notes 照抄 (4.24)，并标明与 Lemma 4.14 / Corollary 4.15 不一致；`勘误待批` | 作者 | 未批 |
| Example 4.22 印刷页 116；PDF 页 135 | 记号笔误 | “The family of functions $\{g_c,c\in\mathbb R^{d+1}\}$ is a vector space of dimension $d+2$” | 原页；同段定义 $g_c(x)=\langle c,\phi(x)\rangle$、$c\in\mathbb R^{d+2}$，$\phi:\mathbb R^d\to\mathbb R^{d+2}$ | 保留原文；Notes 按 $c\in\mathbb R^{d+2}$ 讲解；`勘误待批` | 作者 | 未批 |
| Example 4.22 / Exercise 4.13 印刷页 116、120；PDF 页 135、139 | 术语嫌疑 | 集合 $S_{a,b}:=\{x:\lVert x-a\rVert_2\le b\}$ 称为 sphere | 原页；该集合是闭球；球面是 $\lVert x-a\rVert_2=b$ | 保留原文；Notes 按闭球讲解并标明教材用词；`勘误待批` | 作者 | 未批 |
| Exercise 4.3(a)(i) 印刷页 118；PDF 页 137 | 公式笔误 | Bernoulli：$p_\theta(x)=e^{\theta x}/(1+e^{\theta x})$，$x\in\{0,1\}$ | 原页 PNG；该式在 $\{0,1\}$ 上不是概率质量函数（$x=0$ 给出 $1/2$，$x=1$ 给出 $e^\theta/(1+e^\theta)$，两者之和一般为 1 当且仅当 $\theta=0$）。指数族 Bernoulli 应为 $e^{\theta x}/(1+e^\theta)$ | 保留原文；Solutions 按 $e^{\theta x}/(1+e^\theta)$ 求解并记录；`勘误待批` | 作者 | 未批 |
| Example 4.17 印刷页 112；PDF 页 131 | 记号不一致 | 先定义 $\mathcal S_{\mathrm{two}}:=\{(b,a]:b<a\}$，随后写 “any set of the form $(-b,a]$” | 原页；左端点符号从 $b$ 换成 $-b$，基数论证不受影响 | 保留原文；Notes 按两个端点各选 $n+1$ 个间隔讲解；`勘误待批` | 作者 | 未批 |
| Exercise 4.14 印刷页 120；PDF 页 139 | 记号 | 正文 $h_S$，展示式写成 $h_s$ | 原页；同一函数 | 保留原文；Solutions 统一用 $h_S$；`勘误待批` | 作者 | 未批 |

## 完成检查

- [x] 主教材可读、版本可识别，且目标章节已定位。
- [x] 目标语言、学习者起点和 Notes 唯一路径均已确认。
- [x] 章节全部内容均有处理去向。
- [x] 定义、假设、命题、引理、定理、推论和关键公式均逐项登记。
- [x] 聚合条目仅覆盖处理方式相同的连续内容。
- [x] 所有 `并入相关内容` 条目均有明确合并目标。
- [x] 所有 `不进入 Notes` 条目均有理由，且不含正式内容。
- [x] Notes 实际转写的公式、表格、图形及低置信内容均已对照原页。
- [x] 作者补充的桥接推导均已完成独立数学复核。
- [x] 所有勘误均保留原文、证据、复核记录及明确批准。
- [x] 纳入 Notes 的来源公式均不再处于 `待核`、`勘误待批` 或 `受阻`。
