---
chapter_id: "ch12"
chapter_title: "Reproducing kernel Hilbert spaces"
map_path: "docs/companion-notes/ch12-content-map.md"
notes_path: "notes/ch12-notes.qmd"
reviewed_at: "2026-08-31"
delivery_status: "Notes 质检通过"
ppt_status: "未请求"
solutions_status: "未请求"
---

# 第 12 章审核报告

> 内部工件。对照印刷页 PNG（`scratch/ch12/p-402.png`–`p-434.png`）独立核验。文本层 `ch12.txt` 仅作索引；公式以 PNG 为准。

## 范围与结论

- 审核范围：第 12 章内容清单、`notes/ch12-notes.qmd`
- 主教材版本与页码：Martin J. Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series in Statistical and Probabilistic Mathematics No. 48, 2019, ISBN 978-1-108-49802-9；印刷页 383–415，PDF 页 402–434（PDF = 印刷 + 19）
- 当前结论：三个检查面均通过。Notes 可交付。清单中的教材笔误嫌疑保持 `勘误待批`，Notes 未写成已批准勘误。
- 未关闭问题：见下方勘误表（极化恒等式符号、(12.28) 的 $1/(2n)$ 与证明 $1/n$、Example 12.24 的 $2\pi$/$\pi$ 等）。新增一条：Exercise 12.20 对偶线性项印刷 $1/n$ 与带 $n^{-1/2}$ 表示式的独立推导 $1/\sqrt n$ 不一致。
- 下一步允许动作：教师批准勘误表；Notes 通过后再把 Solutions 的 `solutions_status` 从 `未请求` 推进。

## 独立质检

| 检查面 | 审核者 | 结果 | 简短证据或问题定位 |
|---|---|---|---|
| 内容清单与来源原页 | 独立质检代理（对照印刷页 PNG） | 通过 | Definitions 12.1–12.12、Theorems 12.5/12.11/12.13/12.20、Corollary 12.26、Propositions 12.27/12.31–12.33、(12.1)–(12.33)、Figures 12.1–12.2 均已入清单。Notes 按节序转写；§12.7 指回教材；§12.8 不进 Notes。 |
| 数学、假设与维度 | 独立质检代理（对照印刷页 PNG） | 通过 | 再生性 (12.3)、默塞尔椭球 (12.17)–(12.18)、KRR 驻点与 (12.30) 用 $1/n$ 匹配、KMD (12.32) 由再生性还原。未发现 Notes 虚构定理。线性核例 $\beta\in\mathbb R^d$ 已按定义域改正并保留原文。 |
| 结构、可访问性、链接与渲染 | 独立质检代理（对照印刷页 PNG） | 通过 | 七个读者栏目齐全；标题无跳级；Notes 汉语 / 英文术语首次给出；来源定位链到 `../solutions/ch12-solutions.qmd`。自测 `<details>` 含「参考答案」。 |

## 派生产物

| 产物 | 请求范围 | 状态 | 自身检查证据或受阻原因 |
|---|---|---|---|
| PPT | 未请求 | 未请求 | 用户未请求 PPT。 |
| Solutions | 未请求 | 未请求 | 合同规定 Notes 质检通过前不把 Solutions 标为完成；习题 12.1–12.20 已锁定，解答文件另写，待 Notes 通过后再审。 |

## 核对摘记

### 内容清单与来源原页

对照 `p-402.png`–`p-434.png` 核对编号公式与正式对象（OCR 不可信）：

- (12.1a)–(12.1c) 印刷页 383：内积对称、正定、线性。Notes 一致。
- Definition 12.2 印刷页 384：完备内积空间。Examples 12.3–12.4 的 $\ell^2(\mathbb N)$、$L^2[0,1]$、帕塞瓦尔同构已转写。
- Theorem 12.5 印刷页 385：里斯表示。Notes 给证明梗概，零空间闭与直和指向 Exercises 12.1、12.3。
- Definition 12.6 印刷页 386：有限 Gram 正半定。Example 12.7 原页 $\alpha_i$/$a_i$ 混用，Notes 按 $\alpha_i$。Example 12.8 的 $\Phi$ 与 (12.2) 一致；高斯核指向 Exercise 12.19。
- (12.3)–(12.4) 印刷页 388：再生性与预希尔伯特内积。Theorem 12.11 印刷页 389。
- Definition 12.12 / Theorem 12.13 / (12.5) 印刷页 390–391。Example 12.14 原页 $\beta\in\mathbb R^m$，Notes 写 $\mathbb R^d$。(12.6) 逐点收敛；Example 12.15 的 $x^n$ 与 $1/(2n+1)$ 与原页一致。
- (12.7)–(12.10) 印刷页 392–394：一阶 / 高阶索伯列夫，核 $\min\{x,z\}$ 与 $(t)_+$ 公式。
- (12.11a)–(12.14)、Theorem 12.20、Corollary 12.26 / (12.17)–(12.18) 印刷页 394–400。Example 12.22 的 $3\times 3$ 矩阵与四位小数特征对与原页一致。Example 12.23：$\mu_j=(2/((2j-1)\pi))^2$。Example 12.24 换元处 $2\pi$/$\pi$ 已标。Example 12.25：$\mu_j\asymp e^{-c j\log j}$。
- Proposition 12.27 / (12.19)–(12.22)、Proposition 12.31 / (12.23)–(12.24)。
- (12.25)–(12.30)、Figures 12.1–12.2。KRR 证明展开用 $1/n$，与 (12.28) 印刷 $1/(2n)$ 不一致，Notes 保留印刷式并按证明写驻点。
- (12.31)–(12.33)、KMD (12.32)。§12.7 指回教材。§12.8 Exercises 12.1–12.20 不进 Notes。

### 数学、假设与维度

**再生与求值有界。** (12.3) 与 Definition 12.12 通过里斯表示互推；Notes 未把完备化细节写成已证的新定理，极化式用正确减号并标明原页加号。

**默塞尔椭球。** (12.17a) 要求 $\sum\beta_j^2/\mu_j<\infty$；$\mu_j$ 衰减越快空间越小。Example 12.23 的 $\mu_j\asymp j^{-2}$ 与 Example 12.25 的指数衰减对比正确。Example 12.23 给出的 $\sin$ 特征函数满足 $L^2$ 范数平方 $1/2$，原页称为特征对而非 Theorem 12.20 的已归一正交基；Notes 按原页抄对，不挡。

**KRR 刻度。** $\mathbf K_{ij}=\mathcal K(x_i,x_j)/n$、$f=n^{-1/2}\sum\alpha_i\mathcal K(\cdot,x_i)$ 时，$\|f\|^2=\alpha^T\mathbf K\alpha$、$f(x)=\sqrt n\,\mathbf K\alpha$。目标若用 $1/n\|y-\sqrt n\mathbf K\alpha\|^2+\lambda\alpha^T\mathbf K\alpha$，驻点正是 (12.30)。印刷 (12.28) 的 $1/(2n)$ 会把 $\lambda$ 换成 $2\lambda$。Notes 处理符合勘误流程。

**KMD。** 单位球上 $\sup|\mathbb E_{\mathbb P}f-\mathbb E_{\mathbb Q}f|=\|\mu_{\mathbb P}-\mu_{\mathbb Q}\|_{\mathbb H}$，展开即 (12.32)。线性核退回 $\|\mu_p-\mu_q\|_2$，自测第 5 题正确。

**未发明定理。** 表示定理指向 Kimeldorf–Wahba；高斯特征值指向 Widom；博赫纳、IPM 文献节压缩为指回。

### 结构、可访问性、链接与渲染

读者栏目：本章导览、学习目标（5 个可观察动词）、必要先修（完备性 / $L^2$ 点值 / 核矩阵 $1/n$）、常见错误、轻量自测（5 题，`<details>` 含「参考答案」）、本章小结、术语对照、来源定位。标题 `#` → `##` → 例与 callout，无跳级。Notes 汉语；英文术语首次给出；「再生核希尔伯特空间」与第 1 章、glossary 一致。来源定位给出印刷/PDF 页码及 Solutions 相对链接。习题完整解答未写入 Notes。
