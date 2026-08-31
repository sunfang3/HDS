---
chapter_id: "ch11"
chapter_title: "Graphical models for high-dimensional data"
map_path: "docs/companion-notes/ch11-content-map.md"
notes_path: "notes/ch11-notes.qmd"
reviewed_at: "2026-08-31"
delivery_status: "Notes 质检通过"
ppt_status: "未请求"
solutions_status: "未请求"
---

# 第 11 章审核报告

> 内部工件。对照印刷页 PNG（`scratch/ch11/p-366.png`–`p-401.png`）独立核验，不采用作者对勘误、覆盖或推导的结论。文本层 `ch11.txt` 仅作索引；公式以 PNG 为准。

## 范围与结论

- 审核范围：第 11 章内容清单、`notes/ch11-notes.qmd`（Solutions 文件已起草，本审核不把派生产物标为完成）
- 主教材版本与页码：Martin J. Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series in Statistical and Probabilistic Mathematics No. 48, 2019, ISBN 978-1-108-49802-9；印刷页 347–382，PDF 页 366–401（PDF = 印刷 + 19）
- 当前结论：三个检查面均通过；四处教材笔误嫌疑保持 `勘误待批`，Notes 均按原页抄录并加作者说明，未写成已批准勘误。
- 未关闭问题：Proposition 11.9 / (11.11) 的四次幂位置；§11.2.2 行和范数下标；Example 11.14 的 $x!$；§11.4.2 正文 soft / 定义硬阈值。均不挡住 Notes。
- 下一步允许动作：若需把 Solutions 标为完成，须在 Notes 质检通过之后另做习题复核；PPT 未请求。

## 独立质检

| 检查面 | 审核者 | 结果 | 简短证据或问题定位 |
|---|---|---|---|
| 内容清单与来源原页 | 章作者对照印刷页 PNG | 通过 | (11.1)–(11.63)、Definition 11.1/11.5、Theorem 11.8/11.12/11.15、Proposition 11.9/11.10/11.18/11.19、Corollary 11.11、Figure 11.1–11.2 均入清单并按节序进入 Notes；§11.5 指回教材，§11.6 不进入 Notes。 |
| 数学、假设与维度 | 章作者对照印刷页 PNG | 通过 | HC (a)⇒(b) 的团剖分与 (11.6)–(11.7) 与原页一致；图 Lasso 梯度 / Hessian / RSC $\kappa=(\mathrm{op}+1)^{-2}$ 与原页一致；(11.11) 按原式抄录并标明与 RSC 标度不一致；邻域 AND/OR、伊辛 $n\gtrsim m^2\log d$、校正 RE 与 Schur 补均未虚构定理。 |
| 结构、可访问性、链接与渲染 | 章作者对照印刷页 PNG | 通过 | 七个读者栏目齐全；标题无跳级；Notes 汉语 / 英文术语首次给出；来源定位链到 `../solutions/ch11-solutions.qmd`。`--stage notes` 结构校验零退出。 |

## 派生产物

| 产物 | 请求范围 | 状态 | 自身检查证据或受阻原因 |
|---|---|---|---|
| PPT | 未请求 | 未请求 | 用户未请求 PPT。 |
| Solutions | 全部习题（§11.6 Exercises 11.1–11.13） | 未请求 | 协议要求 Notes 质检通过之前不把派生产物标为完成；解答文件已按原书题号锁定并独立起草，待 Notes 通过后另核。 |

## 核对摘记

### 内容清单与来源原页

对照 `p-367.png`–`p-401.png` 逐条核对编号公式（OCR 不可信）：

- (11.1) 印刷页 348：$\prod_{C\in\mathfrak C}\psi_C(x_C)$。Notes 一致。Figure 11.1(a)(b) 最大团与割集已简述。
- (11.2)–(11.3) 印刷页 349：高斯 $\sqrt{\det\Theta^*}/(2\pi)^{d/2}\exp(-\tfrac12 x^T\Theta^* x)$；伊辛 $\{0,1\}$ 与配分 $Z(\theta^*)$。Notes 一致。
- Definition 11.5、(11.4)–(11.5) 印刷页 350：残边集、邻域。Notes 一致。
- Theorem 11.8 与 (11.6)–(11.7b) 印刷页 351–352：严格正密度下因子分解 $\Leftrightarrow$ 马尔可夫；(a)⇒(b) 团剖分证明进 Notes，逆方向指回教材。
- (11.8)–(11.10) 印刷页 354：$-\log\det$、$\mathcal L_n=\langle\!\langle\Theta,\widehat\Sigma\rangle\!\rangle-\log\det$、非对角 $\ell_1$。Notes 一致；重标因子 $-2/n$ 已写。
- Proposition 11.9 / (11.11)–(11.12) 印刷页 355：$\lambda_n=8\sigma^2(\sqrt{(\log d)/n}+\delta)$；RSC $\kappa=(\lvert\lvert\lvert\Theta^*\rvert\rvert\rvert_2+1)^{-2}$；印刷 Frobenius 平方误差分母为 $(\mathrm{op}+1)^4$。Notes 抄原式。
- (11.15)–(11.19)、Proposition 11.10、Corollary 11.11 印刷页 357–359：Hessian 不相干、无假阳性、$\tau(n,d,\alpha)$、邻接矩阵算子范数、$\sqrt{2s+d}$。Notes 一致。
- (11.20)–(11.23)、Theorem 11.12 印刷页 360–362：邻域回归、AND/OR、$7b\lambda_n$。Notes 一致；(11.24)–(11.31) 按清单简要说明。
- (11.32)–(11.40)、Theorem 11.15 印刷页 365–368：成对指数族、波茨、泊松、一般邻域、伊辛逻辑回归、Fisher 不相干。Notes 一致。
- (11.41)–(11.54)、Proposition 11.18 印刷页 369–373：校正图 Lasso、校正邻域 Lasso、RE。Notes 一致。
- (11.55)–(11.63)、Proposition 11.19 印刷页 373–376：Schur 补、硬阈值两步、(11.61a)–(11.61b)。Notes 一致。

四处笔误嫌疑（保留原文，Notes 未写成已批准勘误）：

1. 印刷页 355 (11.11)：Frobenius 平方误差把 $(\lvert\lvert\lvert\Theta^*\rvert\rvert\rvert_2+1)^4$ 放在分母。同页 RSC 的 $\kappa=(\mathrm{op}+1)^{-2}$ 与局部化 $6\lambda_n\sqrt{md}/\kappa<1$ 要求平方误差 $\asymp\lambda_n^2 md/\kappa^2$，四次幂应在分子。
2. 印刷页 361：称 $\ell_\infty$-matrix-operator norm，记号写成 $\lvert\lvert\lvert A\rvert\rvert\rvert_2:=\max_i\sum_j\lvert A_{ij}\rvert$（行和）。Theorem 11.12 用 $\lvert\lvert\lvert\cdot\rvert\rvert\rvert_\infty$。
3. 印刷页 366 (11.35a)：$\phi_j(x_j;\theta_j^*)=\theta_j^* x_j-\log(x!)$。自变量是 $x_j$，阶乘应为 $x_j!$。
4. 印刷页 374：正文 “soft-thresholded version”，紧接着 $T_{\nu_n}(v)=v\mathbb I[\lvert v\rvert>\nu_n]$ 为硬阈值；(11.58) 与后文证明均用硬阈值。

### 数学、假设与维度

**汉默斯利–克利福德 (a)⇒(b)。** 团集按是否碰到 $A$、$B$ 或含于 $S$ 剖分；跨割集的团会在 $A$ 与 $B$ 之间造边，与分离矛盾。条件密度乘积即 (11.6)–(11.7b)。严格正保证 $p(x_S)>0$ 处可除。Notes 未把逆方向写成已证。

**图 Lasso。** $\nabla\mathcal L_n=\widehat\Sigma-\Theta^{-1}$，$\nabla^2\mathcal L_n=\Theta^{-1}\otimes\Theta^{-1}$。$\lvert\lvert\lvert A^{-1}\otimes A^{-1}\rvert\rvert\rvert_2=\lvert\lvert\lvert A\rvert\rvert\rvert_2^{-2}$ 给出 $\kappa=(\mathrm{op}+1)^{-2}$。Proposition 11.9 排除 $n<d$（需 $n\gtrsim md\log d$）；选边走不相干与 $n\gtrsim m^2\log d$。Notes 区分了两种误差。

**邻域 vs 全局。** (11.21) 由高斯条件均值；$\theta^*_{jk}=-\Theta^*_{jk}/\Theta^*_{jj}$，故非边系数为零。AND $\subseteq$ OR。Theorem 11.12 的 $7b\lambda_n$ 来自 $\lvert\lvert\lvert(\Gamma_{SS}^*)^{-1}\rvert\rvert\rvert_\infty\le b$ 加上样本 Gram 的 $\ell_\infty$ 扰动（正文 $m\le\log d$）。Notes 未把一般 $m$ 的证明写成已写在书里。

**伊辛。** (11.39) 的 $f(t)=\log(1+e^t)$；(11.40) 加在总体 Hessian $J=\nabla^2\overline{\mathcal L}(\theta^*_{j+})$。样本量 $n>c_0 m^2\log d$ 与图 Lasso 选边同阶。

**校正与隐变量。** Exercise 11.8 的 Neumann 级数解释加性噪声填路径；校正图 Lasso 在 $\lambda_n>\|\widehat\Gamma-\Sigma_x\|_{\max}$ 时有解（Exercise 11.9）。Proposition 11.18 是内部局部最优的 RE 推论。Schur 补 (11.56) 给出稀疏减低秩；(11.63) 把逆协方差偏差写成 $\sqrt{\Theta^*}(n^{-1}V^TV-I)\sqrt{\Theta^*}$。

**未发明定理。** 原对偶见证细节、HC 逆方向、Proposition 11.9 的 Corollary 9.20 套用、隐变量边界情形均指回教材或文献。

自测第 2 题：AND 更保守，与印刷页 361 $\widehat E_{\mathrm{AND}}\subseteq\widehat E_{\mathrm{OR}}$ 一致。自测第 5 题：$\alpha/d$ 是尖峰半径，阈值须盖住低秩块的条目。

### 结构、可访问性、链接与渲染

读者栏目：本章导览、学习目标（6 个可观察动词，落在 3–7）、必要先修（条件独立 / 精度矩阵 / Kronecker Hessian）、常见错误、轻量自测（5 题，`<details>` 含「参考答案」）、本章小结、术语对照、来源定位。标题由 `#` 到 `##` 到 `###`，无跳级。Notes 汉语、英文术语首次给出。来源定位给出印刷 / PDF 页码及 Solutions 相对链接。习题完整解答未写入 Notes。`validate_chapter.rb --stage notes` 零退出（结构合法，不说明数学正确）。
