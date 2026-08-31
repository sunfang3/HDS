---
chapter_id: "ch01"
chapter_title: "Introduction"
source_title: "High-Dimensional Statistics: A Non-Asymptotic Viewpoint"
source_version: "Cambridge Series in Statistical and Probabilistic Mathematics, No. 48; first published 2019; ISBN 978-1-108-49802-9"
main_source_path: "High-Dimensional Statistics A Non-Asymptotic Viewpoint (Martin J. Wainwright) (z-library.sk, 1lib.sk, z-lib.sk).pdf"
printed_pages: "1–20"
pdf_pages: "20–39"
target_notes: "notes/ch01-notes.qmd"
language: "zh-CN"
learner_profile: "学过陈希孺《概率论与数理统计》本科教材；熟悉大数定律、中心极限定理、多元正态与协方差、假设检验的奈曼–皮尔逊思想；首次需要把固定维数的渐近换成 (n,d) 同时变大时的非渐近尾界，并理解稀疏、低秩、可加等低维结构如何缓解维数灾难。"
map_status: "清单完成"
---

# 第 1 章内容清单

> 内部质量工件。正式内容逐项登记；三个 vignette 按小节拆开；正文留给读者的 (1.14) 作为习题登记但不进入 Notes。

## 来源边界

- 教材权威来源：Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series No. 48
- 版本识别依据：封面 Cambridge Series；版权页 © Martin J. Wainwright 2019，First published 2019，ISBN 978-1-108-49802-9 Hardback，DOI 10.1017/9781108627771
- 目标章节与页码：第 1 章，印刷页 1–20；PDF 页 20–39（**PDF = 印刷 + 19**）
- 补充来源及用途：无（(1.14) 独立求解）
- 已知来源限制：文本层可用但公式常错位；公式、图注须对照 `scratch/ch01/p-0XX.png`

## 内容清单

| 定位 | 类型 | 内容/范围 | 重要性 | Notes 处理 | 合并目标/排除理由 | 核验状态 |
|---|---|---|---|---|---|---|
| 章首 印刷页 1；PDF 页 20 | SECTION | Chapter 1 Introduction：高维非渐近理论的动机与全书目标 | 关键 | 完整讲解 |  | 原页已核 |
| §1.1 印刷页 1–2；PDF 页 20–21 | SECTION | Classical versus high-dimensional theory | 关键 | 完整讲解 |  | 原页已核 |
| §1.1 印刷页 1；PDF 页 20 | FORMULA | 大数定律：样本均值 $\hat\mu_n\to\mu$ 依概率；中心极限定理 $\sqrt n(\hat\mu_n-\mu)$ 依分布趋于 $N(0,\Sigma)$ | 关键 | 完整讲解 |  | 原页已核 |
| §1.1 印刷页 2；PDF 页 21 | PROSE_RANGE | 动机问题：n=1000、d=500 时，固定 d、$n\to\infty$ 的理论是否有用；三点事实 | 关键 | 完整讲解 |  | 原页已核 |
| §1.2 印刷页 2–9；PDF 页 21–28 | SECTION | What can go wrong in high dimensions? | 关键 | 完整讲解 |  | 原页已核 |
| §1.2.1 印刷页 2–5；PDF 页 21–24 | SECTION | Linear discriminant analysis | 关键 | 完整讲解 |  | 原页已核 |
| (1.1) 印刷页 2；PDF 页 21 | FORMULA | 已知两类正态 $N(\mu_j,\Sigma)$ 的对数似然比化为 $\Psi(x)=\langle\mu_1-\mu_2,\Sigma^{-1}(x-(\mu_1+\mu_2)/2)\rangle$ | 关键 | 完整讲解 |  | 原页已核 |
| (1.2) 印刷页 3；PDF 页 22 | FORMULA | 等先验下 $\mathrm{Err}(\Psi)=\Phi(-\gamma/2)$，$\gamma=\sqrt{(\mu_1-\mu_2)^T\Sigma^{-1}(\mu_1-\mu_2)}$ | 关键 | 完整讲解 |  | 原页已核 |
| (1.3a)–(1.3b) 印刷页 3；PDF 页 22 | FORMULA | 样本均值与合并样本协方差 | 关键 | 完整讲解 |  | 原页已核 |
| (1.4) 印刷页 3；PDF 页 22 | FORMULA | 费希尔线性判别（插入估计；需 $n_i>d$） | 关键 | 完整讲解 |  | 原页已核 |
| (1.5) 印刷页 3；PDF 页 22 | FORMULA | $\Sigma=I_d$ 已知时的 $\widehat\Psi_{\mathrm{id}}$ | 关键 | 完整讲解 |  | 原页已核 |
| (1.6) 印刷页 4；PDF 页 23 | FORMULA | Kolmogorov 高维极限：$\mathrm{Err}(\widehat\Psi_{\mathrm{id}})\to\Phi(-\gamma^2/(2\sqrt{\gamma^2+2\alpha}))$，$d/n_i\to\alpha$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 1.1 印刷页 4；PDF 页 23 | FIGURE_TABLE | d=400 时经验误差 vs 经典 (1.2) vs 高维 (1.6) | 辅助 | 简要说明 |  | 原页已核 |
| (1.7) 及随后未编号式 印刷页 5；PDF 页 24 | FORMULA | 一般阈值 t、不等比例 $\alpha_1,\alpha_2$ 的极限误差；最优阈值 $t=(\alpha_2-\alpha_1)/2$ | 关键 | 完整讲解 |  | 原页已核 |
| §1.2.2 印刷页 5–7；PDF 页 24–26 | SECTION | Covariance estimation | 关键 | 完整讲解 |  | 原页已核 |
| (1.8) 印刷页 5；PDF 页 24 | FORMULA | 零均值样本协方差 $\widehat\Sigma=n^{-1}\sum x_i x_i^T$，无偏 | 关键 | 完整讲解 |  | 原页已核 |
| (1.9) 印刷页 6；PDF 页 25 | DEFINITION | $\ell_2$-算子范数 $\Vert\Vert\vert\widehat\Sigma-\Sigma\Vert\Vert\vert_2=\sup_{u\neq0}\Vert(\widehat\Sigma-\Sigma)u\Vert_2/\Vert u\Vert_2$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 1.2 印刷页 6；PDF 页 25 | FIGURE_TABLE | 样本特征值直方图 vs 马尔琴科–帕斯图尔律，$\alpha=0.2,0.5$ | 辅助 | 简要说明 |  | 原页已核 |
| (1.10) 印刷页 7；PDF 页 26 | FORMULA | MP 支撑 $[t_{\min}(\alpha),t_{\max}(\alpha)]=[(1-\sqrt\alpha)^2,(1+\sqrt\alpha)^2]$ | 关键 | 完整讲解 |  | 原页已核 |
| (1.11) 印刷页 7；PDF 页 26 | FORMULA | 非渐近上尾 $\mathbb P[\gamma_{\max}(\widehat\Sigma)\ge(1+\sqrt{d/n}+\delta)^2]\le e^{-n\delta^2/2}$ | 关键 | 完整讲解 |  | 原页已核 |
| §1.2.3 印刷页 7–9；PDF 页 26–28 | SECTION | Nonparametric regression | 关键 | 完整讲解 |  | 原页已核 |
| (1.12) 印刷页 7；PDF 页 26 | FORMULA | 回归函数 $f(x)=\mathbb E[Y\mid x]$；MSE $\Vert\widehat f-f\Vert_{L^2}^2$ | 关键 | 完整讲解 |  | 原页已核 |
| (1.13) 印刷页 8；PDF 页 27 | FORMULA | $\rho_\infty(n,d)=\mathbb E\min_i\Vert X'-X_i\Vert_\infty$ | 关键 | 完整讲解 |  | 原页已核 |
| (1.14) 印刷页 8；PDF 页 27 | FORMULA | $\log\rho_\infty(n,d)\ge\log(d/(2(d+1)))-(\log n)/d$；正文留作习题 | 关键 | 完整讲解 | 不等式进入 Notes；证明进 Solutions | 原页已核 |
| Figure 1.3 印刷页 8；PDF 页 27 | FIGURE_TABLE | $\rho_\infty(2d,d)$ 与 $\rho_\infty(d^2,d)$ 随 d 增大仍高于 1/3 | 辅助 | 简要说明 |  | 原页已核 |
| (1.15) 印刷页 9；PDF 页 28 | FORMULA | 确定性 $\ell_\infty$ 覆盖：$\sup_{x'}\min_i\Vert x'-x_i\Vert_\infty\le\delta$ 需约 $(1/(2\delta))^d$ 个点 | 关键 | 完整讲解 |  | 原页已核 |
| §1.2.3 印刷页 9；PDF 页 28 | DEFINITION | $\delta$-覆盖与 $\delta$-填装；指数标度不可避免 | 关键 | 完整讲解 |  | 原页已核 |
| §1.3 印刷页 9–14；PDF 页 28–33 | SECTION | What can help us in high dimensions? 低维结构 | 关键 | 完整讲解 |  | 原页已核 |
| §1.3.1 印刷页 10–11；PDF 页 29–30 | SECTION | Sparsity in vectors | 关键 | 完整讲解 |  | 原页已核 |
| §1.3.1 印刷页 10；PDF 页 29 | FORMULA | $\Vert\hat\mu_j-\mu_j\Vert_2^2$ 集中在 $d/n_j=\alpha$（预告 Example 2.11） | 关键 | 完整讲解 |  | 原页已核 |
| (1.16) 印刷页 10；PDF 页 29 | DEFINITION | 硬阈值 $H_\lambda(x)=x\,\mathbb I[\lvert x\rvert>\lambda]$ | 关键 | 完整讲解 |  | 原页已核 |
| (1.17) 印刷页 10；PDF 页 29 | DEFINITION | 软阈值 $T_\lambda(x)=\mathbb I[\lvert x\rvert>\lambda](x-\lambda\mathrm{sign}(x))$ | 关键 | 完整讲解 |  | 原页已核 |
| (1.18)–(1.19) 印刷页 10；PDF 页 29 | FORMULA | $\lambda_n=\sqrt{2\log d/n}$ 的硬阈值均值与阈值线性判别 | 关键 | 完整讲解 |  | 原页已核 |
| Figure 1.4 印刷页 11；PDF 页 30 | FIGURE_TABLE | 硬/软阈值函数；s=5 稀疏时经典预测重新准确 | 辅助 | 简要说明 |  | 原页已核 |
| §1.3.2 印刷页 11–12；PDF 页 30–31 | SECTION | Structure in covariance matrices | 关键 | 完整讲解 |  | 原页已核 |
| Figure 1.5 印刷页 12；PDF 页 31 | FIGURE_TABLE | 硬阈值协方差的谱集中；有界迹时算子范数误差 $\asymp n^{-1/2}$ | 辅助 | 简要说明 |  | 原页已核 |
| §1.3.3 印刷页 12–14；PDF 页 31–33 | SECTION | Structured forms of regression | 关键 | 完整讲解 |  | 原页已核 |
| (1.20) 印刷页 13；PDF 页 32 | DEFINITION | 可加模型 $f(x)=\sum_{j=1}^d g_j(x_j)$ | 关键 | 完整讲解 |  | 原页已核 |
| (1.21) 印刷页 13；PDF 页 32 | DEFINITION | 稀疏可加模型（SPAM）$f=\sum_{j\in S}g_j$ | 关键 | 完整讲解 |  | 原页已核 |
| (1.22) 印刷页 13；PDF 页 32 | DEFINITION | 多指标模型 $f(x)=h(Ax)$；单指标 $s=1$ | 关键 | 完整讲解 |  | 原页已核 |
| (1.23) 印刷页 13；PDF 页 32 | DEFINITION | 投影寻踪回归 $f=\sum_{j=1}^M g_j(\langle a_j,x\rangle)$ | 关键 | 完整讲解 |  | 原页已核 |
| §1.4 印刷页 14–15；PDF 页 33–34 | SECTION | What is the non-asymptotic viewpoint? 三种分析模式 | 关键 | 完整讲解 |  | 原页已核 |
| §1.5 印刷页 15–19；PDF 页 34–38 | SECTION | Overview of the book | 辅助 | 简要说明 |  | 原页已核 |
| §1.5.1 印刷页 15–17；PDF 页 34–36 | PROSE_RANGE | TT/ME 分章与依赖：第 2、4 章必读；第 3 章可选加深 | 辅助 | 简要说明 |  | 原页已核 |
| §1.5.2 印刷页 17；PDF 页 36 | PROSE_RANGE | 推荐先修：线性代数、初等实分析、概率、经典数理统计 | 关键 | 简要说明 | 与必要先修合并讲解 | 原页已核 |
| §1.5.3 / Figure 1.6 印刷页 17–18；PDF 页 36–37 | FIGURE_TABLE | 教学路径与章依赖图 | 辅助 | 简要说明 |  | 原页已核 |
| §1.6 印刷页 19–20；PDF 页 38–39 | PROSE_RANGE | Bibliographic details：Rao、Kolmogorov、MP、Huber、阈值与 $\ell_1$、可加/SPAM/单指标/投影寻踪 | 辅助 | 指回教材 | 文献清单不抄入 Notes | 原页已核 |
| 正文习题 (1.14) 印刷页 8；PDF 页 27 | EXERCISE | 证明下界 (1.14) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |

## 来源异常与勘误

| 定位 | 问题类型 | 原式/原文 | 核验证据 | 处置 | 数学复核人 | 批准人 |
|---|---|---|---|---|---|---|
| §1.2.1 印刷页 5；PDF 页 24 | 笔误嫌疑 | 正文写 “classical prediction $\Phi(-\gamma)$ drastically underestimates” | 原页；(1.2) 与 Figure 1.1 用的是 $\Phi(-\gamma/2)$；$\alpha=0$ 时 (1.6) 也回到 $\Phi(-\gamma/2)$ | 保留原文；Notes 标明与 (1.2) 不一致；`勘误待批` | 作者 | 未批 |
| Figure 1.2 图注 印刷页 6；PDF 页 25 | 笔误嫌疑 | 图注写 $\gamma_{\max}(\Sigma)$ 接近 $(1+\sqrt\alpha)^2$ | 原页；总体 $\Sigma=I_d$ 时 $\gamma_{\max}(\Sigma)=1$；正文 (1.11) 讨论的是 $\gamma_{\max}(\widehat\Sigma)$ | 保留原文；Notes 按 $\widehat\Sigma$ 解读；`勘误待批` | 作者 | 未批 |
| Figure 1.5(a) 印刷页 12；PDF 页 31 | 笔误嫌疑 | 图题印 $\alpha=0.5$，正文写 $\alpha=0.2$、$(n,d)=(4000,800)$ | 独立审核对照原页；与 Figure 1.2(a) 设定相同 | 保留原文；Notes 跟正文 $\alpha=0.2$；`勘误待批` | 独立质检代理 | 未批 |

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
