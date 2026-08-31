---
chapter_id: "ch11"
chapter_title: "Graphical models for high-dimensional data"
source_title: "High-Dimensional Statistics: A Non-Asymptotic Viewpoint"
source_version: "Cambridge Series in Statistical and Probabilistic Mathematics, No. 48; first published 2019; ISBN 978-1-108-49802-9"
main_source_path: "High-Dimensional Statistics A Non-Asymptotic Viewpoint (Martin J. Wainwright) (z-library.sk, 1lib.sk, z-lib.sk).pdf"
printed_pages: "347–382"
pdf_pages: "366–401"
target_notes: "notes/ch11-notes.qmd"
language: "zh-CN"
learner_profile: "学过陈希孺《概率论与数理统计》本科教材，并已读本书第 2、6、7、9 章的尾界、样本协方差、Lasso 与可分解正则；首次需要把无向图模型的因子分解 / 条件独立与汉默斯利–克利福德定理接到高维图选择（图 Lasso、邻域回归、伊辛、损坏与隐变量）。"
map_status: "清单完成"
---

# 第 11 章内容清单

> 内部质量工件。正式定义、命题、定理、推论与编号公式逐项登记；长证明中的中间式按证明块聚合；§11.6 习题不进入 Notes。

## 来源边界

- 教材权威来源：Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series No. 48
- 版本识别依据：封面 Cambridge Series；版权页 © Martin J. Wainwright 2019，First published 2019，ISBN 978-1-108-49802-9 Hardback，DOI 10.1017/9781108627771
- 目标章节与页码：第 11 章，印刷页 347–382；PDF 页 366–401（**PDF = 印刷 + 19**）
- 补充来源及用途：无（习题独立求解）
- 已知来源限制：文本层可用但公式常错位；公式、图注须对照 `scratch/ch11/p-3XX.png`

## 内容清单

| 定位 | 类型 | 内容/范围 | 重要性 | Notes 处理 | 合并目标/排除理由 | 核验状态 |
|---|---|---|---|---|---|---|
| 章首 印刷页 347；PDF 页 366 | SECTION | Chapter 11 Graphical models for high-dimensional data：无向图模型与高维估计问题 | 关键 | 完整讲解 |  | 原页已核 |
| §11.1 印刷页 347；PDF 页 366 | SECTION | Some basics：无向图模型 / 马尔可夫随机场 | 关键 | 完整讲解 |  | 原页已核 |
| §11.1.1 印刷页 347–349；PDF 页 366–368 | SECTION | Factorization | 关键 | 完整讲解 |  | 原页已核 |
| §11.1.1 印刷页 347；PDF 页 366 | DEFINITION | 团、最大团；团相容函数 $\psi_C$ | 关键 | 完整讲解 |  | 原页已核 |
| Definition 11.1 / (11.1) 印刷页 348；PDF 页 367 | DEFINITION | 按图 $G$ 因子分解：$p(x)\propto\prod_{C\in\mathfrak C}\psi_C(x_C)$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 11.1 印刷页 348；PDF 页 367 | FIGURE_TABLE | (a) 最大团 $A,B,C,D$；(b) 顶点割集 $S$ | 辅助 | 简要说明 |  | 原页已核 |
| Example 11.2 印刷页 348–349；PDF 页 367–368 | EXAMPLE | 马尔可夫链的顶点–边因子分解与对称化分解 | 关键 | 完整讲解 |  | 原页已核 |
| Example 11.3 / (11.2) 印刷页 349；PDF 页 368 | EXAMPLE | 零均值高斯：$p\propto\sqrt{\det\Theta^*}\,\exp(-\tfrac12 x^T\Theta^* x)$；边团因子 | 关键 | 完整讲解 |  | 原页已核 |
| Example 11.4 / (11.3) 印刷页 349；PDF 页 368 | EXAMPLE | 伊辛模型（$X_j\in\{0,1\}$）及配分函数 $Z(\theta^*)$ | 关键 | 完整讲解 |  | 原页已核 |
| §11.1.2 印刷页 350；PDF 页 369 | SECTION | Conditional independence | 关键 | 完整讲解 |  | 原页已核 |
| (11.4) 印刷页 350；PDF 页 369 | DEFINITION | 顶点诱导子图的残边集 $E(V\setminus S)$；顶点割集 | 关键 | 完整讲解 |  | 原页已核 |
| Definition 11.5 印刷页 350；PDF 页 369 | DEFINITION | 关于图 $G$ 的马尔可夫性：$X_A\perp X_B\mid X_S$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 11.6 印刷页 350；PDF 页 369 | EXAMPLE | 链图：过去 $\perp$ 未来 $\mid$ 现在 | 关键 | 简要说明 |  | 原页已核 |
| Example 11.7 / (11.5) 印刷页 350；PDF 页 369 | EXAMPLE | 邻域 $\mathcal N(j)$ 是割集，分离 $\{j\}$ 与 $V\setminus\mathcal N^+(j)$ | 关键 | 完整讲解 |  | 原页已核 |
| §11.1.3 印刷页 351–352；PDF 页 370–371 | SECTION | Hammersley–Clifford equivalence | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 11.8 印刷页 351；PDF 页 370 | THEOREM | 严格正密度下因子分解 $\Leftrightarrow$ 马尔可夫性 | 关键 | 完整讲解 |  | 原页已核 |
| (11.6)–(11.7b) 印刷页 351–352；PDF 页 370–371 | PROOF_DERIVATION | 因子分解 $\Rightarrow$ 马尔可夫：团剖分与条件密度乘积 | 关键 | 完整讲解 |  | 原页已核 |
| HC 逆方向 印刷页 351；PDF 页 370 | PROSE_RANGE | 逆命题证明指向文献节 | 辅助 | 指回教材 | 逆方向不在正文展开 | 原页已核 |
| §11.1.4 印刷页 352；PDF 页 371 | SECTION | Estimation of graphical models：参数估计 vs 图选择 | 关键 | 完整讲解 |  | 原页已核 |
| §11.2 印刷页 352–353；PDF 页 371–372 | SECTION | Estimation of Gaussian graphical models | 关键 | 完整讲解 |  | 原页已核 |
| §11.2 / Figure 11.2 印刷页 352–353；PDF 页 371–372 | FIGURE_TABLE | 高斯 MRF：$\Theta^*_{jk}=0$ 当 $(j,k)\notin E$；链的三对角精度 | 关键 | 完整讲解 |  | 原页已核 |
| §11.2 印刷页 353；PDF 页 372 | FORMULA | 图选择误差 $\mathbb P[\widehat E\neq E]$；算子 / Frobenius 范数 | 关键 | 完整讲解 |  | 原页已核 |
| §11.2.1 印刷页 353–359；PDF 页 372–378 | SECTION | Graphical Lasso: $\ell_1$-regularized maximum likelihood | 关键 | 完整讲解 |  | 原页已核 |
| (11.8) 印刷页 354；PDF 页 373 | DEFINITION | $-\log\det(\Theta)=-\sum_j\log\gamma_j(\Theta)$（$\Theta\succ 0$），否则 $+\infty$ | 关键 | 完整讲解 |  | 原页已核 |
| (11.9) 印刷页 354；PDF 页 373 | FORMULA | 重标负对数似然 $\mathcal L_n(\Theta)=\langle\!\langle\Theta,\widehat\Sigma\rangle\!\rangle-\log\det\Theta$ | 关键 | 完整讲解 |  | 原页已核 |
| (11.10) 印刷页 354；PDF 页 373 | FORMULA | 图 Lasso：负对数似然加非对角 $\ell_1$ 罚 | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 11.9 / (11.11) 印刷页 355；PDF 页 374 | PROPOSITION | 图 Lasso 的 Frobenius 界；$\lambda_n=8\sigma^2(\sqrt{(\log d)/n}+\delta)$ | 关键 | 完整讲解 |  | 原页已核 |
| $\nabla\mathcal L_n$, $\nabla^2\mathcal L_n$ 印刷页 355；PDF 页 374 | FORMULA | $\nabla\mathcal L_n=\widehat\Sigma-\Theta^{-1}$，$\nabla^2\mathcal L_n=\Theta^{-1}\otimes\Theta^{-1}$ | 关键 | 完整讲解 |  | 原页已核 |
| (11.12) 印刷页 355；PDF 页 374 | FORMULA | RSC：$\mathcal E_n(\Delta)\ge(\kappa/2)$ 倍 Frobenius 平方，$\kappa=(\mathrm{op}(\Theta^*)+1)^{-2}$ | 关键 | 完整讲解 |  | 原页已核 |
| (11.13)–(11.14) 印刷页 356–357；PDF 页 375–376 | PROOF_DERIVATION | 子空间 Lipschitz、事件 $\mathbb G(\lambda_n)$、误差局部化 | 辅助 | 简要说明 |  | 原页已核 |
| (11.15) 印刷页 357；PDF 页 376 | ASSUMPTION | Hessian $\Gamma^*=\nabla^2\mathcal L_n(\Theta^*)$ 的 $\alpha$-不相干 | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 11.10 / (11.16) 印刷页 358；PDF 页 377 | PROPOSITION | 无假阳性与 $\ell_\infty$ 界；需 $n\gtrsim(1+8\alpha^{-1})^2 m^2\log d$ | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 11.11 / (11.17a)–(11.17b) 印刷页 358–359；PDF 页 377–378 | COROLLARY | 算子范数界；最大度 $m$ 时乘 $(m+1)$ | 关键 | 完整讲解 |  | 原页已核 |
| (11.18)–(11.19) 印刷页 359；PDF 页 378 | FORMULA | 逐元界与 Frobenius 推论 $\sqrt{2s+d}$ | 辅助 | 简要说明 |  | 原页已核 |
| §11.2.2 印刷页 359–365；PDF 页 378–384 | SECTION | Neighborhood-based methods | 关键 | 完整讲解 |  | 原页已核 |
| (11.20)–(11.21) 印刷页 360；PDF 页 379 | FORMULA | $X_j\perp X_{V\setminus\mathcal N^+(j)}\mid X_{\mathcal N(j)}$；高斯邻域回归 $X_j=\langle X_{\setminus j},\theta_j^*\rangle+W_j$ | 关键 | 完整讲解 |  | 原页已核 |
| ALGORITHM / (11.22) 印刷页 360–361；PDF 页 379–380 | ALGORITHM | 基于 Lasso 的邻域回归；AND / OR 规则 | 关键 | 完整讲解 |  | 原页已核 |
| (11.23) 印刷页 361；PDF 页 380 | ASSUMPTION | 协方差子矩阵关于 $S$ 的 $\alpha$-不相干 | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 11.12 印刷页 361–362；PDF 页 380–381 | THEOREM | 邻域 Lasso 图选择相合：无假边；显著边 $\lvert\Theta^*_{jk}\rvert\ge 7b\lambda_n$ | 关键 | 完整讲解 |  | 原页已核 |
| (11.24)–(11.31) 印刷页 362–365；PDF 页 381–384 | PROOF_DERIVATION | 随机设计的原对偶见证；对偶可行与 $\ell_\infty$ 误差 | 辅助 | 简要说明 | 完整计算指回教材 | 原页已核 |
| §11.3 印刷页 365–368；PDF 页 384–387 | SECTION | Graphical models in exponential form | 关键 | 完整讲解 |  | 原页已核 |
| (11.32)–(11.33) 印刷页 365；PDF 页 384 | FORMULA | 成对指数族因子分解；高斯 / 伊辛作为特例 | 关键 | 完整讲解 |  | 原页已核 |
| Example 11.13 / (11.34a)–(11.34b) 印刷页 365–366；PDF 页 384–385 | EXAMPLE | 波茨模型 | 辅助 | 简要说明 |  | 原页已核 |
| Example 11.14 / (11.35a)–(11.35b) 印刷页 366；PDF 页 385 | EXAMPLE | 泊松图模型；$\theta^*_{jk}\le 0$ 才能归一化 | 关键 | 完整讲解 |  | 原页已核 |
| §11.3.1 / (11.36)–(11.37) 印刷页 366–367；PDF 页 385–386 | FORMULA | 一般邻域回归：条件似然 + 块范数惩罚 | 关键 | 完整讲解 |  | 原页已核 |
| §11.3.2 / (11.38)–(11.39) 印刷页 367；PDF 页 386 | FORMULA | 伊辛邻域逻辑回归，$f(t)=\log(1+e^t)$ | 关键 | 完整讲解 |  | 原页已核 |
| (11.40) 印刷页 368；PDF 页 387 | ASSUMPTION | Fisher 信息 $J=\nabla^2\overline{\mathcal L}(\theta^*_{j+})$ 的 $\alpha$-不相干 | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 11.15 印刷页 368；PDF 页 387 | THEOREM | 伊辛邻域选择：$n>c_0 m^2\log d$；无假阳性与 $\ell_\infty$ 界 | 关键 | 完整讲解 |  | 原页已核 |
| §11.4 印刷页 368；PDF 页 387 | SECTION | Graphs with corrupted or hidden variables | 关键 | 完整讲解 |  | 原页已核 |
| §11.4.1 印刷页 368–373；PDF 页 387–392 | SECTION | Gaussian graph estimation with corrupted data | 关键 | 完整讲解 |  | 原页已核 |
| (11.41) 印刷页 369；PDF 页 388 | FORMULA | 朴素图 Lasso（用 $\widehat\Sigma_z$）一般不相合 | 关键 | 完整讲解 |  | 原页已核 |
| Example 11.16 / (11.42) 印刷页 369；PDF 页 388 | EXAMPLE | 加性噪声的无偏协方差 $\widehat\Gamma=n^{-1}Z^T Z-\Sigma_v$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 11.17 / (11.43) 印刷页 369；PDF 页 388 | EXAMPLE | 完全随机缺失的无偏协方差 | 关键 | 完整讲解 |  | 原页已核 |
| (11.44) 印刷页 369；PDF 页 388 | FORMULA | 校正图 Lasso | 关键 | 完整讲解 |  | 原页已核 |
| (11.45)–(11.47) 印刷页 370；PDF 页 389 | FORMULA | 损坏线性回归；总体 / 经验校正目标 | 关键 | 完整讲解 |  | 原页已核 |
| (11.48)–(11.49) 印刷页 371；PDF 页 390 | FORMULA | 校正 Lasso（罚 + $\ell_1$ 约束）；局部最优的变分不等式 | 关键 | 完整讲解 |  | 原页已核 |
| (11.50) 印刷页 371；PDF 页 390 | ASSUMPTION | 对可能非正定 $\widehat\Gamma$ 的限制特征值 | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 11.18 / (11.51)–(11.52) 印刷页 372；PDF 页 391 | PROPOSITION | 任一局部最优满足 $\ell_2$ 误差 $\le(2/\kappa)\sqrt{s}\,\lambda_n$ | 关键 | 完整讲解 |  | 原页已核 |
| (11.53)–(11.54) 印刷页 372–373；PDF 页 391–392 | PROOF_DERIVATION | 校正 Lasso 局部最优的误差控制 | 辅助 | 简要说明 |  | 原页已核 |
| §11.4.2 印刷页 373–376；PDF 页 392–395 | SECTION | Gaussian graph selection with hidden variables | 关键 | 完整讲解 |  | 原页已核 |
| (11.55)–(11.57) 印刷页 373–374；PDF 页 392–393 | FORMULA | 块精度、Schur 补：$(\Sigma^*_{OO})^{-1}=\Gamma^*-\Lambda^*$；观测模型 $Y=\Gamma^*-\Lambda^*+W$ | 关键 | 完整讲解 |  | 原页已核 |
| (11.58)–(11.60) 印刷页 374；PDF 页 393 | FORMULA | 硬阈值两步估计；尖峰约束；$\sqrt{\Theta^*}$ 的 $\ell_\infty$ 算子范数 | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 11.19 / (11.61a)–(11.61b) 印刷页 374–375；PDF 页 393–394 | PROPOSITION | $\widehat\Gamma$ 的 max-范数与 $\widehat\Lambda$ 的算子范数 | 关键 | 完整讲解 |  | 原页已核 |
| (11.62a)–(11.63) 印刷页 375–376；PDF 页 394–395 | PROOF_DERIVATION | 逆样本协方差的谱 / max 偏差及阈值论证 | 辅助 | 简要说明 |  | 原页已核 |
| §11.5 印刷页 376–378；PDF 页 395–397 | PROSE_RANGE | Bibliographic details：HC 史、图 Lasso、邻域、伊辛、校正、隐变量 | 辅助 | 指回教材 | 文献清单不抄入 Notes | 原页已核 |
| §11.6 印刷页 378–382；PDF 页 397–401 | SECTION | Exercises 11.1–11.13 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 11.1 印刷页 378–379；PDF 页 397–398 | EXERCISE | log-det 的严格凸、梯度、Hessian | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 11.2 印刷页 379；PDF 页 398 | EXERCISE | 高斯 MLE 为 $\widehat\Sigma^{-1}$，奇异时无定义 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 11.3 印刷页 379；PDF 页 398 | EXERCISE | 高斯邻域回归分解与 $\theta^*_{jk}=0$ | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 11.4 / (11.64)–(11.66) 印刷页 379–380；PDF 页 398–399 | EXERCISE | CLIME 估计量及其 $\ell_\infty$ 界 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 11.5 印刷页 380；PDF 页 399 | EXERCISE | 一般邻域回归在高斯下回到 (11.22) | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 11.6 印刷页 380；PDF 页 399 | EXERCISE | 条件分布只依赖 $\Theta_{j+}$ | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 11.7 / (11.67) 印刷页 380；PDF 页 399 | EXERCISE | $\{\pm 1\}$ 伊辛：矩与条件逻辑 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 11.8 印刷页 380；PDF 页 399 | EXERCISE | 加性噪声破坏马尔可夫性；路径填充 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 11.9 印刷页 380–381；PDF 页 399–400 | EXERCISE | 校正图 Lasso 存在唯一解的条件 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 11.10 印刷页 381；PDF 页 400 | EXERCISE | 未校正 Lasso 即使 $n\to\infty$ 也不相合 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 11.11 印刷页 381；PDF 页 400 | EXERCISE | 无 $\ell_1$ 半径时校正 Lasso 可不达全局最小 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 11.12 印刷页 381；PDF 页 400 | EXERCISE | 加性损坏下 $\widehat\Gamma,\widehat\gamma$ 无偏、偏差与 RE | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 11.13 印刷页 381–382；PDF 页 400–401 | EXERCISE | 缺失数据下的对应结论 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |

## 来源异常与勘误

| 定位 | 问题类型 | 原式/原文 | 核验证据 | 处置 | 数学复核人 | 批准人 |
|---|---|---|---|---|---|---|
| Proposition 11.9 / (11.11) 印刷页 355；PDF 页 374 | 笔误嫌疑 | Frobenius 平方误差 $\le 9(\mathrm{op}(\Theta^*)+1)^{-4}md\lambda_n^2$ | 原页；(11.12) 的 RSC 常数 $\kappa=(\mathrm{op}(\Theta^*)+1)^{-2}$，标准推论给出误差 $\asymp\lambda_n\sqrt{md}/\kappa$，故四次幂应在分子 | 保留原文；Notes 按原式抄录并标明与 RSC 标度不一致；勘误待批 | 作者 | 未批 |
| §11.2.2 印刷页 361；PDF 页 380 | 记号嫌疑 | 称 $\ell_\infty$-matrix-operator norm 却把记号写成三竖线的下标 2 | 原页；该式是行和范数；后文 Theorem 11.12 用 $\infty$-算子范数 | 保留原文；Notes 按行和范数解读；勘误待批 | 作者 | 未批 |
| Example 11.14 / (11.35a) 印刷页 366；PDF 页 385 | 笔误嫌疑 | $\phi_j(x_j;\theta_j^*)=\theta_j^* x_j-\log(x!)$ | 原页；自变量是 $x_j$，阶乘应为 $x_j!$ | 保留原文；Notes 按 $\log(x_j!)$ 解读；勘误待批 | 作者 | 未批 |
| §11.4.2 印刷页 374；PDF 页 393 | 笔误嫌疑 | 正文写 soft-thresholded version，紧接着定义硬阈值 $T_{\nu_n}(v)=v\mathbb I[\lvert v\rvert>\nu_n]$ | 原页；(11.58) 与后文证明均用硬阈值 | 保留原文；Notes 按硬阈值使用；勘误待批 | 作者 | 未批 |

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
