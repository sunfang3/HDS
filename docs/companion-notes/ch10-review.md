---
chapter_id: "ch10"
chapter_title: "Matrix estimation with rank constraints"
map_path: "docs/companion-notes/ch10-content-map.md"
notes_path: "notes/ch10-notes.qmd"
reviewed_at: "2026-08-31"
delivery_status: "Notes 草稿"
ppt_status: "未请求"
solutions_status: "未请求"
---

# 第 10 章审核报告

> 内部工件。对照印刷页 PNG（`scratch/ch10/p-331.png`–`p-365.png`）核验，不采用作者对勘误、覆盖或推导的结论作为已批准事实。文本层 `ch10.txt` 仅作索引；公式、命题框与图注以 PNG 为准。

## 范围与结论

- 审核范围：第 10 章内容清单、`notes/ch10-notes.qmd`。习题解答已起草于 `solutions/ch10-solutions.qmd`（Exercises 10.1–10.11），但按合同在 Notes 质检通过前不把 Solutions 标为完成。
- 主教材版本与页码：Martin J. Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series in Statistical and Probabilistic Mathematics No. 48, 2019, ISBN 978-1-108-49802-9；印刷页 312–346，PDF 页 331–365（PDF = 印刷 + 19）
- 当前结论：清单与 Notes 的来源覆盖、关键公式（对照 PNG）与结构栏目可通过作者核验；独立质检代理尚未另跑，故 `delivery_status` 保持 `Notes 草稿`。若干教材笔误嫌疑保持 `勘误待批`。
- 未关闭问题：见下方勘误表。无一处挡住 Notes 按印刷式加旁注的写法。
- 下一步允许动作：独立质检通过后将 `delivery_status` 改为 `Notes 质检通过`，再把 Solutions 从「已起草」升为 `完成`。

## 独立质检

| 检查面 | 审核者 | 结果 | 简短证据或问题定位 |
|---|---|---|---|
| 内容清单与来源原页 | 作者核验（对照印刷页 PNG） | 通过 | (10.1)–(10.57)、Proposition 10.6–10.7、Theorem 10.8/10.12/10.17、Corollary 10.9/10.10/10.13/10.14/10.18/10.22、Example 10.1–10.21、Figure 10.1–10.2 均入清单；Notes 按节序转写。关键式与 `p-331`–`p-360` 一致，见摘记。 |
| 数学、假设与维度 | 作者核验（对照印刷页 PNG） | 通过 | 锥上 $\sqrt{2r}$ 来自 $\overline{\mathbb M}$ 秩 $\le 2r$；(10.19) 为 (10.18) 的恰低秩特化；相位恢复证明集合 $A_1(\sqrt{\rho})$ 与印刷 (10.30) 方向相反，Notes 已并陈。未发现 Notes 虚构定理。 |
| 结构、可访问性、链接与渲染 | 作者核验 | 通过 | 七个读者栏目齐全；标题无跳级；Notes 汉语 / Solutions 英语；来源定位链到 `../solutions/ch10-solutions.qmd`。习题不进 Notes。 |

## 派生产物

| 产物 | 请求范围 | 状态 | 自身检查证据或受阻原因 |
|---|---|---|---|
| PPT | 未请求 | 未请求 | 用户未请求 PPT。 |
| Solutions | 全部习题（§10.9 Exercises 10.1–10.11） | 未请求 | 已起草 `solutions/ch10-solutions.qmd` 并独立求解；按合同在 Notes 质检通过前保持 `未请求`，不升为 `完成`。 |

## 核对摘记

### 内容清单与来源原页

对照 `p-331.png`–`p-365.png` 逐条核对编号公式（OCR 不可信）：

- (10.1)–(10.5) 印刷页 312–313：迹内积、Frobenius、观测算子、核范数正则 LS、核范数定义。Notes 一致。
- Example 10.1–10.5 与 (10.6)–(10.11)：多元回归掩码 $X_{j\ell}=Z^T E_{j\ell}$；补全重标定 $\sqrt{d_1 d_2}$；相位恢复提升；VAR (10.10)–(10.11)。Notes 一致。
- (10.12)–(10.15) 印刷页 317–319：$\mathbb M$ 秩 $\le r$，$\overline{\mathbb M}$ 十字块秩 $\le 2r$，可分解，锥因子 3 与 4。Notes 一致。
- (10.17)–(10.21) 印刷页 319–321：RSC 容忍 $(d_1+d_2)/n$；神谕 (10.18)；恰低秩 (10.19)；$\Phi^*$ 曲率 (10.20)；算子范数 (10.21) 的 $3\sqrt{2}\,\lambda_n/\kappa$。PNG 确认 $\mathbb G(\lambda_n)$ 的门槛是 $\lambda_n/2$。
- Theorem 10.8 / Corollary 10.9–10.10 / (10.22)–(10.27)：$\rho^2(\Sigma)$ 定义、无噪 $n\gtrsim r(d_1+d_2)$、含噪 (10.25) 的 $125$ 与 $\lambda_n=10\sigma\rho(\cdot)$、$\ell_q$ 球 (10.26)–(10.27)。Notes 一致。
- (10.28)–(10.31)、Theorem 10.12、Corollary 10.13：SDP (10.29)、印刷锥 (10.30)、$A_1(\sqrt{\rho})$、(10.31a) 印刷系数。Notes 保留原文并标 `勘误待批`。
- Corollary 10.14 / (10.32)–(10.35)：印刷 $(Y,Z)\in\mathbb R^{n\times T}\times\mathbb R^{p\times T}$ 与 Example 10.1 冲突。Notes 按 $Z\in\mathbb R^{n\times p}$ 解读。
- Theorem 10.17 / Corollary 10.18 / (10.36)–(10.44)：尖刺比 (10.40) 带 $\sqrt{d_1 d_2}$；一致 RSC；$\ell_\infty$ 约束补全；(10.43) 的 $\max\{\sigma^2,\alpha^2\}r(d\log d)/n$。Notes 一致。
- (10.49)–(10.57)：可加分解；印刷 (10.53) 写 $\|\Lambda\|_2$，证明用核范数。Notes 并陈。

Figure 10.1（Netflix / Jester）与 Figure 10.2（Frobenius 对 $n$ 与对 $n/(rd)$）均入清单；图注 $d\in\{40,80,160\}$ 与正文 $d^2\in\{400,1600,6400\}$ 不一致，标 `勘误待批`。

### 数学、假设与维度

**锥与 $\sqrt{2r}$。** (10.14) 的十字表示使 $\overline{\mathbb M}$ 秩 $\le 2r$，故 $\Psi(\overline{\mathbb M})\le\sqrt{2r}$。无约束核范数极小（Exercise 10.4）给出因子 $1$；正则锥 (10.15) 给出因子 $3$，合起来 $\|\widehat\Delta\|_{\mathrm{nuc}}\le 4\sqrt{2r}\,\|\widehat\Delta\|_{\mathrm{F}}$。Proposition 10.6 的 $r\le\kappa n/(128 c_0(d_1+d_2))$ 正是 $\tau_n^2\Psi^2\le\kappa/64$。Notes 未把 $\sqrt{r}$ 与 $\sqrt{2r}$ 混用。

**(10.19) 还原。** 恰低秩时 $\sum_{j>r}\sigma_j=0$，(10.18) 只剩 $(9/2)(\lambda_n^2/\kappa^2)r$。Notes 一致。

**相位恢复锥。** 核范数 $\ge$ Frobenius，印刷 (10.30) 在 $\rho\ge 1$ 时含全体矩阵。Corollary 10.13 证明导出 $\|\widehat\Delta\|_{\mathrm{nuc}}\le\sqrt{2}\,\|\widehat\Delta\|_{\mathrm{F}}$，即 $A_1(\sqrt{2})$。Notes 保留印刷式并指向证明集合。

**(10.31a)。** 对称矩阵 Wick：$ \mathbb E[(x^T\Delta x)^2]=2\|\Delta\|_{\mathrm{F}}^2+(\mathrm{tr}\Delta)^2$。印刷把 $2$ 写在迹上。标准正态 $\mathbb E[Z^4]=3$ 而非印刷的 $4$；$\mathbb E[Z^8]=105$ 正确。Notes/Solutions 写出正确恒等式。

**(10.53) 对偶。** 若正则真是 $\omega_n\|\Lambda\|_2$，对偶应是核范数。印刷 (10.57) 与证明中的 $\Phi_{\omega_n}=\|\Gamma\|_1+\omega_n\|\Lambda\|_{\mathrm{nuc}}$ 一致，故印刷 (10.53) 的 $\|\Lambda\|_2$ 是核范数的误排。

**VAR Lyapunov。** $\|\Theta^*\|_2<1$ 足以保证 (10.58) 有 $\Sigma\succ 0$（Exercise 10.2(c)）；反之只推出谱半径 $<1$。反例 $\Theta^*=\begin{pmatrix}0&2\\0&0\end{pmatrix}$。Solutions 给出反例；Notes 不抄习题。

**未发明定理。** Gordon–Slepian 用于 Theorem 10.8 指向 Exercise 10.6；相位恢复单边律指向 Theorem 14.12；补全剥皮指向第 3、4、6 章。$\lambda_n$ 的数值因子（10、5、25、125）按原页抄录，不改成「某个常数」。

### 结构、可访问性、链接与渲染

读者栏目：本章导览、学习目标（6 个可观察动词）、必要先修（迹内积 / 核范数对偶 / $\overline{\mathbb M}$ 的 $2r$）、常见错误、轻量自测（5 题，`<details>` 含「参考答案」）、本章小结、术语对照、来源定位。标题由 `#` 到 `##` 到 `### 关键核对`，无跳级。Notes 汉语、英文术语首次给出；Solutions 英语。来源定位给出印刷/PDF 页码及 Solutions 相对链接。未把 §10.9 的完整解答写入 Notes。

## 勘误待批（汇总）

| 定位 | 印刷 | 拟议 | 状态 |
|---|---|---|---|
| Exercise 10.1 印刷页 343 | $\widehat\Sigma_{XY}$ | $\widehat\Sigma_{ZY}$ | 勘误待批 |
| §10.5 印刷页 329 | $Z\in\mathbb R^{p\times T}$ | $Z\in\mathbb R^{n\times p}$ | 勘误待批 |
| Theorem 10.12 / (10.30) 印刷页 327 | $\|\Theta\|_{\mathrm{F}}^2\le\rho\|\Theta\|_{\mathrm{nuc}}^2$ | $A_1(\sqrt{\rho})$：核范数 $\le\sqrt{\rho}$ Frobenius | 勘误待批 |
| (10.31a) 与 Ex. 10.9(b) | $\|\Delta\|_{\mathrm{F}}^2+2(\mathrm{tr}\Delta)^2$ | $2\|\Delta\|_{\mathrm{F}}^2+(\mathrm{tr}\Delta)^2$ | 勘误待批 |
| Thm 10.12 证明 $\mathbb E[x_j^4]$ | $4$ | $3$ | 勘误待批 |
| (10.53) 印刷页 340 | $\omega_n\|\Lambda\|_2$ | $\omega_n\|\Lambda\|_{\mathrm{nuc}}$ | 勘误待批 |
| Exercise 10.2(b) | 由 Lyapunov 解推出 $\|\Theta^*\|_2<1$ | 只推出谱半径 $<1$ | 勘误待批 |
| Exercise 10.3 | $\mathfrak X_n\to\mathbb R$ | $\to\mathbb R^n$ | 勘误待批 |
| Exercise 10.6 | $\mathbb B(t)\subset\mathbb R^{d_1\times d_1}$ | $d_1\times d_2$ | 勘误待批 |
| Exercise 10.10(c) | “Use part (c)” | part (b) | 勘误待批 |
| Figure 10.2 图注 印刷页 324 | $d\in\{40,80,160\}$ | 正文 $d^2\in\{400,1600,6400\}$ 即 $d\in\{20,40,80\}$ | 勘误待批 |
| §10.7 印刷页 339 | $\Theta^{\mathrm{bad}}$ from Example 10.16 | Example 10.15 | 勘误待批 |
