---
chapter_id: "ch02"
chapter_title: "Basic tail and concentration bounds"
map_path: "docs/companion-notes/ch02-content-map.md"
notes_path: "notes/ch02-notes.qmd"
reviewed_at: "2026-08-31"
delivery_status: "Notes 质检通过"
ppt_status: "未请求"
solutions_status: "未请求"
---

# 第 2 章审核报告

> 内部工件。对照印刷页 PNG（`scratch/ch02/p-040.png`–`p-076.png`）独立核验，不采用作者对覆盖、推导或勘误的结论。文本层 `ch02.txt` 仅作索引，公式以 PNG 为准。

## 范围与结论

- 审核范围：第 2 章内容清单与 `notes/ch02-notes.qmd`（不含习题解答）
- 主教材版本与页码：Martin J. Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series in Statistical and Probabilistic Mathematics No. 48, 2019, ISBN 978-1-108-49802-9；印刷页 21–57，PDF 页 40–76（PDF = 印刷 + 19）
- 当前结论：三个检查面均通过。关键定义、霍夫丁 / 伯恩斯坦 / 阿祖马–McDiarmid / 高斯利普希茨，以及 Notes 中出现的编号式 (2.1)–(2.46) 与原页一致。未改 Notes。
- 未关闭问题：Example 2.24 的 $n$ 未定义；印刷页 28 把伯恩斯坦条件写成 (2.16)；Appendix B 把 $\gamma$ 说成幂级数收敛半径（与 Theorem 2.13(IV) 互斥）。习题页另有三处嫌疑，不进入 Notes。均保持 `勘误待批`。
- 下一步允许动作：Notes 可作后续章合同；PPT / Solutions 仍为未请求。

## 独立质检

| 检查面 | 审核者 | 结果 | 简短证据或问题定位 |
|---|---|---|---|
| 内容清单与来源原页 | 独立质检代理（对照印刷页 PNG） | 通过 | §§2.1–2.7、Definition 2.2/2.7、Proposition 2.5/2.9/2.10/2.14、Theorem 2.6/2.13/2.19/2.26、Corollary 2.20/2.21、Lemma 2.27 及 (2.1)–(2.52) 均已入清单；Notes 按节序转写，习题 2.1–2.22 不进入 Notes。 |
| 数学、假设与维度 | 独立质检代理（对照印刷页 PNG） | 通过 | 次高斯 / 次指数定义域、霍夫丁 $\sigma=(b-a)/2$、伯恩斯坦分母 $\sigma^2+bt$、鞅差条件矩母函数、McDiarmid $L_k$、Theorem 2.26 参数 $L$（正文证明 $\pi L/2$）均与原页一致。未发现 Notes 虚构定理。 |
| 结构、可访问性、链接与渲染 | 独立质检代理（对照印刷页 PNG） | 通过 | 七个读者栏目齐全；学习目标 5 条；标题无跳级；Notes 汉语；来源定位含印刷/PDF 页。自测含「参考答案」。 |

## 派生产物

| 产物 | 请求范围 | 状态 | 自身检查证据或受阻原因 |
|---|---|---|---|
| PPT | 未请求 | 未请求 | 用户未请求 PPT。 |
| Solutions | 未请求 | 未请求 | 用户要求本审核保持未请求；即使 Solutions 并行撰写，亦不在本报告验收。 |

## 核对摘记

### 内容清单与来源原页

对照 `p-040.png`–`p-076.png`。清单覆盖章首至 §2.7；正式对象单独成行；`并入相关内容` 均有目标；习题 2.1–2.22 为 `不进入 Notes`。关键纳入项核验列为 `原页已核`。

**定义与主定理（原页）：**

- Definition 2.2（印刷页 23，PDF 42）：$\mathbb E[e^{\lambda(X-\mu)}]\le e^{\sigma^2\lambda^2/2}$，对一切 $\lambda\in\mathbb R$。Notes (2.8) 一致。
- Definition 2.7（印刷页 26，PDF 45）：同一上界对 $\lvert\lambda\rvert<1/\alpha$；$\alpha=0$ 时 $1/\alpha=+\infty$。Notes (2.13) 一致。
- Proposition 2.5 / (2.10)（印刷页 24，PDF 43）：独立次高斯和上尾 $\exp(-t^2/(2\sum\sigma_i^2))$。Notes 一致。
- (2.11)（印刷页 25，PDF 44）：有界时 $\sigma=(b-a)/2$ 代入得 $e^{-2t^2/(n(b-a)^2)}$。Notes 一致。
- Proposition 2.10 / (2.17a)–(2.17b)（印刷页 28，PDF 47）：矩母函数 $( \lambda^2\sigma^2/2)/(1-b\lvert\lambda\rvert)$；集中 $2e^{-t^2/(2(\sigma^2+bt))}$。Notes 把 (2.17a) 指回 (2.16)，(2.17b) 原式保留。
- Corollary 2.20 / (2.30)（印刷页 36，PDF 55）：$2\exp(-2t^2/\sum(b_k-a_k)^2)$。Notes 一致；指数中的 $2$ 来自 $\sigma\le(b-a)/2$。
- Corollary 2.21 / (2.33)（印刷页 37，PDF 56）：$2\exp(-2t^2/\sum L_k^2)$。汉明特例 (2.35) 为 $2e^{-2t^2/(nL^2)}$。Notes 一致。
- Theorem 2.26 / (2.39)（印刷页 40，PDF 59）：标准高斯向量的 $L$-利普希茨函数参数 $\le L$，尾 $2e^{-t^2/(2L^2)}$。Notes 同时写明正文只证 $\pi L/2$ 与 $2\exp(-2t^2/(\pi^2 L^2))$，锐常数指回文献。与原页证明策略一致。

**编号式 (2.1)–(2.46) 在 Notes 中出现者，均与 PNG 同型：**

- (2.1)–(2.5) 印刷页 21–22：马尔可夫 / 切比雪夫 / $k$ 阶矩 / 指数马尔可夫 / 切尔诺夫。切尔诺夫对 $\lambda\in[0,b]$ 取 $\inf$。
- (2.6)–(2.9) 印刷页 22–23：高斯矩母函数、上尾、次高斯定义、两尾 $2e^{-t^2/(2\sigma^2)}$。原页 (2.9) 写 $t\in\mathbb R$；Notes 照抄（$t<0$ 时事件恒真，属教材惯用）。
- (2.10)–(2.11) 见上。Theorem 2.6 的 (2.12a)–(2.12d) 印在印刷页 25：偶矩 $(2k)!\,\theta^{2k}/(2^k k!)$；平方指数矩 $1/\sqrt{1-\lambda}$，$\lambda\in[0,1)$。Notes 四条均在。
- (2.13)–(2.16) 印刷页 26–28：次指数；Example 2.8 的 $(\nu,\alpha)=(2,4)$ 与 (2.14)；伯恩斯坦条件从 $k=2$ 起为 $\tfrac12 k!\,\sigma^2 b^{k-2}$。
- Proposition 2.9 两段尾：二次 $0\le t\le\nu^2/\alpha$，线性 $t>\nu^2/\alpha$。Notes 陈述与原页命题框一致；推导段按原页证明用 $t<\nu^2/\alpha$ / $t\ge\nu^2/\alpha$，分界处两指数相等。
- (2.18) 印刷页 29：样本均值两段尾。原页求和指标写 $\sum_{i=1}^n(X_k-\mu_k)$；Notes 照抄。二次段 $-nt^2/(2(\nu_*^2/n))$ 即 $-n^2 t^2/(2\nu_*^2)$。
- (2.19)–(2.20) 印刷页 29–30：$\chi^2$ 在 $t\in(0,1)$ 为 $2e^{-nt^2/8}$；JL 为 $(1\pm\delta)$ 乘平方距离，$m>16\delta^{-2}\log(N/\varepsilon)$。
- Theorem 2.13 的 (2.21a)–(2.21b) 与 (II)(IV) 印刷页 31：$\gamma=\sup_{k\ge 2}(\mathbb E[\lvert X\rvert^k]/k!)^{1/k}$。Notes 有绝对值，与命题框一致。
- (2.22a)–(2.23) 印刷页 31：单侧伯恩斯坦分母 $1-b\lambda/3$，$\lambda\in[0,3/b)$；非负下尾分母为 $2n^{-1}\sum\mathbb E[Y_i^2]$，无线性项。
- (2.24)–(2.27) 印刷页 33–35：杜布鞅、定义 2.15、鞅差、望远镜。
- (2.28) 并入 Theorem 2.19：Notes 用文字给出二次 / 线性两段与系数 2，未再单列标签，与清单「并入」一致。
- (2.30)–(2.37) 印刷页 36–39：阿祖马、改坐标、有界差分、McDiarmid、汉明特例、$U$-统计、拉德马赫复杂度。$U$-统计 $L_k=4b/n$，$\sum L_k^2=16b^2/n$，尾 $2e^{-nt^2/(8b^2)}$，与原页算得一致。
- (2.38)–(2.40)、(2.44)、(2.46)–(2.47) 印刷页 40–43：欧氏利普希茨、高斯集中、插值引理、$\chi^2$ 利普希茨路径 $e^{-nt^2/18}$（$t\in[0,3]$）、高斯复杂度 $D(\mathcal A)$。

§2.4–2.5 按清单为简要说明（证明骨架，细节指回）；§2.6 指回教材；§2.7 不进入 Notes。节序为 2 → 2.1 / 2.1.1–2.1.4 → 2.2 / 2.2.1–2.2.2 → 2.3 → 2.4–2.6，无跳节。

**独立确认的来源异常（不挡 Notes）：**

1. Example 2.24 印刷页 39：尾界含 $n$，本例未定义 $n$。边指示向量维数是 $\binom{d}{2}$；代入 (2.35)、$t=n\delta$、$L=1$ 才得到印刷的 $2e^{-2n\delta^2}$。Notes 写明 $n=\binom{d}{2}$，并标待批，未写成已批准勘误。
2. 印刷页 28 段末：正文 “Bernstein condition (2.16)”。同页命题框与前一段均把 (2.15) 叫伯恩斯坦条件，(2.16) 是其矩母函数推论。Notes 命题与术语表按 (2.15) 解读。
3. 印刷页 49 Appendix B：正文称 $\gamma$ 为 (2.58) 的收敛半径；Theorem 2.13(IV) 的 $\gamma=\sup_k(\mathbb E[\lvert X\rvert^k]/k!)^{1/k}$ 是根检验下半径的**倒数**。Notes 写「倒数」，与编号定义一致、与附录那句不一致。清单未单列此项，建议补进勘误表，仍 `勘误待批`。
4. 习题 2.21–2.22 的三处嫌疑只影响 Solutions，本审核不验收。

### 数学、假设与维度

**次高斯对次指数。** (2.8) 要求整条实轴；(2.13) 只要求 $\lvert\lambda\rvert<1/\alpha$。Example 2.8：$\mathbb E[e^{\lambda(Z^2-1)}]=e^{-\lambda}/\sqrt{1-2\lambda}$ 仅 $\lambda<1/2$ 有限，故非次高斯；(2.14) 在 $\lvert\lambda\rvert<1/4$ 给出 $(\nu,\alpha)=(2,4)$。Notes 适用边界与自测第 1 题正确。

**霍夫丁常数。** Example 2.4 对称化得 $\sigma\le b-a$；Exercise 2.4 锐化到 $(b-a)/2$。代入 (2.10)：$2\sum\sigma_i^2=2n(b-a)^2/4=n(b-a)^2/2$，故指数 $-2t^2/(n(b-a)^2)$，即 (2.11)。阿祖马同一算术：条件区间长 $b_k-a_k$，参数 $(b_k-a_k)/2$，指数系数 2。

**伯恩斯坦相对霍夫丁。** $\lvert X-\mu\rvert\le b$ 时 Exercise 2.4 给出次高斯参数 $b$（区间 $[-b,b]$ 半长），不是 $b/2$。Notes 直觉框写「参数是 $b$（或 Exercise 2.4 的 $b/2$）」把两种 $b$ 的约定写在同一括号里，易混，但不改印刷公式。(2.17b) 在 $t$ 不太大时像参数 $\sigma$ 的次高斯；$\sigma^2\le b^2$，故从不劣于只看区间长度的界。由 (2.16) 在 $\lvert\lambda\rvert\le 1/(2b)$ 得 $1-b\lvert\lambda\rvert\ge 1/2$，从而次指数参数 $(\sqrt 2\,\sigma,\,2b)$，与原页一致。切尔诺夫取 $\lambda=t/(bt+\sigma^2)\in[0,1/b)$ 即 (2.17b)。

**独立次指数和与 $\chi^2$。** $\alpha_*=\max\alpha_k$，$\nu_*=\sqrt{\sum\nu_k^2}$。$Y=\sum Z_k^2$ 参数 $(2\sqrt n,4)$；平均值的分界 $\nu_*^2/(n\alpha_*)=1$，故 $t\in(0,1)$ 落在二次段，$2e^{-nt^2/8}$ 即 (2.19)。JL 对 $\binom{N}{2}$ 对点并界，取 $m>16\delta^{-2}\log(N/\varepsilon)$ 足够。

**单侧 (2.22)–(2.23)。** $h(u)=2(e^u-u-1)/u^2$；$k!\ge 2\cdot 3^{k-2}$ 给出 $h(\lambda b)\le(1-\lambda b/3)^{-1}$。非负 $Y_i$ 的下尾去掉 $b\delta/3$，分母只留二阶矩。Notes 代数核与原页证明一致。

**有界差分。** $D_k$ 落入长度 $L_k$ 的随机区间，用到坐标独立把条件期望写成对 $X_{k+1}^n$ 的普通期望。$U$-统计改一个样本动 $n-1$ 对：$(n-1)\cdot 2b/\binom{n}{2}=4b/n$。拉德马赫复杂度 $L_k=2\sup_a\lvert a_k\rvert$，参数 $2\sqrt{\sum_k\sup_a a_k^2}$；更锐的 $\sqrt{\sup_a\sum a_k^2}$ 原页指向 Example 3.5，Notes 未提前当成本章定理。

**高斯利普希茨。** $\lVert\nabla f\rVert_2\le L$ 时插值给出矩母函数 $\exp(\lambda^2\pi^2 L^2/8)$，即参数 $\pi L/2$。Example 2.28：$V=\lVert Z\rVert_2/\sqrt n$ 由 1-利普希茨欧氏范数再缩放，得到 $e^{-n\delta^2/2}$（原页单侧、无因子 2）。$(1+\delta)^2\le 1+3\delta$（$\delta\in[0,1]$）、$t=3\delta$ 得到 (2.44) 的 $e^{-nt^2/18}$。常数劣于 (2.19) 的 $1/8$，原页已比较。Notes 适用边界写明：无凸性时，任意次高斯坐标的利普希茨函数不必有维数无关集中（Ledoux），与印刷页 42、50 一致。

**附录骨架。** $(\mathrm{I})\Rightarrow(\mathrm{II})$ 用 $Z\sim N(0,2\sigma^2)$ 的米尔斯比，$c=\sqrt{8e}$。$(\mathrm{II})\Rightarrow(\mathrm{III})$ 原页用 $\theta=c\tau$（$c\ge 1$ 时 $c\le c^{2k}$）。$(\mathrm{III})\Rightarrow(\mathrm{I})$ 对称时参数 $\theta$，非对称时 $\sqrt 2\,\theta$。次指数链 $(\mathrm{I})\Leftrightarrow(\mathrm{II})\Leftrightarrow(\mathrm{III})$、$(\mathrm{II})\Leftrightarrow(\mathrm{IV})$ 与 Appendix B 一致。Notes 未把附录细节写成新定理。

**自测。** 第 1、2、4、5 题与正文一致。第 3 题定性（方差远小于区间平方时选伯恩斯坦）与印刷页 28 评注一致；计算把 (2.11)（和）与 (2.17b)（单个变量）接到同一 $t=2\sigma$，且「更精确」把指数写成 $-1/(2\sqrt n)$，直接代入是 $-4 n^{-1}/(2n^{-1}+4n^{-1/2})\sim -n^{-1/2}$。不挡定理核验；若修订 Notes，只需把比较对象改成同一随机变量。

未发明定理。必要先修只钉矩母函数邻域、塔性质、次高斯参数不是方差。

### 结构、可访问性、链接与渲染

读者栏目：本章导览、学习目标（5 个可观察动词，落在 3–7）、必要先修、常见错误、轻量自测（5 题，`<details>` 含「参考答案」）、本章小结、术语对照、来源定位。标题由 `#` 到 `##` 到 `### 关键推导`，无跳级。Notes 汉语；英文术语在次高斯 / 次指数 / 偏差 / 集中等处首次给出。作者补充标了 `作者解释`（塔性质、参数不是方差、多项式矩）。来源定位给出印刷页 21–50 / PDF 40–69，习题页 50–57 / PDF 69–76，以及 `../solutions/ch02-solutions.qmd`（Solutions 本审核不验收）。未把习题完整解答写入 Notes。术语表中文从通行名词委/教材译名；英文从教材。
