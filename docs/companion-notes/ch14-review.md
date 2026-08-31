---
chapter_id: "ch14"
chapter_title: "Localization and uniform laws"
map_path: "docs/companion-notes/ch14-content-map.md"
notes_path: "notes/ch14-notes.qmd"
reviewed_at: "2026-08-31"
delivery_status: "Notes 质检通过"
ppt_status: "未请求"
solutions_status: "完成"
---

# 第 14 章审核报告

> 内部工件。对照印刷页 PNG（`scratch/ch14/p-472.png`–`p-503.png`）独立核验。文本层 `ch14.txt` 仅作索引；公式、定理框、习题题干以 PNG 为准。

## 范围与结论

- 审核范围：第 14 章内容清单、`notes/ch14-notes.qmd`、§14.7 Exercises 14.1–14.11 的独立解答（`solutions/ch14-solutions.qmd`）
- 主教材版本与页码：Martin J. Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series in Statistical and Probabilistic Mathematics No. 48, 2019, ISBN 978-1-108-49802-9；印刷页 453–484，PDF 页 472–503（PDF = 印刷 + 19）
- 当前结论：三个检查面均通过；Notes 可交付。清单原有八处加 Exercise 14.5(c) 一处笔误嫌疑保持 `勘误待批`。习题 14.1–14.11 已从 PNG 锁定并独立求解。
- 未关闭问题：见下方勘误表（均未写成已批准勘误）。
- 下一步允许动作：勘误待教师批准；术语新词可由父代理合并进 `glossary.qmd`。

## 独立质检

| 检查面 | 审核者 | 结果 | 简短证据或问题定位 |
|---|---|---|---|
| 内容清单与来源原页 | 对照印刷页 PNG 的章作者核验 | 通过 | (14.1)–(14.69) 及 Theorems 14.1、14.12、14.20，Corollaries 14.3、14.5、14.15、14.22、14.24，Lemma 14.8–14.9、14.21，Proposition 14.25，Figures 14.1–14.2，Exercises 14.1–14.11 均已入清单；Notes 按节序转写，证明节为简要说明。关键式与原页一致，见下。 |
| 数学、假设与维度 | 对照印刷页 PNG 的章作者核验 | 通过 | 临界不等式量纲与 Example 14.2 / 14.6 / 14.7 的速率一致；单边定律的四阶矩与锥状注记足以覆盖线性类；Corollary 14.15 的 Case 1 按平方经验范数解读后与 Theorem 13.5、14.12 相加。未发现 Notes 虚构定理。 |
| 结构、可访问性、链接与渲染 | 对照印刷页 PNG 的章作者核验 | 通过 | 七个读者栏目齐全；标题无跳级；Notes 汉语 / Solutions 英语；来源定位链到 `../solutions/ch14-solutions.qmd`。无 样章读者门。 |

## 派生产物

| 产物 | 请求范围 | 状态 | 自身检查证据或受阻原因 |
|---|---|---|---|
| PPT | 未请求 | 未请求 | 用户未请求 PPT。 |
| Solutions | 全部习题（§14.7 Exercises 14.1–14.11） | 完成 | 题号从 `p-501.png`–`p-503.png` 锁定（文本层可能漏 14.1）；独立求解。14.4 按 $\sum\theta_j^2\le\delta^2$、14.5(c) 按 $1/\sqrt{\mu_j}$、14.6 按 $C^2=B+6$ 处理并标明原文。 |

## 核对摘记

### 内容清单与来源原页

对照 `p-472.png`–`p-503.png` 逐条核对编号公式（OCR 不可信）：

- (14.1)–(14.2) 印刷页 453：总体 / 经验 $L^2$ 范数。Notes 一致。
- 霍夫丁尾 印刷页 454：$2\exp(-nt^2/(2b^4))$。Notes 跟原页（比区间霍夫丁的 $2\exp(-2nt^2/b^4)$ 更松）。
- (14.3)–(14.8)、Theorem 14.1 印刷页 454–455：局部总体 / 经验拉德马赫，临界 $\overline{\mathcal R}_n(\delta)\le\delta^2/b$，平方偏差 (14.5a) 含 $t^2/2$，范数偏差 (14.5b) 含 $n\delta_n^2\ge(2/c_2)\log(4\log(1/\delta_n))$。Notes 一致。
- (14.9)–(14.12)、Example 14.2 印刷页 455–457：VC 界 (14.10) 无局部化；(14.11) 原页为 $\tfrac12\|f\|_2^2+t^2$（不是 $t^2/2$）；勒让德基给出 $\delta_n=c/\sqrt n$ 与 (14.12) 的 $t^2/2$。Notes 分别按各显示式转写。
- Corollary 14.3 / (14.13) 印刷页 457：积分下限 $\delta^2/(2b)$，系数 $64/\sqrt n$，右端 $\delta^2/b$。Notes 跟 PNG，不跟文本层可能出现的 $\delta^2 b^2$。
- Example 14.4 印刷页 457–458：$\log N_{\mathrm{sup}}\lesssim t^{-1/2}$，$\int_0^\delta t^{-1/4}\,dt=(4/3)\delta^{3/4}/\sqrt n$，故 $\delta_n\asymp n^{-2/5}$。
- Corollary 14.5 / (14.14) 印刷页 458：$\sqrt{2/n}\sqrt{\sum\min\{\mu_j,\delta^2\}}$；经验核矩阵 $K_{ij}=\mathcal K(x_i,x_j)/n$。
- Example 14.6–14.7 印刷页 459：$\mu_j=(2/((2j-1)\pi))^2$，$\delta_n=cn^{-1/3}$；高斯核 $\mu_j\le c_0 e^{-c_1 j\log j}$，$\delta_n=c_0\sqrt{\log(n+1)/n}$。
- Lemma 14.8–14.9、(14.15)–(14.20) 印刷页 460–462：重标度临界 $\delta^2/16$；剥皮 $M\le 4\log(1/\delta_n)$。Notes 为简要说明。
- (14.21)–(14.25)、Theorem 14.12 印刷页 462–464：弱 / 强四阶矩；临界 $\overline{\mathcal R}_n(\delta)/\delta\le\delta/(128C)$；下界 $\tfrac12\|f\|_2^2$。
- Example 14.13–14.14、(14.26)–(14.31) 印刷页 465–466：线性类与可加模型。两处原文笔误按清单解读，Notes 用作者解释标明，未写成已批准勘误。
- Corollary 14.15 / (14.32)–(14.33) 印刷页 466–467：总体误差 $c_0(\varepsilon_n^2+\delta_n^2)$。Case 1 原页 $\lvert\widehat f-f^*\rvert_n\ge 16\delta_n^2$ 按平方范数读。
- (14.34)–(14.38) 印刷页 468–469：截断 $\tau^2=4C^2$。简要说明。
- (14.39)–(14.53)、Theorem 14.20 印刷页 469–473：Lipschitz / 强凸；超额风险无强凸时 $O(\delta_n)$、有强凸时 $O(\delta_n^2)$。Huber (14.44) 保留原文并给出标准定义。证明页 474 的 $10L/\gamma$ 按带 $\delta_n$ 的 (14.52a) 读。
- (14.56)–(14.65)、Corollary 14.22 / 14.24 印刷页 475–479：NPMLE 海林格界；投影神谕不等式。Figures 14.1–14.2 仅作简要说明，未插入图片。
- Proposition 14.25 / (14.66)–(14.68) 印刷页 480–481：$\delta_n/4\le\hat\delta_n\le 3\delta_n$。
- §14.6 指回教材；§14.7 不进 Notes。
- Exercises 14.1–14.11 印刷页 482–484：14.1 仅出现在 PNG（文本层从文献段落下半页开始）。题号锁定为 14.1–14.11。

### 数学、假设与维度

**Example 14.2 的两种速率。** 无局部化时 $\overline{\mathcal R}_n(\delta)\lesssim\sqrt{\log n/n}$ 与 $\delta$ 无关，解 $\delta^2\gtrsim n^{-1/2}$ 得 $n^{-1/4}$。勒让德参数化后 $\overline{\mathcal R}_n(\delta)\lesssim\delta/\sqrt n$，解得 $n^{-1/2}$。Notes 的自测第 1 题与此一致。原页在 (14.12) 前写 Theorem 4.10，Notes 按 Theorem 14.1 解读。

**RKHS 临界半径。** $\mu_j\asymp j^{-2}$ 时 $\sum\min\{\mu_j,\delta^2\}\asymp\delta$，故 $\overline{\mathcal R}_n\lesssim\sqrt{\delta/n}$，令其 $\le\delta^2$ 得 $\delta_n\asymp n^{-1/3}$（Example 14.6）。超指数衰减给出 $\sqrt{\log n/n}$（Example 14.7）。量纲正确。

**单边定律与线性类。** 高斯四阶矩 $C^2=3$ 与 $\lambda_{\max}(\Sigma)$ 无关；$x=\sqrt{\Sigma}w$、$w\sim N(0,I_d)$ 时 $\overline{\mathcal R}_n(\delta)\le\delta\sqrt{d/n}$，故 $\delta_n^2\lesssim d/n$。原页写 $w\sim N(0,\Sigma)$ 会破坏“$\varepsilon_i w_i$ 标准高斯”与 $\mathbb E\|n^{-1}\sum\varepsilon_i w_i\|_2\le\sqrt{d/n}$。Notes 标明按 $I_d$ 读。

**Corollary 14.15 Case 1。** Theorem 13.5 控制的是平方经验误差 $\lVert\widehat f-f^*\rVert_n^2\ge 16 t\delta_n$；取 $t=\delta_n$ 得 $16\delta_n^2$。原页丢掉平方后无法与 $2\lVert\cdot\rVert_n^2$ 相加得到总体平方误差。Notes 按平方解读。

**Theorem 14.20(b)。** $(\gamma/2)r^2\le 10L\delta_n r$ 推出 $r\le 20L\delta_n/\gamma$，与 (14.52a) 的 $(20L/\gamma+1)\delta_n$ 一致。证明正文漏 $\delta_n$。

**Huber (14.44)。** 原文 $\tau u-\tau^2/2$ 在 $u<-\tau$ 无下界，且与后文 $\|\Psi'\|_\infty\le\tau$ 矛盾。Notes 给出标准 $\tau\lvert u\rvert-\tau^2/2$，未标成已批准勘误。

**未发明定理。** Dudley 积分、Ledoux–Talagrand、Talagrand 集中、Lemma 13.6、Theorem 13.5 / 13.13、Corollary 12.26、Theorem 7.16 均指向既有编号结果。作者解释只用于星形单调性、两种 $L^2$ 范数的差别、以及上述原文与后文不一致处。

**习题独立性。** 14.1 用压缩 + Jensen 得到印刷常数 $\sqrt 5$；14.2 用 Lemma 13.6；14.4 按 $\delta^2$ 约束才能得到椭圆常数 2；14.8 对称分配 $\delta_j=\delta/\sqrt d$ 给出 $\delta_n^2\lesssim d\varepsilon_n^2$；14.10 用 $-\log t\ge 1-t$ 于 $\sqrt{g/f}$ 得到 $D\ge 2H^2$；14.11 平衡 $T^{-2}+T/n$ 得 $n^{-2/3}$。

### 结构、可访问性、链接与渲染

读者栏目：本章导览、学习目标（5 个可观察动词，落在 3–7）、必要先修（局部化 / 星形 / 两种 $L^2$ 范数）、常见错误、轻量自测（5 题，`<details>` 含「参考答案」）、本章小结、术语对照、来源定位。标题由 `#` 到 `##` 到 `### 例`，无跳级。Notes 汉语、英文术语首次给出；Solutions 英语。来源定位给出印刷 / PDF 页码及 Solutions 相对链接。证明节按清单为简要说明；习题解不进 Notes。未改 `glossary.qmd` / `_quarto.yml` / `index.qmd` / 其他章。

## 勘误待批（保留原文，未写成已批准）

| 定位 | 原文 | 拟读法 | 状态 |
|---|---|---|---|
| Example 14.2 印刷页 457 | Applying Theorem 4.10 then guarantees (14.12) | 按 Theorem 14.1 的 (14.5a) | 勘误待批 |
| Example 14.13 印刷页 465 | $w\sim\mathcal N(0,\Sigma)$ | $w\sim\mathcal N(0,I_d)$ | 勘误待批 |
| Example 14.14 印刷页 466 | $\overline{\mathcal R}_n(\varepsilon;\mathscr F)\lesssim\varepsilon^2$ | $\overline{\mathcal R}_n(\varepsilon;\mathscr G)$ | 勘误待批 |
| Example 14.17 / (14.44) 印刷页 471 | Huber 在 $\lvert u\rvert>\tau$ 为 $\tau u-\tau^2/2$ | $\tau\lvert u\rvert-\tau^2/2$ | 勘误待批 |
| Corollary 14.15 Case 1 印刷页 467 | $\lVert\widehat f-f^*\rVert_n\ge 16\delta_n^2$ | $\lVert\widehat f-f^*\rVert_n^2\ge 16\delta_n^2$ | 勘误待批 |
| Theorem 14.20 证明 印刷页 474 | $\lVert\widehat f-f^*\rVert_2\le 10L/\gamma$ | $r\le 20L\delta_n/\gamma$，与 (14.52a) 一致 | 勘误待批 |
| Exercise 14.4(a) 印刷页 483 | $\sum\theta_j^2\le\delta$ | $\sum\theta_j^2\le\delta^2$ | 勘误待批 |
| Exercise 14.5(c) 印刷页 483 | 分母 $\mu_j$ | 分母 $\sqrt{\mu_j}$（$\lVert\phi_j\rVert_{\mathbb H}=1/\sqrt{\mu_j}$） | 勘误待批 |
| Exercise 14.6 印刷页 483 | (14.22b) with $C=B+6$ | $C^2=B+6$ | 勘误待批 |
