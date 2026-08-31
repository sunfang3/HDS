---
chapter_id: "ch09"
chapter_title: "Decomposability and restricted strong convexity"
map_path: "docs/companion-notes/ch09-content-map.md"
notes_path: "notes/ch09-notes.qmd"
reviewed_at: "2026-08-31"
delivery_status: "Notes 质检通过"
ppt_status: "未请求"
solutions_status: "完成"
---

# 第 9 章审核报告

> 内部工件。对照印刷页 PNG（`scratch/ch09/p-278.png`–`p-330.png`）独立核验，不采用作者对勘误、覆盖或推导的结论。文本层 `ch09.txt` 仅作索引；公式以 PNG 为准。

## 范围与结论

- 审核范围：第 9 章内容清单、`notes/ch09-notes.qmd`、§9.11 Exercises 9.1–9.14 的独立解答（`solutions/ch09-solutions.qmd`）
- 主教材版本与页码：Martin J. Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series in Statistical and Probabilistic Mathematics No. 48, 2019, ISBN 978-1-108-49802-9；印刷页 259–311，PDF 页 278–330（PDF = 印刷 + 19）
- 当前结论：三个检查面均通过。Notes 按节序转写可分解正则、RSC、组套索与重叠组；六处教材笔误嫌疑保持 `勘误待批`。
- 未关闭问题：清单中已登记的六处原文问题（Figure 9.3 指向、$\Psi$ 锥不等式左右对调、Corollary 9.20 的 9 与 9.26 的 9/4、$\mathbb B_2(R)$ 的 dummy、Exercise 9.14 的 $L=B^2/2$ 与 $\mathbb T(R;\rho)$ 半径符号）均未获教师批准。
- 下一步允许动作：勘误待教师批准；新词由父代理合并进 `glossary.qmd`。

## 独立质检

| 检查面 | 审核者 | 结果 | 简短证据或问题定位 |
|---|---|---|---|
| 内容清单与来源原页 | 独立质检代理（对照印刷页 PNG） | 通过 | (9.1)–(9.101)、Definition 9.9–9.22、Proposition 9.13、Lemma 9.14/9.21/9.25、Theorem 9.19/9.24/9.34/9.36、Corollary 9.20/9.26–9.31、Table 9.1、Figure 9.1–9.10 均已入清单；Notes 按节序转写，习题不进 Notes。 |
| 数学、假设与维度 | 独立质检代理（对照印刷页 PNG） | 通过 | 好事件 $\lambda_n\ge 2\Phi^*(\nabla\mathcal L_n(\theta^*))$ 推出锥 (9.29)；RSC 容差与 $\Psi(\overline{\mathbb M})$ 的乘积条件与原页 $\kappa/64$、$\kappa/32$ 一致；组套索 $\Psi=\sqrt{\lvert S_{\mathcal G}\rvert}$。未发现 Notes 虚构定理。常数 9 与 9/4 按原框抄入并标明不衔接。 |
| 结构、可访问性、链接与渲染 | 独立质检代理（对照印刷页 PNG） | 通过 | 七个读者栏目齐全；标题无跳级；Notes 汉语 / Solutions 英语；来源定位链到 `../solutions/ch09-solutions.qmd`；表格语法已核验。 |

## 派生产物

| 产物 | 请求范围 | 状态 | 自身检查证据或受阻原因 |
|---|---|---|---|
| PPT | 未请求 | 未请求 | 用户未请求 PPT。 |
| Solutions | 全部习题（§9.11 Exercises 9.1–9.14） | 完成 | 题号由印刷页 307–311 锁定；独立求解。9.1 变分范数；9.4–9.5 对偶；9.9–9.10 强凸等价与球外线性曲率；9.12 软阈值唯一并给出基本不等式常数 3（印刷为 $3/2$）；9.14(a) 链规则得 $L=B^2$（印刷为 $B^2/2$）。 |

## 核对摘记

### 内容清单与来源原页

对照 `p-278.png`–`p-330.png` 抽核编号公式（OCR 不可信）：

- (9.1)–(9.3) 印刷页 259–260：总体代价、$\theta^*$、正则化 $M$ 估计。Notes 一致。
- (9.4) 印刷页 261：$n^{-1}$ 下有 $1/2$ 的平方损失。Notes 一致。
- (9.5)–(9.8) 印刷页 261–262：GLM 指数族、对数优势、负对数似然、GLM 套索。Notes 一致。
- (9.9)–(9.10) 印刷页 262–264：普通组范数与重叠变分。Notes 一致。
- (9.11)–(9.16) 印刷页 265–267：图形套索、多元回归、分解形式。Notes 简要说明 9.5/9.8、完整讲解 9.6/9.7，符合清单。
- (9.17)–(9.19) 印刷页 268：SVD 与核范数。Notes 完整讲解。
- Definition 9.9 / (9.22) 印刷页 269：$\Phi(\alpha+\beta)=\Phi(\alpha)+\Phi(\beta)$，$\alpha\in\mathbb M$，$\beta\in\overline{\mathbb M}^\perp$。Notes 一致。
- (9.25)–(9.26) 印刷页 271：重叠反例 $4>2+\sqrt{2}$；放大组集。Notes 一致。
- Table 9.1 / (9.27)–(9.28) 印刷页 272–273：对偶对与好事件。Notes 表已去掉未转义竖线。
- Proposition 9.13 / (9.29)–(9.30) 印刷页 273–274：锥系数 3 与 4。Notes 一致。
- Lemma 9.14 / (9.32)–(9.34) 印刷页 275。Notes 完整讲解策略。
- Definition 9.15 / (9.38) 印刷页 277：RSC。Notes 一致。
- (9.39)–(9.45) 印刷页 278–279：RE、$\mu_n$、$\Psi$。Notes 标明 (9.45) 后一句左右对调。
- Theorem 9.19 / (9.47)–(9.48) 印刷页 280：$\tau_n^2\Psi^2\le\kappa/64$。Notes 一致。
- Corollary 9.20 / (9.49) 印刷页 281：$\Phi$ 界 $6(\lambda_n/\kappa)\Psi^2$，$\|\cdot\|^2$ 界 $9(\lambda_n^2/\kappa^2)\Psi^2$。
- Theorem 9.24 / Lemma 9.25 印刷页 285–286：$3\lambda_n/\kappa$ 与 $16\Psi^2\Phi^*$。Notes 一致。
- Corollary 9.26 / (9.63) 印刷页 287：$\ell_2^2$ 为 $(9/4)s\lambda_n^2/\kappa^2$。Notes 标明与 9.20 不衔接。
- Corollary 9.27 印刷页 289：$\lambda_n=2BC\{\cdots\}$（9.26 为 $4BC$）。Notes 按各框原文抄入。
- Corollary 9.28 / (9.68)–(9.69) 印刷页 290–291：组界与多元回归比较。Notes 一致。
- Corollary 9.31 / (9.77) 印刷页 295：自适应 $36\lambda_n^2/\kappa^2$。Notes 一致。
- Theorem 9.34 / 9.36 印刷页 300、303。Notes 完整讲解陈述、证明指回教材，符合清单。
- §9.11 印刷页 307–311：Exercises 9.1–9.14 不进 Notes，全部进 Solutions。处理正确。

六处笔误嫌疑（保留原文，Notes 未写成已批准勘误），与清单一致：

1. Example 9.3 印刷页 262：正文指向 Figure 9.3(a) 为 overlapping groups；图注 (a) 为不重叠，(b) 为重叠。
2. Definition 9.18 讨论 印刷页 279：先写 $\|\Delta\|_1\le 4\sqrt s\|\Delta\|_2$，随即称 familiar inequality $\|\Delta\|_2\le 4\sqrt s\|\Delta\|_1$。
3. Corollary 9.20 vs 9.26：$(9.49\mathrm b)$ 为 $9$；$(9.63)$ 为 $9/4$。9.26 证明写应用 9.20，却用 $9\Psi^2\lambda_n^2/(4\kappa^2)<1$。
4. (9.82) 印刷页 298：$\mathbb B_2(R):=\{\Delta:\|\theta\|_2\le R\}$，dummy 应为 $\Delta$。
5. Exercise 9.14(a) 印刷页 310：称 (9.101) 以 $L=B^2/2$ 成立；链规则给出 $L=B^2$。
6. Exercise 9.14(b) 印刷页 310：集合名 $\mathbb T(R;\rho)$，定义半径为 $r$。

### 数学、假设与维度

**可分解与锥。** $\ell_1$ 与不重叠组对 $(\mathbb M,\mathbb M^\perp)$ 可分解；重叠普通组范数被 (9.25) 否定，放大 $\widetilde S_{\mathcal G}$ 后对 $(\mathbb M(S_{\mathcal G}),\mathbb M^\perp(\widetilde S_{\mathcal G}))$ 恢复可分解。Lemma 9.14 两式相加得到 (9.29) 的系数 3 与 4，与原页代数一致。$\theta^*\in\mathbb M$ 时 (9.30) 的 4 来自 $1+3$。

**RSC 与神谕。** Definition 9.15 的容差是 $\tau_n^2\Phi^2(\Delta)$。Theorem 9.19(b) 要求 $\tau_n^2\Psi^2(\overline{\mathbb M})\le\kappa/64$ 才能把二次型系数收到 $\kappa/4$。Corollary 9.20 的 $\ell_2$ 前置 9 来自 $(\kappa/2)r=(3\lambda_n/2)\Psi$ 配平方；$\Phi$ 前置 6 若配合 $\|\Delta\|\le 3(\lambda_n/\kappa)\Psi$ 会得到 12，与 9/4 路线的 $4\times 3/2=6$ 一致——这正是 9 与 9/4 冲突在 (9.49a) 上的投影。Notes 不擅自改常数。

**GLM 与组。** (G2) 为 $\|\psi''\|_\infty\le B^2$，排除 Poisson。得分次高斯参数 $BC/\sqrt n$ 由矩母函数 Taylor 得到。组套索 $\Psi=\sqrt{\lvert S_{\mathcal G}\rvert}$，覆盖基数 $5^{|g|}$ 给出 $m\log 5+\log\lvert\mathcal G\rvert$。多元回归 (9.69b) 两项分别对应已知组的参数个数与行搜索。重叠分解对偶 $\max(\|v\|_\infty,\omega^{-1}\max\|v_g\|_2)$，权重 (9.74) 对齐两条噪声。

**RSC 证明。** Theorem 9.34 把利普希茨代价的 RSC 收到 $\Phi^*(\bar x_n)$；Theorem 9.36 用截断使 $\psi''$ 只需紧集正下界。Notes 只留策略，符合清单对长证明的 `指回教材`。

**Solutions。** 14 题均独立求解。9.12(b) 基本不等式给出 $\|\Delta\|_2\le 3\sqrt s\lambda_n$，印刷为 $3/2$；9.14(a) 给出 $L=B^2$。两处均保留印刷常数并标明差异，不写成已批准勘误。

### 结构、可访问性、链接与渲染

读者栏目：本章导览、学习目标（5 个可观察动词）、必要先修（对偶范数 / 次梯度 / 强凸两种写法）、常见错误、轻量自测（5 题，`<details>` 含「参考答案」）、本章小结、术语对照、来源定位。标题由 `#` 到 `##`，无跳级。Notes 汉语、英文术语首次给出；Solutions 英语，题号 `### Exercise 9.1`–`9.14`。来源定位给出印刷/PDF 页码及 Solutions 相对链接。习题完整解答不在 Notes。
