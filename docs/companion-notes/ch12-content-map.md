---
chapter_id: "ch12"
chapter_title: "Reproducing kernel Hilbert spaces"
source_title: "High-Dimensional Statistics: A Non-Asymptotic Viewpoint"
source_version: "Cambridge Series in Statistical and Probabilistic Mathematics, No. 48; first published 2019; ISBN 978-1-108-49802-9"
main_source_path: "High-Dimensional Statistics A Non-Asymptotic Viewpoint (Martin J. Wainwright) (z-library.sk, 1lib.sk, z-lib.sk).pdf"
printed_pages: "383–415"
pdf_pages: "402–434"
target_notes: "notes/ch12-notes.qmd"
language: "zh-CN"
learner_profile: "学过陈希孺《概率论与数理统计》本科教材；熟悉欧氏内积、正交投影与多元正态；首次需要把函数空间上的优化写成再生核希尔伯特空间，并用核矩阵把无穷维问题降成 n 维线性代数。"
map_status: "清单完成"
---

# 第 12 章内容清单

> 内部质量工件。正式内容逐项登记；习题整节不进入 Notes；文献节聚合。

## 来源边界

- 教材权威来源：Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series No. 48
- 版本识别依据：封面 Cambridge Series；版权页 © Martin J. Wainwright 2019，First published 2019，ISBN 978-1-108-49802-9 Hardback，DOI 10.1017/9781108627771
- 目标章节与页码：第 12 章，印刷页 383–415；PDF 页 402–434（**PDF = 印刷 + 19**）
- 补充来源及用途：无（§12.8 习题独立求解）
- 已知来源限制：文本层可用但公式常错位；公式、图注须对照 `scratch/ch12/p-4XX.png`

## 内容清单

| 定位 | 类型 | 内容/范围 | 重要性 | Notes 处理 | 合并目标/排除理由 | 核验状态 |
|---|---|---|---|---|---|---|
| 章首 印刷页 383；PDF 页 402 | SECTION | Chapter 12 RKHS：插值、回归、密度估计等函数空间优化的核框架 | 关键 | 完整讲解 |  | 原页已核 |
| §12.1 印刷页 383–385；PDF 页 402–404 | SECTION | Basics of Hilbert spaces | 关键 | 完整讲解 |  | 原页已核 |
| Definition 12.1 印刷页 383；PDF 页 402 | DEFINITION | 内积 (12.1a)–(12.1c)：对称、正定、线性 | 关键 | 完整讲解 |  | 原页已核 |
| §12.1 印刷页 383；PDF 页 402 | FORMULA | 内积诱导范数 $\Vertf\Vert_V=\sqrt{\langle f,f\rangle}$；Cauchy 列 | 关键 | 完整讲解 |  | 原页已核 |
| Definition 12.2 印刷页 384；PDF 页 403 | DEFINITION | Hilbert 空间：完备内积空间 | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.3 印刷页 384；PDF 页 403 | EXAMPLE | $\ell^2(\mathbb N)$ 与 $\mathbb R^m$ 作为切片 | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.4 印刷页 384；PDF 页 403 | EXAMPLE | $L^2[0,1]$、Parseval、与 $\ell^2(\mathbb N)$ 同构；可分 Hilbert | 关键 | 完整讲解 |  | 原页已核 |
| §12.1 印刷页 385；PDF 页 404 | DEFINITION | 有界线性泛函；由内积给出的泛函 | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 12.5 印刷页 385；PDF 页 404 | THEOREM | 里斯表示定理：有界线性泛函有唯一表示元 | 关键 | 完整讲解 |  | 原页已核 |
| §12.2 印刷页 385–394；PDF 页 404–413 | SECTION | Reproducing kernel Hilbert spaces | 关键 | 完整讲解 |  | 原页已核 |
| §12.2.1 印刷页 386–387；PDF 页 405–406 | SECTION | Positive semidefinite kernel functions | 关键 | 完整讲解 |  | 原页已核 |
| Definition 12.6 印刷页 386；PDF 页 405 | DEFINITION | 正半定核：所有有限 Gram 矩阵正半定 | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.7 印刷页 386；PDF 页 405 | EXAMPLE | 线性核 $\mathcal K(x,x')=\langle x,x'\rangle$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.8 / (12.2) 印刷页 386；PDF 页 405 | FORMULA | 齐次/非齐次多项式核；二次特征映射 $\Phi$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.9 印刷页 386–387；PDF 页 405–406 | EXAMPLE | 高斯核 $\exp(-\Vertx-z\Vert_2^2/(2\sigma^2))$ | 关键 | 完整讲解 |  | 原页已核 |
| §12.2.2 印刷页 387–388；PDF 页 406–407 | SECTION | Feature maps in $\ell^2(\mathbb N)$；核技巧 | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.10 印刷页 387–388；PDF 页 406–407 | EXAMPLE | 由正交基与可和权重构造 PSD 核 $\sum\mu_j\phi_j(x)\phi_j(z)$ | 关键 | 完整讲解 |  | 原页已核 |
| §12.2.3 印刷页 388–390；PDF 页 407–409 | SECTION | 由核构造 RKHS | 关键 | 完整讲解 |  | 原页已核 |
| (12.3) 印刷页 388；PDF 页 407 | FORMULA | 再生性质 $\langle f,\mathcal K(\cdot,x)\rangle_{\mathbb H}=f(x)$ | 关键 | 完整讲解 |  | 原页已核 |
| (12.4) 印刷页 388；PDF 页 407 | FORMULA | 预 Hilbert 内积 $\langle f,\tilde f\rangle_{\widetilde{\mathbb H}}=\sum_{j,k}\alpha_j\tilde\alpha_k\mathcal K(x_j,\bar x_k)$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 12.11 印刷页 389；PDF 页 408 | THEOREM | 每个 PSD 核对应唯一 RKHS | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 12.11 证明 印刷页 389–390；PDF 页 408–409 | PROOF_DERIVATION | 正定性、完备化、唯一性；极化恒等式排版 | 辅助 | 简要说明 | 极化式与 $\Vertg_n-g_m\Vert$ 缺平方见勘误表 | 勘误待批 |
| §12.2.4 印刷页 390–394；PDF 页 409–413 | SECTION | 赋值泛函有界的抽象定义与更多例子 | 关键 | 完整讲解 |  | 原页已核 |
| Definition 12.12 印刷页 390；PDF 页 409 | DEFINITION | RKHS：赋值泛函点点有界 | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 12.13 印刷页 391；PDF 页 410 | THEOREM | 赋值有界的 Hilbert 空间有唯一 PSD 再生核 | 关键 | 完整讲解 |  | 原页已核 |
| (12.5) 印刷页 391；PDF 页 410 | FORMULA | $f(x)=\langle f,R_x\rangle_{\mathbb H}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.14 印刷页 391–392；PDF 页 410–411 | EXAMPLE | $\mathbb R^d$ 上线性函数的 RKHS；$\beta\in\mathbb R^m$ 笔误 | 关键 | 完整讲解 | 空间按 $\mathbb R^d$ 讲解；见勘误表 | 原页已核 |
| (12.6) 印刷页 392；PDF 页 411 | FORMULA | RKHS 范数收敛蕴含逐点收敛 | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.15 印刷页 392；PDF 页 411 | EXAMPLE | $L^2[0,1]$ 不是 RKHS；$f_n(x)=x^n$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.16 / (12.7)–(12.8) 印刷页 392–393；PDF 页 411–412 | EXAMPLE | 一阶索伯列夫 $\mathbb H^1[0,1]$，核 $\min\{x,z\}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.17 / (12.9)–(12.10) 印刷页 393–394；PDF 页 412–413 | EXAMPLE | 高阶索伯列夫与光滑样条核 | 关键 | 完整讲解 |  | 原页已核 |
| §12.3 印刷页 394–400；PDF 页 413–419 | SECTION | Mercer's theorem and its consequences | 关键 | 完整讲解 |  | 原页已核 |
| (12.11a)–(12.11b) 印刷页 394；PDF 页 413 | FORMULA | 核积分算子 $T_{\mathcal K}$ 与 Hilbert–Schmidt 条件 | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.18 / (12.12) 印刷页 395；PDF 页 414 | EXAMPLE | 离散计数测度下 PSD 矩阵的谱分解 | 辅助 | 简要说明 |  | 原页已核 |
| Example 12.19 印刷页 395；PDF 页 414 | EXAMPLE | $T_{\mathcal K}$ 作用于 $\min\{x,z\}$ | 辅助 | 并入相关内容 | 并入 Example 12.23 | 原页已核 |
| Theorem 12.20 印刷页 395；PDF 页 414 | THEOREM | 默塞尔定理：(12.13a)–(12.13b) 绝对一致收敛 | 关键 | 完整讲解 |  | 原页已核 |
| (12.14) 印刷页 396；PDF 页 415 | FORMULA | Mercer 特征映射 $x\mapsto(\sqrt{\mu_j}\phi_j(x))_j$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.21 印刷页 396；PDF 页 415 | EXAMPLE | 对称 PSD 矩阵的特征函数即特征向量 | 辅助 | 简要说明 |  | 原页已核 |
| Example 12.22 印刷页 396–397；PDF 页 415–416 | EXAMPLE | $(1+xz)^2$ 在 $[-1,1]$ 上的三角特征系统 | 辅助 | 简要说明 |  | 原页已核 |
| Example 12.23 印刷页 397；PDF 页 416 | EXAMPLE | 一阶索伯列夫：正弦特征函数与 $\mu_j=(2/((2j-1)\pi))^2$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.24 印刷页 397–398；PDF 页 416–417 | EXAMPLE | 平移不变核、卷积与余弦系数；换元处 $2\pi$/$\pi$ | 关键 | 完整讲解 | 计算按 $\pi j$ 讲解；见勘误表 | 原页已核 |
| Example 12.25 / (12.15)–(12.16) 印刷页 398–399；PDF 页 417–418 | EXAMPLE | 高斯核特征值 $\mu_j\asymp e^{-c j\log j}$ | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 12.26 / (12.17a)–(12.17b) 印刷页 399；PDF 页 418 | COROLLARY | Mercer 核的 RKHS 为加权 $\ell^2$ 椭球 | 关键 | 完整讲解 |  | 原页已核 |
| (12.18) 印刷页 399；PDF 页 418 | FORMULA | 单位球对应椭球 $\mathcal E$ | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 12.26 证明 印刷页 400；PDF 页 419 | PROOF_DERIVATION | $K(\cdot,x)\in\mathbb H$ 与再生性 | 辅助 | 简要说明 |  | 原页已核 |
| §12.4 印刷页 400–404；PDF 页 419–423 | SECTION | Operations on reproducing kernel Hilbert spaces | 关键 | 完整讲解 |  | 原页已核 |
| §12.4.1 印刷页 400–403；PDF 页 419–422 | SECTION | Sums of reproducing kernels | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 12.27 / (12.19) 印刷页 401；PDF 页 420 | PROPOSITION | $\mathbb H_1+\mathbb H_2$ 的核为 $K_1+K_2$，范数为最小分解 | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.28 印刷页 401；PDF 页 420 | EXAMPLE | 常数核加 $\min\{x,z\}$ 去掉 $f(0)=0$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.29 / (12.20)–(12.21) 印刷页 401–402；PDF 页 420–421 | EXAMPLE | 高阶索伯列夫的多项式直和扩张 | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.30 印刷页 402；PDF 页 421 | EXAMPLE | 可加模型与函数 ANOVA | 关键 | 完整讲解 |  | 原页已核 |
| (12.22) 印刷页 402；PDF 页 421 | FORMULA | 直和 $\mathbb F=\mathbb H_1\oplus\mathbb H_2$ 的范数 | 辅助 | 并入相关内容 | 并入 Proposition 12.27 证明梗概 | 原页已核 |
| Proposition 12.27 证明 印刷页 402–403；PDF 页 421–422 | PROOF_DERIVATION | $L_\perp^{-1}$ 与再生性；两内积之间缺加号 | 辅助 | 简要说明 | 见勘误表 | 勘误待批 |
| §12.4.2 印刷页 403–404；PDF 页 422–423 | SECTION | Tensor products | 关键 | 完整讲解 |  | 原页已核 |
| (12.23) 印刷页 403；PDF 页 422 | FORMULA | 张量积内积 | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 12.31 / (12.24) 印刷页 404；PDF 页 423 | PROPOSITION | 张量积 RKHS 的核为核的乘积 | 关键 | 完整讲解 |  | 原页已核 |
| §12.5 印刷页 405–409；PDF 页 424–428 | SECTION | Interpolation and fitting | 关键 | 完整讲解 |  | 原页已核 |
| §12.5.1 印刷页 405–406；PDF 页 424–425 | SECTION | Function interpolation | 关键 | 完整讲解 |  | 原页已核 |
| Figure 12.1 印刷页 405；PDF 页 424 | FIGURE_TABLE | $n=11$ 多项式核与一阶样条的无噪插值 | 辅助 | 简要说明 |  | 原页已核 |
| (12.25) 印刷页 405；PDF 页 424 | FORMULA | 极小范数插值 | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 12.32 印刷页 406；PDF 页 425 | PROPOSITION | 可行当且仅当 $y\in\mathrm{range}(\mathbf K)$；表示式 $\widehat f=n^{-1/2}\sum\widehat\alpha_i\mathcal K(\cdot,x_i)$ | 关键 | 完整讲解 |  | 原页已核 |
| §12.5.2 印刷页 407–409；PDF 页 426–428 | SECTION | Fitting via kernel ridge regression | 关键 | 完整讲解 |  | 原页已核 |
| (12.26)–(12.28) 印刷页 407；PDF 页 426 | FORMULA | 约束 / 惩罚形式的核岭回归 | 关键 | 完整讲解 | (12.28) 的 $1/(2n)$ 与证明 $1/n$ 不一致，见勘误表 | 原页已核 |
| Proposition 12.33 / (12.29)–(12.30) 印刷页 407；PDF 页 426 | PROPOSITION | KRR 的表示定理与 $\widehat\alpha=(\mathbf K+\lambda_n I_n)^{-1}y/\sqrt n$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 12.2 印刷页 408；PDF 页 427 | FIGURE_TABLE | $n=11$、$\lambda_n=0.10$ 的多项式与样条 KRR | 辅助 | 简要说明 |  | 原页已核 |
| Proposition 12.33 证明 印刷页 408–409；PDF 页 427–428 | PROOF_DERIVATION | 二次型与驻点 $\mathbf K(\mathbf K+\lambda I)\alpha=\mathbf K y/\sqrt n$ | 辅助 | 简要说明 | 目标函数用 $1/n$ 而非 (12.28) 的 $1/(2n)$ | 勘误待批 |
| §12.6 印刷页 409–411；PDF 页 428–430 | SECTION | Distances between probability measures | 关键 | 完整讲解 |  | 原页已核 |
| (12.31) 印刷页 409；PDF 页 428 | FORMULA | 积分概率伪度量 $\rho_{\mathcal F}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.34 印刷页 409；PDF 页 428 | EXAMPLE | Kolmogorov 距离 | 辅助 | 简要说明 |  | 原页已核 |
| Example 12.35 印刷页 409–410；PDF 页 428–429 | EXAMPLE | $\Vertf\Vert_\infty\le 1$ 给出两倍全变差 | 关键 | 完整讲解 |  | 原页已核 |
| (12.32) 印刷页 410；PDF 页 429 | FORMULA | 核均值差异（KMD）的闭式 | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.36 印刷页 410–411；PDF 页 429–430 | EXAMPLE | 线性核 KMD 为均值欧氏距离；二次齐次核为二阶矩 Frobenius | 关键 | 完整讲解 |  | 原页已核 |
| Example 12.37 印刷页 411；PDF 页 430 | EXAMPLE | $\min\{x,z\}$ 的 KMD | 辅助 | 简要说明 |  | 原页已核 |
| §12.7 印刷页 411–412；PDF 页 430–431 | PROSE_RANGE | Bibliographic details：Aronszajn、表示定理、Bochner、Widom、IPM | 辅助 | 指回教材 | 文献清单不抄入 Notes | 原页已核 |
| (12.33) 印刷页 412；PDF 页 431 | FORMULA | 逼近误差 $A(f^\ast;R)$ 与 $L^p$-universal | 辅助 | 简要说明 |  | 原页已核 |
| §12.8 印刷页 412–415；PDF 页 431–434 | SECTION | Exercises 12.1–12.20 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.1 印刷页 412；PDF 页 431 | EXERCISE | 有界线性泛函零空间闭 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.2 印刷页 412；PDF 页 431 | EXERCISE | 闭凸集上的投影；题干 $\inf\Vert\widehat g-f\Vert$ 排版 | 辅助 | 不进入 Notes | 按 $\inf_g\Vertg-f\Vert$ 求解；见勘误表 | 勘误待批 |
| Exercise 12.3 印刷页 412；PDF 页 431 | EXERCISE | 闭子空间的直和分解 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.4 印刷页 412；PDF 页 431 | EXERCISE | 再生核唯一 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.5 印刷页 412–413；PDF 页 431–432 | EXERCISE | 核的 Cauchy–Schwarz | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.6 印刷页 413；PDF 页 432 | EXERCISE | 线性核的特征函数与二阶矩矩阵 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.7 印刷页 413；PDF 页 432 | EXERCISE | 两个不同多项式核生成同一函数类 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.8 印刷页 413；PDF 页 432 | EXERCISE | 核的最小值 / 归一化内积，判断正误 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.9 印刷页 413；PDF 页 432 | EXERCISE | 左右乘函数保持 PSD | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.10 印刷页 413；PDF 页 432 | EXERCISE | 幂集核 $2^{\lvert A\cap B\rvert}$ | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.11 印刷页 413；PDF 页 432 | EXERCISE | 多项式核特征映射维数 $\binom{d+m}{m}$ | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.12 印刷页 413；PDF 页 432 | EXERCISE | 事件的协方差核 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.13 印刷页 414；PDF 页 433 | EXERCISE | 由集合核诱导幂集核 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.14 印刷页 414；PDF 页 433 | EXERCISE | 核有界蕴含单位球一致有界 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.15 印刷页 414；PDF 页 433 | EXERCISE | (12.20) 生成 (12.21) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.16 印刷页 414；PDF 页 433 | EXERCISE | Hadamard 积与核的乘积 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.17 印刷页 414；PDF 页 433 | EXERCISE | 全变差与 $\Vertf\Vert_\infty\le 1$ | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.18 印刷页 414；PDF 页 433 | EXERCISE | KMD 闭式 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.19 印刷页 414–415；PDF 页 433–434 | EXERCISE | 高斯核正半定 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 12.20 / (12.34) 印刷页 415；PDF 页 434 | EXERCISE | 核支持向量机的表示定理与对偶；对偶线性项 $1/n$ | 辅助 | 不进入 Notes | 完整解答写入 Solutions；对偶线性项见勘误表 | 勘误待批 |

## 来源异常与勘误

| 定位 | 问题类型 | 原式/原文 | 核验证据 | 处置 | 数学复核人 | 批准人 |
|---|---|---|---|---|---|---|
| Example 12.7 印刷页 386；PDF 页 405 | 笔误嫌疑 | $\alpha^T\mathbf K\alpha=\sum_{i,j}\alpha_i\alpha_j\langle x_i,x_j\rangle=\Vert\sum_i a_i x_i\Vert_2^2$ | 原页同一行 $\alpha_i$ 与 $a_i$ 混用 | 保留原文；Notes 按 $\alpha_i$ 解读；`勘误待批` | 作者 | 未批 |
| Theorem 12.11 证明 印刷页 390；PDF 页 409 | 笔误嫌疑 | $\Vertg_n-g_m\Vert_{\widetilde{\mathbb H}}=\Vertg_n\Vert^2+\Vertg_m\Vert^2-2\langle g_n,g_m\rangle$ | 原页左边是范数、右边是平方展开 | 保留原文；Notes 按平方范数理解；`勘误待批` | 作者 | 未批 |
| Theorem 12.11 证明 印刷页 390；PDF 页 409 | 笔误嫌疑 | $\langle f,g\rangle_{\mathbb H}:=\tfrac12\{\Vertf+g\Vert^2-\Vertf\Vert^2+\Vertg\Vert^2\}$ | 极化恒等式应为 $\tfrac12(\Vertf+g\Vert^2-\Vertf\Vert^2-\Vertg\Vert^2)$ | 保留原文；Notes 用正确极化式并标明；`勘误待批` | 作者 | 未批 |
| Example 12.14 印刷页 391；PDF 页 410 | 笔误嫌疑 | $f_\beta(\cdot)=\langle\cdot,\beta\rangle$，$\beta\in\mathbb R^m$ | 该例定义域是 $\mathbb R^d$ | 保留原文；Notes 写 $\beta\in\mathbb R^d$；`勘误待批` | 作者 | 未批 |
| Example 12.24 印刷页 398；PDF 页 417 | 笔误嫌疑 | 换元后写 $\cos(2\pi j(x+u))$，随后恒等式又用 $\cos(\pi j(x+u))$ | 原页同一段 $\pi$ 与 $2\pi$ 不一致；特征函数是 $\cos(\pi j x)$ | 保留原文；Notes 全程用 $\pi j$；`勘误待批` | 作者 | 未批 |
| Proposition 12.27 证明 印刷页 403；PDF 页 422 | 笔误嫌疑 | $\langle f_1,K_1(\cdot,x)\rangle_{\mathbb H_1}\langle f_2,K_2(\cdot,x)\rangle_{\mathbb H_2}=f_1(x)+f_2(x)$ | 原页两内积之间缺加号 | 保留原文；Notes 补加号；`勘误待批` | 作者 | 未批 |
| (12.28) 与证明 印刷页 407–409；PDF 页 426–428 | 笔误嫌疑 | (12.28) 用 $\tfrac1{2n}\sum(y_i-f(x_i))^2$；证明展开用 $\tfrac1n\Verty-\sqrt n\mathbf K\alpha\Vert_2^2$ | 驻点 $\mathbf K(\mathbf K+\lambda I)\alpha=\mathbf K y/\sqrt n$ 与 (12.30) 匹配的是 $1/n$ 而不是 $1/(2n)$ | 保留原文；(12.30) 按证明使用；`勘误待批` | 作者 | 未批 |
| Exercise 12.2 印刷页 412；PDF 页 431 | 笔误嫌疑 | $\Vert\widehat g-f\Vert_{\mathbb H}=\inf_{g\in\mathbb G}\Vert\widehat g-f\Vert_{\mathbb H}$ | 下确界应变元为 $g$；定义要求 $\Vert\widehat g-f\Vert=\inf_g\Vertg-f\Vert$ | 保留原文；Solutions 按标准投影定义求解；`勘误待批` | 作者 | 未批 |
| Exercise 12.20 印刷页 415；PDF 页 434 | 笔误嫌疑 | 对偶目标 $\tfrac1n\sum\alpha_i-\tfrac12\alpha^T\widetilde{\mathbf K}\alpha$，箱约束 $\alpha_i\in[0,1/(\lambda_n\sqrt n)]$ | 表示式带 $n^{-1/2}$ 时，拉格朗日对偶在同一箱约束下线性项为 $1/\sqrt n$（或带正因子 $\lambda_n$ 的等价式）；二次项与 $\widetilde{\mathbf K}$ 一致 | 保留原文；Solutions 按 $1/\sqrt n$ 推导并对照印刷式；`勘误待批` | 作者 | 未批 |

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
