---
chapter_id: "ch15"
chapter_title: "Minimax lower bounds"
map_path: "docs/companion-notes/ch15-content-map.md"
notes_path: "notes/ch15-notes.qmd"
reviewed_at: "2026-08-31"
delivery_status: "Notes 质检通过"
ppt_status: "未请求"
solutions_status: "完成"
---

# 第 15 章审核报告

> 内部工件。对照印刷页 PNG（`scratch/ch15/p-504.png`–`p-542.png`）独立核验，不采用作者对勘误、覆盖或推导的结论。文本层 `ch15.txt` 仅作索引；公式以 PNG 为准。

## 范围与结论

- 审核范围：第 15 章内容清单、`notes/ch15-notes.qmd`、§15.6 Exercises 15.1–15.18 的独立解答（`solutions/ch15-solutions.qmd`）
- 主教材版本与页码：Martin J. Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series in Statistical and Probabilistic Mathematics No. 48, 2019, ISBN 978-1-108-49802-9；印刷页 485–523，PDF 页 504–542（PDF = 印刷 + 19）
- 当前结论：三个检查面均通过。六处教材笔误嫌疑保持 `勘误待批`。Notes 未把它们写成已批准勘误。
- 未关闭问题：见下方勘误表；均不挡住 Notes。
- 下一步允许动作：六处勘误待教师批准。

## 独立质检

| 检查面 | 审核者 | 结果 | 简短证据或问题定位 |
|---|---|---|---|
| 内容清单与来源原页 | 独立质检代理（对照印刷页 PNG） | 通过 | (15.1)–(15.67) 及 §§15.1–15.6、Figure 15.1–15.4、Prop./Lemma/Cor./Def. 15.1–15.25、Examples 15.4–15.23 均已入清单；Notes 按节序转写。关键式与原页一致，见下。 |
| 数学、假设与维度 | 独立质检代理（对照印刷页 PNG） | 通过 | 两点勒卡姆常数 $1/12$、$1/24$ 与平斯克改进 $1/8$、$1/16$ 复核通过；均匀位置 $n^{-2}$、二次泛函 $n^{-4/9}$、密度 $n^{-4/5}$、索伯列夫 $(\sigma^2/n)^{2\alpha/(2\alpha+1)}$ 的标度与原页一致。未发现 Notes 虚构定理。 |
| 结构、可访问性、链接与渲染 | 独立质检代理（对照印刷页 PNG） | 通过 | 七个读者栏目齐全；标题无跳级；Notes 汉语 / Solutions 英语；来源定位链到 `../solutions/ch15-solutions.qmd`。§15.6 未进入 Notes。 |

## 派生产物

| 产物 | 请求范围 | 状态 | 自身检查证据或受阻原因 |
|---|---|---|---|
| PPT | 未请求 | 未请求 | 用户未请求 PPT。 |
| Solutions | 全部习题（§15.6 Exercises 15.1–15.18） | 完成 | 题号已从印刷页 519–523 锁定为 15.1–15.18；独立求解并复核印刷常数（高斯 $1/8$ 与 $1/16$、均匀 $2/n^2$、Pinsker 伯努利形 (15.64)、GLM / 可加回归标度）。 |

## 核对摘记

### 内容清单与来源原页

对照 `p-504.png`–`p-542.png` 逐条核对编号公式（OCR 不可信）：

- (15.1)–(15.2) 印刷页 486：极小极大风险与复合损失。Notes 一致。
- Proposition 15.1 / (15.3) 印刷页 487：$\mathfrak M\ge\Phi(\delta)\inf\mathbb Q[\psi\neq J]$。Notes 一致。
- (15.4) 印刷页 488：最近邻检验。Figure 15.1 几何在 Notes 中简要说明。
- (15.5)–(15.6) 印刷页 489：TV 的集合上确界与 $\frac12\|p-q\|_{L^1}$。Notes 一致。
- (15.7)–(15.10) 印刷页 490：KL；平斯克 $\mathrm{TV}\le\sqrt{D/2}$；平方赫林格取值 $[0,2]$；勒卡姆不等式 $\mathrm{TV}\le H\sqrt{1-H^2/4}$。Notes 与 PNG 一致（文本层把根号结构拆碎）。
- (15.11)–(15.12) 印刷页 491：KL 可加；$\frac12 H^2$ 的乘积公式及 i.i.d. 上界 $\frac n2 H^2$。Notes 保留左边的 $1/2$。
- (15.13)–(15.14) 印刷页 491–492：贝叶斯风险 $\frac12\{1-\mathrm{TV}\}$；两点勒卡姆。Notes 一致。
- Example 15.4 / (15.15)–(15.16) 印刷页 492：$\delta=\sigma/(2\sqrt n)$ 时 TV $\le\frac12\sqrt{e-1}$，绝对值 $\ge\sigma/(12\sqrt n)$，MSE $\ge\sigma^2/(24n)$。样本均值 $\sqrt{2/\pi}\,\sigma/\sqrt n$ 与 $\sigma^2/n$。Notes 一致。
- Example 15.5 印刷页 493：$2\delta=1/(4n)$，MSE $\ge(1-1/\sqrt2)/128\cdot n^{-2}$。Notes 一致。
- (15.17)–(15.18) 印刷页 493–494：$\omega(\epsilon)$ 与 Corollary 15.6。Notes 一致。
- Example 15.7 / (15.19)–(15.20) 印刷页 494–495：帽函数，$H^2\le\frac13\delta^3$，$\delta^3=3/(4n)$，MSE $\gtrsim n^{-2/3}$。Figure 15.2 取 $\delta=0.12$。Notes 一致。
- Example 15.8 / (15.21)–(15.24) 印刷页 496–497：$\phi_j=(C/m^2)\phi(m(x-x_j))$，$\Phi(t)=t$ 给出 $n^{-1/2}$。Figure 15.3 四联图。Notes 一致。
- Lemma 15.9 / (15.25)–(15.26) 印刷页 498：凸包。Notes 一致。
- Example 15.10 / (15.27) 印刷页 499：$\ge 3\sigma/(20\sqrt n)$。Notes 一致。
- Example 15.11 / (15.28) 印刷页 499–500：$m^9=4b_0^2 n^2$ 给出 $n^{-4/9}$。Figure 15.4。Notes 一致。
- (15.29)–(15.34) 印刷页 501–502：互信息、范诺、凸性上界。Notes 一致。
- Example 15.13 印刷页 502–503：$\delta^2=\sigma^2/(20n)$ 给出 $\sigma^2/(80n)$。Notes 一致。
- (15.35)–(15.41) 印刷页 503–506：局部填装；线性回归 $\sigma^2\mathrm{rank}(\mathbf X)/(128n)$；密度 $n^{-4/5}$；稀疏回归 $(\sigma^2/\gamma_{2s}^2)s\log(ed/s)/n$。Notes 一致。
- Lemma 15.17 / (15.42)–(15.43) 印刷页 506–507。Notes 一致。
- Example 15.18 / (15.44) 印刷页 507：印刷第一项为 $\log(d+s-1)$。Notes 保留原文并按 Ensemble B 的 $M=d-s+1$ 解读。
- (15.47)–(15.50) 印刷页 509–511：尖刺模型与 PCA $\min\{(1+\nu)d/(\nu^2 n),1\}$。Notes 一致。
- Example 15.20 印刷页 511–512：印刷先写 $\log(d-s-1)$，随后比值用 $\log(d-s+1)$。Notes 按 $d-s+1$。
- Lemma 15.21 / (15.51)–(15.53) 印刷页 512–513。Notes 一致。
- Examples 15.22–15.23 / (15.54)–(15.56) 印刷页 513–515：$n^{-4/5}$ 与 $(\sigma^2/n)^{2\alpha/(2\alpha+1)}$。Notes 一致。
- Definitions 15.24–15.25 / (15.57)–(15.62) 印刷页 516–518。Notes 按 $-\int q\log q$ 写条件熵，并标明印刷缺负号、链式法则写错、范诺证明末句缺 $q_e$。
- §15.5 指回教材；§15.6 不进入 Notes。处理正确。

六处笔误嫌疑（保留原文，Notes 未写成已批准勘误）：

1. 印刷页 516 Definition 15.25 (15.59)：条件熵展开缺负号。Definition 15.24 明确 $H=-\int q\log q$。
2. 印刷页 517 (15.60c)：$H(X,Y\mid Z)=H(X\mid Z)+H(X\mid Y,Z)$。应为 $H(X\mid Z)+H(Y\mid X,Z)$。
3. 印刷页 518 范诺证明末句：$H(V,J\mid Z)\le h(q_e)+\log(M-1)$。按 $H(J\mid V,Z)=q_e H(J\mid Z,V=1)$ 应为 $h(q_e)+q_e\log(M-1)$ 才能得 (15.61)。
4. 印刷页 505 Example 15.15：$(\sqrt{f_\alpha}+\sqrt{f_\beta})^2=2(f_\alpha+f_\beta)\le 4$。展开是 $f_\alpha+f_\beta+2\sqrt{f_\alpha f_\beta}$；$\alpha_j\neq\beta_j$ 时 $f_\alpha+f_\beta=2$，故 $4$ 是上界不是恒等。
5. 印刷页 507 (15.44) 第一项分子写 $\log(d+s-1)$。Ensemble B 明确 $M=d-s+1$，印刷页 509 亦写 $\log(d-s+1)>4\log 2$。
6. 印刷页 512 Example 15.20：正文写 $\log M=\log(d-s-1)$，随后比值用 $\log(d-s+1)$，且 $M=\lvert S^c\rvert=d-s+1$。

### 数学、假设与维度

**(15.16) 的 $\sqrt{e-1}$。** $\delta=\sigma/(2\sqrt n)$ 使 $4n\delta^2/\sigma^2=1$，故 $\mathrm{TV}^2\le(e-1)/4$、$\mathrm{TV}\le\frac12\sqrt{e-1}$。$\frac12\{1-\frac12\sqrt{e-1}\}\ge 1/6$ 因为 $\sqrt{e-1}\approx 1.311$。$\delta/6=\sigma/(12\sqrt n)$。MSE 同因子给出 $\sigma^2/(24n)$。Notes 与 PNG 一致。

**Exercise 15.8 平斯克改进。** $D=2n\delta^2/\sigma^2$，$\mathrm{TV}\le\delta\sqrt n/\sigma$。同一 $\delta=\sigma/(2\sqrt n)$ 给出 $\mathrm{TV}\le 1/2$，绝对值 $\ge\delta/4=\sigma/(8\sqrt n)$，MSE $\ge\delta^2/4=\sigma^2/(16n)$。Solutions 复核了印刷常数。

**均匀位置。** $H^2=2\lvert\theta'-\theta\rvert$，$2\delta=1/(4n)$ 使 $\frac12 H^2(\mathbb U^n)\le 1/4$，从而 $\mathrm{TV}^2\le 1/2$。$\delta=1/(8n)$，$\Phi(\delta)/2=\delta^2/2=1/(128 n^2)$，乘 $\{1-1/\sqrt2\}$。Exercise 15.9：$U_{(1)}$ 的二阶矩 $2/((n+1)(n+2))\le 2/n^2$。

**二次泛函阶。** 两点：$m\sim n^{1/4}$，$\theta(g)\sim 1/m^2\sim n^{-1/2}$。凸包：$H^2(\mathbb U^n\Vert\mathbb Q)\lesssim n^2/m^9$，取 $m\sim n^{2/9}$ 则 $1/m^2\sim n^{-4/9}$。Notes 正确区分“下界变大”（$-4/9>-1/2$）。

**线性回归 (15.37)。** $D=\|X\Delta\theta\|_2^2/(2\sigma^2)\le 32 n\delta^2/\sigma^2$（上界 $8\delta$ 代入）。$\delta^2=\sigma^2 r/(64n)$ 配合 $\log M\ge r\log 2$ 给出印刷的 $1/128$。

**范诺 (15.61) $\to$ (15.31)。** $H(J\mid Z)=\log M-I$，$h(q_e)\le\log 2$，且须保留 $q_e\log(M-1)\le q_e\log M$。印刷末句丢掉 $q_e$ 后左端过大，推导不闭合。Notes 补 $q_e$ 并标 `勘误待批`。

**未发明定理。** Kolmogorov / MP 未出现。Assouad、Birgé–Massart (15.28)、Yang–Barron 熵指数 $(1/\delta)^{1/2}$ 与 $(1/\delta)^{1/\alpha}$ 均指回教材或第 5 章。Corollary 8.7、Example 13.8 仅作上界对照。$\sqrt{2\log d/n}$ 未在本章出现。

自测第 2 题：平斯克两点给出 $\sigma/(8\sqrt n)$，与 Exercise 15.8 及 (15.16a) 的 $1/12$ 对照正确。

### 结构、可访问性、链接与渲染

读者栏目：本章导览、学习目标（6 个可观察动词，落在 3–7）、必要先修（半度量 / TV 与贝叶斯风险 / 互信息即平均 KL）、常见错误、轻量自测（5 题，`<details>` 含「参考答案」）、本章小结、术语对照、来源定位。标题由 `#` 到 `##`，无跳级。Notes 汉语、英文术语首次给出（勒卡姆 Le Cam、范诺 Fano、极小极大保持中文）。Solutions 英语。来源定位给出印刷/PDF 页码及 Solutions 相对链接。§15.6 未写入 Notes。术语表单元格无未转义 `|`。
