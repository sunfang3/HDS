---
chapter_id: "ch13"
chapter_title: "Nonparametric least squares"
map_path: "docs/companion-notes/ch13-content-map.md"
notes_path: "notes/ch13-notes.qmd"
reviewed_at: "2026-08-31"
delivery_status: "Notes 质检通过"
ppt_status: "未请求"
solutions_status: "完成"
---

# 第 13 章审核报告

> 内部工件。对照印刷页 PNG（`scratch/ch13/p-435.png`–`p-471.png`）核验，不采用文本层对公式的结论。文本层 `ch13.txt` 仅作索引；公式以 PNG 为准。

## 范围与结论

- 审核范围：第 13 章内容清单、`notes/ch13-notes.qmd`、§13.6 习题 13.1–13.11 的独立解答（`solutions/ch13-solutions.qmd`）
- 主教材版本与页码：Martin J. Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series in Statistical and Probabilistic Mathematics No. 48, 2019, ISBN 978-1-108-49802-9；印刷页 416–452，PDF 页 435–471（PDF = 印刷 + 19）
- 当前结论：三个检查面均通过。Notes 按节序转写约束最小二乘、局部高斯复杂度、临界半径、神谕不等式与正则化/KRR。清单中的勘误一律保持 `勘误待批`，Notes 未写成已批准勘误。
- 未关闭问题：清单「来源异常与勘误」表中的笔误嫌疑（Figure 13.2 的 $\sigma$、Theorem 13.5 注记的 $2/\pi$ 与 $\|\cdot\|_2$、by/be、Lemma 13.12 的 non-decreasing、(13.53) 哑元、Example 13.15 缺 $R$、Example 13.20 末式 $R^2$ 对 $R^{2/3}$、Exercise 13.9 多余括号与 $\sum_{j=1}^n$）。均不挡住 Notes。
- 下一步允许动作：勘误待教师批准；Solutions 已按锁定题号独立写成。

## 独立质检

| 检查面 | 审核者 | 结果 | 简短证据或问题定位 |
|---|---|---|---|
| 内容清单与来源原页 | 本章写作代理（对照印刷页 PNG） | 通过 | (13.1)–(13.70)、Theorem 13.5/13.13/13.17、Corollary 13.7/13.18、Lemma 13.6/13.12/13.22/13.23、Example 13.1–13.21、Figure 13.1–13.5 均已入清单；Notes 按节序转写。关键式与原页一致，见下。 |
| 数学、假设与维度 | 本章写作代理（对照印刷页 PNG） | 通过 | 临界不等式与星形非增（Lemma 13.6）一致；Theorem 13.5 平方误差尺度为 $t\delta_n$；Lipschitz $n^{-2/3}$、凸 $n^{-4/5}$、Fourier $n^{-2\alpha/(2\alpha+1)}$、KRR 谱条件 (13.56) 与原页一致。未发现 Notes 虚构定理。 |
| 结构、可访问性、链接与渲染 | 本章写作代理（对照印刷页 PNG） | 通过 | 读者栏目齐全；标题无跳级；Notes 汉语 / Solutions 英语；来源定位链到 `../solutions/ch13-solutions.qmd`。习题不进 Notes。 |

## 派生产物

| 产物 | 请求范围 | 状态 | 自身检查证据或受阻原因 |
|---|---|---|---|
| PPT | 未请求 | 未请求 | 用户未请求 PPT。 |
| Solutions | 全部习题（§13.6 的 13.1–13.11） | 完成 | 题号从印刷页 449–452 锁定；独立求解。13.5(b) 复算得 $8/\pi$；13.6 慢/快速率与局部化一致；13.9 按 $\sum_{j=1}^d$ 与去掉多余括号理解。 |

## 核对摘记

### 内容清单与来源原页

对照 `p-435.png`–`p-471.png` 逐条核对编号公式（OCR 不可信）：

- (13.1)–(13.3) 印刷页 416：总体 MSE、回归函数 $f^*=\mathbb E[Y\mid X=x]$、经验 MSE。Notes 一致。
- (13.4)–(13.5) 印刷页 417：超额风险 $=\|f^*-f\|_{L^2(\mathbb P)}^2$；$\|f-f^*\|_n$ 与固定设计。Notes 一致。
- (13.6)–(13.8) 印刷页 417–418：生成模型、$n^{-1}$ 约束最小二乘、$\lambda_n\|f\|_{\mathcal F}^2$ 正则化。Notes 标明 (13.52) 改用 $1/(2n)$。
- Example 13.1–13.4 印刷页 418–420：线性 / 岭 / $\ell_q$ / Lasso；三次样条 (13.9)–(13.10)；KRR 表示 $\widehat\alpha=(\mathbf K+\lambda_n I_n)^{-1}y/\sqrt n$；凸回归 (13.11)–(13.14)，$N=n(d+1)$、$2\binom n2$ 约束。Notes 一致。
- (13.15)–(13.17) 印刷页 421–422：$\mathcal F^*$、局部高斯复杂度、临界不等式 $\mathcal G_n(\delta)/\delta\le\delta/(2\sigma)$。Figure 13.2 正文 $\sigma=1/2$、图注 $\sigma=1$。Notes 跟正文。
- (13.18)–(13.20) 印刷页 423：基本不等式、启发式、Theorem 13.5 尾 $e^{-nt\delta_n/(2\sigma^2)}$。平方误差阈值是 $16t\delta_n$ 不是 $16t\delta_n^2$。Notes 在常见错误里钉死。
- (13.21)–(13.23)、Lemma 13.6 印刷页 424–425：星形包、差类、$\mathcal G_n(\delta)/\delta$ 非增。Notes 一致。
- Corollary 13.7 (13.24) 印刷页 426：积分下限 $\delta^2/(4\sigma)$，右端 $\delta^2/(4\sigma)$，前置 $16/\sqrt n$。Notes 一致。
- Example 13.8–13.11 印刷页 427–430：(13.26) $\sigma^2\mathrm{rank}(\mathbf X)/n$；(13.30)–(13.31) $\ell_q$ 速率 $R_q(\sigma^2\log d/n)^{1-q/2}$；(13.33) $(L\sigma^2/n)^{2/3}$；(13.35) $(\sigma^2/n)^{4/5}$。Notes 一致。
- Lemma 13.12、(13.36)–(13.41) 印刷页 431–432：事件 $\mathcal A(u)$、缩放到 $\|g\|_n=u$、利普希茨 $\sigma u/\sqrt n$。印刷页 432 写 non-decreasing，随后一行按非增使用。Notes 按非增。
- Theorem 13.13 (13.42a,b)、(13.43a,b) 印刷页 433：神谕不等式。Notes 一致。
- Example 13.14–13.16 印刷页 434–437：(13.45) 尾系数 $+\sigma^2 T/n$；(13.47) $c'R/M^{2\alpha}$ 与 Example 13.15 无 $R$ 的系数界冲突；(13.48)–(13.50) $\delta_n^2\simeq\sigma^2 s\log(ed/s)/n$。Notes 按带 $R$ 陈述。
- (13.52)–(13.56)、Theorem 13.17、Corollary 13.18 印刷页 439–440：$1/(2n)$、$\mathbb B_{\partial\mathcal F}(3)$、$\lambda_n\ge 2\delta_n^2$、KRR 临界 $\sqrt{2/n}\sqrt{\sum\min\{\delta^2,\widehat\mu_j\}}\le(R/(4\sigma))\delta^2$。(13.53) 哑元 $g$、被积 $f(x_i)$。Notes 写 $g(x_i)$。
- Example 13.19–13.21、Lemma 13.22 印刷页 440–444：有限秩 $m$、Sobolev $\mu_j\asymp j^{-2}$、高斯核 $e^{-cj\log j}$。Example 13.20 末式 $R^2(\sigma^2/n)^{2/3}$ 与同页 $\delta_n^2\simeq(\sigma^2/(R^2 n))^{2/3}$ 不一致。Notes 写 $R^{2/3}(\sigma^2/n)^{2/3}$。
- Lemma 13.23 与剥皮 (13.63)–(13.69) 印刷页 446–448：Notes 按清单简要说明。
- §13.5 指回教材；§13.6 不进入 Notes。Exercise 13.9 的可加模型在 §13.1.3 作者解释与本章小结出现。

### 数学、假设与维度

**临界半径。** 星形 $\Rightarrow$ 缩放 $\widetilde h=(\delta/t)h$ 留在类内 $\Rightarrow\mathcal G_n(\delta)/\delta$ 非增 $\Rightarrow$ (13.17) 有最小正解。Exercise 13.5(a)：Cauchy–Schwarz 给出 $\mathcal G_n(\delta)/\delta\le 1$，故 $\delta^2=4\sigma^2$ 总有效。13.5(b)：常数函数 $1$ 给出 $\mathcal G_n(\delta)/\delta\ge\sqrt{2/(\pi n)}$，因而 $\delta^2\ge(8/\pi)\sigma^2/n$。与 Theorem 13.5 注记的 $2/\pi$ 不一致；Notes 与 Solutions 采用习题。

**Theorem 13.5 尺度。** $t=\delta_n$ 时平方误差 $O(\delta_n^2)$。积分尾界 $\mathbb E\|\cdot\|_n^2\le c\{\delta_n^2+\sigma^2/n\}$；含常数函数时 $\delta_n^2$ 主导。Lipschitz 常数 $\sigma u/\sqrt n$ 代入 Theorem 2.26 复现 (13.41)。

**Dudley 推论。** 线性：体积比 $\log N\le r\log(1+2\delta/t)$，积分 $\delta\sqrt{r/n}$，临界 $\delta^2\asymp\sigma^2 r/n$。Lipschitz：$\int t^{-1/2}\,dt\sim\delta^{1/2}$，临界指数 $2/3$。凸：$\int t^{-1/4}\,dt\sim\delta^{3/4}$，临界指数 $4/5$。$\ell_q$：熵 (13.30) 推出 $R_q(\sigma^2\log d/n)^{1-q/2}$。Notes 的自测第 2、3 题与上述计算一致。

**神谕。** $f^*\in\mathcal F$ 时 (13.42b) 退回 Theorem 13.5。Fourier：$M\simeq(n/\sigma^2)^{1/(2\alpha+1)}$ 平衡 $M^{-2\alpha}$ 与 $M/n$，总速率 $(\sigma^2/n)^{2\alpha/(2\alpha+1)}$。稀疏：$\partial\mathcal F_{\mathrm{spar}}(s)\subset\mathcal F_{\mathrm{spar}}(2s)$，并上 $\binom{d}{2s}$ 个子集给出 $s\log(ed/s)/n$。

**KRR。** Lemma 13.22 椭圆交 + Hölder + Jensen 给出 $\sqrt{(2/n)\sum\min\{\delta^2,\widehat\mu_j\}}$。Sobolev：$\sum_{j>k}j^{-2}\lesssim k^{-1}\lesssim\delta^2$ 推出 $\delta_n^{3/2}\simeq\sigma/(R\sqrt n)$；乘 $R^2$ 得 $R^{2/3}(\sigma^2/n)^{2/3}$。高斯核正确地消去 $R^2\cdot(\sigma^2/R^2)$。

**未发明定理。** 极小极大下界指向第 15 章；$L^2(\mathbb P)$ 指向第 14 章；可加模型的完整证明在 Solutions 13.9。$\sqrt{2\log n}$ 型极值只出现在 Solutions 13.6，Notes 未伪造常数。

### 结构、可访问性、链接与渲染

读者栏目：本章导览、学习目标（6 个可观察动词）、必要先修（$L^2(\mathbb P_n)$ / 局部复杂度 / Theorem 2.26）、常见错误、轻量自测（5 题，`<details>` 含「参考答案」）、本章小结、术语对照、来源定位。标题由 `#` 到 `##`，无跳级。Notes 汉语、英文术语首次给出；Solutions 英语。来源定位给出印刷/PDF 页码及 Solutions 相对链接。§13.6 未写入 Notes。

Solutions 题号与印刷页锁定一致：13.1(a)(b)(c)–13.11(a)(b)。
