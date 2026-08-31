---
chapter_id: "ch07"
chapter_title: "Sparse linear models in high dimensions"
map_path: "docs/companion-notes/ch07-content-map.md"
notes_path: "notes/ch07-notes.qmd"
reviewed_at: "2026-08-31"
delivery_status: "Notes 质检通过"
ppt_status: "未请求"
solutions_status: "完成"
---

# 第 7 章审核报告

> 内部工件。对照印刷页 PNG（`scratch/ch07/p-213.png`–`p-254.png`）独立核验。文本层 `ch07.txt` 仅作索引；公式、图注以 PNG 为准。

## 范围与结论

- 审核范围：第 7 章内容清单、`notes/ch07-notes.qmd`、§7.8 Exercises 7.1–7.20 的独立解答（`solutions/ch07-solutions.qmd`）
- 主教材版本与页码：Martin J. Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series in Statistical and Probabilistic Mathematics No. 48, 2019, ISBN 978-1-108-49802-9；印刷页 194–235，PDF 页 213–254（PDF = 印刷 + 19）
- 当前结论：三个检查面均通过。Notes 按节序转写主线；§7.6 附录只留 Gordon / 剥壳骨架，§7.7 文献与 §7.8 习题不进 Notes。四处教材笔误嫌疑保持 `勘误待批`。
- 未关闭问题：Example 7.15 交叉引用 (7.19)/(7.20)；Theorem 7.13(c) 陈述 $4/\kappa$ 与证明末行 $8/\kappa$；预言不等式 (7.33) 花括号内 $+2$ 对 $+4$；Proposition 7.11 的 $S$/$S_0$ 记号。另：Exercise 7.7(b) 若某印次写作 $\log(es/d)$，与正文 $s\log(ed/s)$ 冲突，建议一并列入勘误表。
- 下一步允许动作：四处（可加第五处）勘误待教师批准。

## 独立质检

| 检查面 | 审核者 | 结果 | 简短证据或问题定位 |
|---|---|---|---|
| 内容清单与来源原页 | 独立质检（对照印刷页 PNG） | 通过 | (7.1)–(7.59) 及 Definition/Theorem 7.7–7.23、Figure 7.1–7.7、Exercises 7.1–7.20 均已入清单。Notes 按节序转写；关键式与原页一致，见下。 |
| 数学、假设与维度 | 独立质检（对照印刷页 PNG） | 通过 | Theorem 7.8 切锥 $\Leftrightarrow$ $\mathbb C(S)$；RE 锥 $\mathbb C_3(S)$ 推出 (7.25a–c) 与 (7.38)–(7.39)；PDW 严格对偶可行推出唯一性。未发现 Notes 虚构定理。 |
| 结构、可访问性、链接与渲染 | 独立质检 | 通过 | 七个读者栏目齐全；标题无跳级；Notes 汉语 / Solutions 英语；来源定位链到 `../solutions/ch07-solutions.qmd`。 |

## 派生产物

| 产物 | 请求范围 | 状态 | 自身检查证据或受阻原因 |
|---|---|---|---|
| PPT | 未请求 | 未请求 | 用户未请求 PPT。 |
| Solutions | 全部习题（§7.8 Exercises 7.1–7.20） | 完成 | 题号已从印刷页 229–235 锁定。20 题均独立求解；书中给出的常数（$1/(3s)$、$c_1=1/8$、$c_2=50$、慢/快速率预因子）已对照原页。 |

## 核对摘记

### 内容清单与来源原页

对照 `p-213.png`–`p-254.png` 抽核编号公式（OCR 不可信）：

- (7.1)–(7.4) 印刷页 194–195：线性模型、支撑、$q$-球、有序坐标。Notes 一致。Figure 7.1 图注 $q=1,0.75,0.5$，Notes 简要说明。
- (7.6a)–(7.6b) 印刷页 197：硬阈值保留/清零；软阈值 $\mathrm{sign}(y_i)(\lvert y_i\rvert-\lambda)$。与第 1 章 (1.16)–(1.17) 同对象。
- (7.8)–(7.9) 印刷页 200：$\ell_0$ 规划与基追踪 LP。
- Definition 7.7 / Theorem 7.8 印刷页 202：限制零空间 $\mathbb C(S)\cap\mathrm{null}(X)=\{0\}$ 与基追踪唯一恢复等价。
- (7.12)–(7.15) 印刷页 203–204：成对不相干、RIP、夹心 $\delta_{\mathrm{PW}}\le\delta_s\le s\delta_{\mathrm{PW}}$。
- Proposition 7.11 印刷页 204：$\delta_{2s}<1/3$。证明中 $S$ 与 $\widetilde\theta_{S_0}$ 对调，Notes 显式令 $S_0=S$。
- (7.17) 印刷页 205：尖峰单位 $\Sigma=(1-\mu)I+\mu\mathbf 1\mathbf 1^T$。
- (7.18)–(7.20) 印刷页 206：拉格朗日套索、约束套索、松弛基追踪。Figure 7.3 图注稀疏度 $s=\lceil 0.1d\rceil$（ceiling）；Notes 已按 PNG 更正。
- Definition 7.12 / (7.22) 印刷页 208：RE。
- Theorem 7.13 / (7.25a–c) 印刷页 210：$\frac3\kappa\sqrt s\lambda_n$、$\frac4\kappa\sqrt s\lVert X^T w/n\rVert_\infty$、陈述用 $\frac4\kappa$ 加第二项 $\frac2{\sqrt\kappa}$。附加 $\ell_1$ 界 $4\sqrt s$。
- (7.26)–(7.27) 印刷页 211：$6C\sigma/\kappa$ 与 $4C\sigma/\kappa$。
- Theorem 7.16 / (7.31) 印刷页 214：$c_1=1/8$、$c_2=50$，概率 $1-e^{-n/32}/(1-e^{-n/32})$。
- Theorem 7.19 / (7.32) 印刷页 215：预言不等式三项，基数上界 $c_1\bar\kappa n/(64 c_2\rho^2\log d)$。
- Theorem 7.20 / (7.38)–(7.41) 印刷页 217：慢速率 $12\lVert\theta^*\rVert_1\lambda_n$，快速率 $9s\lambda_n^2/\kappa$。
- (A3)(A4) / Theorem 7.21 / (7.44)–(7.45) 印刷页 219–220：下特征值、相互不相干、PDW 阈值与 $\ell_\infty$ 界。
- Corollary 7.22 / (7.46)–(7.47) 印刷页 220–221：$\lambda_n$ 含 $\log(d-s)$。
- PDW (7.48)–(7.54)、Lemma 7.23 印刷页 222–224。
- §7.6 (7.55)–(7.59) 印刷页 224–227：Notes 只留骨架。
- Exercises 7.1–7.20 印刷页 229–235：全部进入 Solutions，未写入 Notes。

四处笔误嫌疑（保留原文，Notes 未写成已批准勘误）：

1. 印刷页 212 Example 7.15：正文 “relaxed basis pursuit program (7.19)”。(7.19) 是约束套索；(7.20) 才是松弛基追踪。
2. 印刷页 210 vs 212：Theorem 7.13(c) 陈述 (7.25c) 为 $4/\kappa$；证明末行与 Example 7.15 写 $8/\kappa$。由 $\kappa x^2\le Ax+B$、$A=4\sqrt s\lVert X^T w/n\rVert_\infty$，配平方给出 $x\le A/\kappa+\sqrt{2B/\kappa}$（即 $4/\kappa$）。
3. 印刷页 215 (7.33)：花括号内 $+2\lVert\theta^*_{S^c}\rVert_1$。由 (7.29) 加 Hölder 与 $\lambda_n\ge 2\lVert X^T w/n\rVert_\infty$，应变为 $+4$。速率阶不变。
4. 印刷页 204–205 Proposition 7.11：先定义 $S$ 为 $s$ 个最大坐标，随后下界改写 $\widetilde\theta_{S_0}$。论证需 $S_0=S$。

非阻断：Exercise 7.7(b) 正文 §7.2.3、Figure 7.3、Exercises 7.15/7.20 一律用 $n\gtrsim s\log(ed/s)$。Solutions 按此解读，并标明若印次出现 $\log(es/d)$ 则为排版笔误。

### 数学、假设与维度

**Theorem 7.8。** $\lVert\widehat\theta\rVert_1\le\lVert\theta^*\rVert_1$ 与 $S$-稀疏推出 $\widehat\Delta\in\mathbb C(S)$；再交 $\mathrm{null}(X)$。反向用辅助问题 (7.11) 与 $[0,-\theta^*_{S^c}]$ 的可行性。Notes 与原页一致。

**(7.25a) 的锥。** $\lambda_n\ge 2\lVert X^T w/n\rVert_\infty$ 把 Hölder 项收成 $\lambda_n\lVert\widehat\Delta\rVert_1$，加上 $2\lambda_n(\lVert\widehat\Delta_S\rVert_1-\lVert\widehat\Delta_{S^c}\rVert_1)$ 得到系数 $3$。RE 给出 $\kappa x^2\le 3\lambda_n\sqrt s\,x$。自测第 2 题正确。

**(7.25c) 常数。** 证明得到 $\kappa x^2\le 4\sqrt s\,\lVert X^T w/n\rVert_\infty\,x+2(b^2-\lVert w\rVert_2^2/(2n))$。陈述用 $4/\kappa$ 与 $2/\sqrt\kappa$ 可由 $x\le A/\kappa+\sqrt{2B/\kappa}$ 读出（$\sqrt{2B/\kappa}=2\kappa^{-1/2}\sqrt{b^2-\cdots}$）。证明末行的 $8/\kappa$ 是把 $A/\kappa$ 再乘 2。Notes 跟陈述并标明差异。

**慢/快速率。** (7.38)：$\lVert\widehat\Delta\rVert_1\le 4\lVert\theta^*\rVert_1$ 代入 (7.29) 得 $12\lVert\theta^*\rVert_1\lambda_n$。 (7.39)：$\frac1n\lVert X\widehat\Delta\rVert_2^2\le 3\lambda_n\sqrt s\,\lVert\widehat\Delta\rVert_2$ 再套 RE 得 $9s\lambda_n^2/\kappa$。相同列破坏 RE 但不破坏 (7.38)；自测第 4 题正确。

**PDW。** 严格对偶可行 $\lVert\widehat z_{S^c}\rVert_\infty\le\tfrac12(1+\alpha)<1$ 来自 (A4) 的 $\alpha$ 与 (7.44) 的 $\tfrac12(1-\alpha)$。Lemma 7.23 用 $\langle\widehat z,\widetilde\theta\rangle=\lVert\widetilde\theta\rVert_1$ 迫使 $\widetilde\theta_{S^c}=0$，再用 (A3) 的严格凸给唯一性。Notes 未把 (A4) 说成 RE，也未把 $\ell_2$ 小说成支撑恢复。

**Theorem 7.16 常数。** PNG 印刷页 214 明确 $c_1=\tfrac18$、$c_2=50$。Exercise 7.11 的均匀 RE 基数与 Remark 中 $c_1\gamma_{\min}n/(32c_2\rho^2\log d)$ 一致（$\alpha=3$ 时 $(1+\alpha)^{-2}=1/16$ 与 $32$ 对 $2$ 的差异在 Exercise 7.11 的 $2c_2$ 对 Remark 的 $32c_2$）。

**未发明定理。** RIP / 成对不相干的充分性、尖峰单位上二者失败、慢速率不可改进、快速率对多项式时间 $s$-稀疏估计需要 RE，均指向教材或 §7.7，Notes 未伪造证明。§7.6 只保留 Gordon 比较与壳事件，细节指回教材。

自测第 3 题：二次墙 $s^2\log d$ 对 $s\log(ed/s)$，尖峰单位 $\mu=1/2$ 时两证书失败而 RE 仍在 $n\gtrsim s\log d$ 成立——与 Example 7.18 / Figure 7.4 一致。

### 结构、可访问性、链接与渲染

读者栏目：本章导览、学习目标（5 个可观察动词，落在 3–7）、必要先修（凸松弛 / 锥上强凸 / 次梯度，对陈希孺读者是真缺口）、常见错误、轻量自测（5 题，`<details>` 含「参考答案」）、本章小结、术语对照、来源定位。标题由 `#` 到 `##` 到 `### 关键推导`（§7.4 的关键推导为 `##`，避免跳级）。Notes 汉语、英文术语首次给出；Solutions 英语。来源定位给出印刷/PDF 页码及 Solutions 相对链接。未把习题完整解答写入 Notes。§7.6 简要说明、§7.7 指回教材，与清单一致。

Solutions 锁定 7.1–7.20，每题 Stem (abridged) + Solution；多小问按 (a)(b)… 展开。Exercise 7.3 独立得到 $\gamma<1/2$ 已够限制零空间，并说明书中 $1/3$ 是更严的充分阈值。Exercise 7.7(b) 按正文 $s\log(ed/s)$ 求解。
