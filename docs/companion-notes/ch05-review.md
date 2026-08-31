---
chapter_id: "ch05"
chapter_title: "Metric entropy and its uses"
map_path: "docs/companion-notes/ch05-content-map.md"
notes_path: "notes/ch05-notes.qmd"
reviewed_at: "2026-08-31"
delivery_status: "Notes 质检通过"
ppt_status: "未请求"
solutions_status: "完成"
---

# 第 5 章审核报告

> 内部工件。对照印刷页 PNG（`scratch/ch05/p-140.png`–`p-177.png`）独立核验。文本层 `ch05.txt` 仅作索引；覆盖/填装定义、达德利积分、苏达科夫下界与习题页以 PNG 为准。

## 范围与结论

- 审核范围：第 5 章内容清单、`notes/ch05-notes.qmd`、§5.8 Exercises 5.1–5.14 的独立解答（`solutions/ch05-solutions.qmd`）
- 主教材版本与页码：Martin J. Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series in Statistical and Probabilistic Mathematics No. 48, 2019, ISBN 978-1-108-49802-9；印刷页 121–158，PDF 页 140–177（PDF = 印刷 + 19）
- 当前结论：三个检查面均通过；Notes 按节序转写 §§5.1–5.7，习题整节不进 Notes。六处教材笔误/符号混用保持 `勘误待批`。
- 未关闭问题：清单中六条勘误仍待教师批准（见下）。
- 下一步允许动作：勘误待批；术语由父代理合并进 `glossary.qmd`。

## 独立质检

| 检查面 | 审核者 | 结果 | 简短证据或问题定位 |
|---|---|---|---|
| 内容清单与来源原页 | 独立质检（对照印刷页 PNG） | 通过 | (5.1a)–(5.75)、Definitions 5.1/5.4/5.16/5.34/5.35、Lemma 5.5/5.7、Prop. 5.17/5.28、Thm. 5.22/5.25/5.27/5.30/5.36、Cor. 5.26、Figure 5.1–5.3、Exercises 5.1–5.14 均已入清单。Notes 按节序转写；§5.7 指回教材；§5.8 不进 Notes。 |
| 数学、假设与维度 | 独立质检（对照印刷页 PNG） | 通过 | (5.4)(5.8)(5.9)(5.33)(5.46)(5.63)(5.69) 与原页一致。一步法对数因子、达德利消对数、苏达科夫须高斯、高维 Lipschitz 熵 $(L/\delta)^d$ 的标度正确。未发现 Notes 虚构定理。 |
| 结构、可访问性、链接与渲染 | 独立质检 | 通过 | 七个读者栏目齐全；标题无跳级；Notes 汉语 / Solutions 英语；覆盖/填装沿用第 1 章；来源定位链到 `../solutions/ch05-solutions.qmd`。 |

## 派生产物

| 产物 | 请求范围 | 状态 | 自身检查证据或受阻原因 |
|---|---|---|---|
| PPT | 未请求 | 未请求 | 用户未请求 PPT。 |
| Solutions | 全部习题（§5.8 Exercises 5.1–5.14） | 完成 | 题号已从印刷页 154–158 / PDF 173–177 锁定；独立求解。5.14(a) 给出理论曲线 $1+\sqrt\alpha$ 与可复现试验说明，未跑 $n=1000$ 全网格。5.4(c) 证明 $K(\nu)=(2\nu)^{2\nu}$，与印刷 $(2\nu)^{2\nu-1}$ 同型。 |

## 核对摘记

### 内容清单与来源原页

对照 `p-140.png`–`p-177.png` 抽核编号公式（OCR 不可信）：

- (5.1a)–(5.1b) 印刷页 121：欧氏度量带根号；重标度汉明。Notes 一致。
- Definition 5.1 / Figure 5.1 印刷页 122：$\delta$-覆盖；$N(\delta;\mathbb T,\rho)$；填装为半径 $\delta/2$ 的不相交球。
- (5.2) 印刷页 123：$N(\delta;[-1,1],\lvert\cdot\rvert)\le 1/\delta+1$。同页 “for any point $\overline\theta\in[0,1]$” 见勘误。
- Definition 5.4、Lemma 5.5 / (5.4) 印刷页 124：$M(2\delta)\le N(\delta)\le M(\delta)$。
- Lemma 5.7 / (5.8) 印刷页 125：体积比。Example 5.8 / (5.9) 印刷页 126：$d\log(1/\delta)\le\log N\le d\log(1+2/\delta)$。
- (5.10) 印刷页 126–127：参数类。 (5.12) 印刷页 127：Lipschitz $\log N_\infty\asymp L/\delta$。
- (5.17) 印刷页 129：光滑类 $(1/\delta)^{1/(\alpha+\gamma)}$。印刷页 130 末式符号混用见勘误。
- (5.22)–(5.24) 印刷页 132：$\mathcal R(\mathbb T)\le\sqrt{\pi/2}\,\mathcal G(\mathbb T)$（PNG 明确有根号）。
- Definition 5.16 / (5.32) 印刷页 134：次高斯过程。Proposition 5.17 / (5.33) 印刷页 135：$4\sqrt{D^2\log N_X}$。
- (5.35)–(5.36) 印刷页 136：局部与朴素离散化。
- (5.39)–(5.41) 印刷页 137–138：谱范数；$6\sqrt{\log N_F}$；$(n+d)\log(1+2/\delta)$。
- (5.45)–(5.47) 印刷页 139–140：达德利积分与链式；$\varepsilon_m=D2^{-m}$。Figure 5.3 图注见勘误。
- (5.49)–(5.51) 印刷页 143：VC 熵与 GC 尾。
- Theorem 5.25 / (5.52)–(5.55) 印刷页 144。证明末行 $f$ 见勘误。
- Corollary 5.26、Theorem 5.27 印刷页 145–146。定理框缺括号见勘误。
- Theorem 5.30 / (5.63) 印刷页 148：$(\delta/2)\sqrt{\log M_X}$。Example 5.31 引 Example 5.9 见勘误。
- Definition 5.34–Theorem 5.36 / (5.65)–(5.69) 印刷页 150–151。
- Exercises 5.1–5.14 印刷页 154–158：题号连续，无缺失。5.14(d) 尾界 $2e^{-nt^2/2}$。

节序：章首 → 5.1 → 5.2 → 5.3 / 5.3.1–5.3.3 → 5.4 / 5.4.1–5.4.3 → 5.5 → 5.6 → 5.7（指回教材）。覆盖/填装沿用第 1 章译名。

### 数学、假设与维度

**填装–覆盖。** (5.4) 的 (a) 用三角不等式；(b) 用极大填装即覆盖。体积比 (5.8) 下界是覆盖的体积并，上界是极大 $(\delta/2)$-填装的不相交球。自身度量 (5.9) 与 Example 5.2/5.6 的 $d\log(1/\delta)$ 一致。

**一步法 vs 达德利。** 参数类熵 $\log(1/\delta)$：一步法取 $\delta\sim n^{-1/2}$ 留下 $\sqrt{\log n}$；达德利积分 $\int_0\sqrt{\log(1/u)}\,du<\infty$ 去掉对数。Lipschitz 熵 $1/\delta$ 给出 $n^{-1/3}$，一步法标度已对。VC 类 (5.50) 比 Lemma 4.14 少一个 $\log n$。

**高斯比较与下界。** 苏达科夫–费尔尼克由增量 $L^2$ 度量比较最大值；斯莱皮安是等方差特例。苏达科夫下界的比较过程 $Z_i\sim N(0,\delta^2/2)$ 使增量恰为 $\delta^2$。Notes 明确该下界不能搬到拉德马赫过程（$\ell_1$-球反例）。高斯收缩用 $\lVert\phi(\theta)-\phi(\theta')\rVert_2\le\lVert\theta-\theta'\rVert_2$。

**谱范数。** Example 5.19 上界 $\mathbb E[\lvert\lvert\lvert W\rvert\rvert\rvert_2]/\sqrt n\lesssim 1+\sqrt{d/n}$；Example 5.33 + Exercise 5.13 同阶下界；Exercise 5.14 用戈登比较把前置常数收到 $1$。

**未发明定理。** 一般链式、Gordon 不等式全文、Mitjagin 一般椭球熵均指回 §5.7。奥利茨尾的常数 $c_1$ 保持万有、不数值化。

自测第 2 题：$\delta=1/4$ 时 (5.9) 给出 $d\log 4$ 与 $d\log 9$，计算正确。

### 结构、可访问性、链接与渲染

读者栏目：本章导览、学习目标（5 个可观察动词）、必要先修（覆盖/填装译名、次高斯增量、有限最大值）、常见错误、轻量自测（5 题，`<details>` 含「参考答案」）、本章小结、术语对照、来源定位。标题由 `#` 到 `##` 到 `### 关键推导`，无跳级。Notes 汉语、英文术语首次给出；Solutions 英语。未把习题解写入 Notes。`execute: enabled: false` 与 `lang: zh-CN` 已设。

## 勘误待批（保留原文，未写成已批准）

1. Example 5.2 印刷页 123；PDF 页 142。构造 $[-1,1]$ 的覆盖时写 “for any point $\overline\theta\in[0,1]$”。Notes 按 $[-1,1]$ 读。
2. Example 5.11 印刷页 130；PDF 页 149。末式 $\log N(\delta;\mathscr F_{\alpha,\gamma},\lVert\cdot\rVert_\infty)\gtrsim(1/\delta)\asymp(1/\varepsilon)^{1/(\alpha+\gamma)}$ 把网格间距与覆盖半径都叫 $\delta$。Notes 以 (5.17) 为准。
3. Theorem 5.25 证明 印刷页 145；PDF 页 164。“second derivatives of $f$”；定理中的函数是 $F$。Notes 写 $F$。
4. Theorem 5.27 印刷页 146；PDF 页 165。定理框 “$(Y_1,\ldots,Y_N$, suppose that” 缺右括号。Notes 补全。
5. Example 5.31 印刷页 149；PDF 页 168。“From Example 5.9, the metric entropy of the ball $\mathbb B_2^d$”。单位球自身熵是 Example 5.8 / (5.9)。Notes 改引 5.8。
6. Figure 5.3 图注 印刷页 141；PDF 页 160。图注 $De^{-m}$-cover；正文 $\varepsilon_m=D2^{-m}$。Notes 按 $D2^{-m}$ 讲。
