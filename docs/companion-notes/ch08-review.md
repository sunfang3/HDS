---
chapter_id: "ch08"
chapter_title: "Principal component analysis in high dimensions"
map_path: "docs/companion-notes/ch08-content-map.md"
notes_path: "notes/ch08-notes.qmd"
reviewed_at: "2026-08-31"
delivery_status: "Notes 质检通过"
ppt_status: "未请求"
solutions_status: "完成"
---

# 第 8 章审核报告

> 内部工件。对照印刷页 PNG（`scratch/ch08/p-255.png`–`p-277.png`）核验，不采用文本层为权威。`ch08.txt` 仅作索引：Toeplitz 条目丢掉了 $\sqrt{|j-k|}$，(8.7) 的平方与迹恒等式冲突，均以 PNG 为准。

## 范围与结论

- 审核范围：第 8 章内容清单、`notes/ch08-notes.qmd`、§8.5 Exercises 8.1–8.9 的独立解答（`solutions/ch08-solutions.qmd`）
- 主教材版本与页码：Martin J. Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series in Statistical and Probabilistic Mathematics No. 48, 2019, ISBN 978-1-108-49802-9；印刷页 236–258，PDF 页 255–277（PDF = 印刷 + 19）
- 当前结论：三个检查面均通过。Notes 按节序转写主线（PCA / Weyl / Theorem 8.5 / 尖刺 / 稀疏 PCA），习题 8.1–8.9 全部锁定并独立求解。六处教材笔误嫌疑保持 `勘误待批`，未写成已批准勘误。
- 未关闭问题：见下方勘误表。(8.7) 的平方、Corollary 8.7 证明里 $\phi$ 的自变量、Lemma 8.6 证明的 $\Psi$ 符号、Corollary 8.12 证明与 (8.25b) 的半径、Exercise 8.2 的 Frobenium、Exercise 8.6 的 $1++\sigma^2$。
- 下一步允许动作：勘误待教师批准；新词由父代理合并进 `glossary.qmd`。

## 独立质检

| 检查面 | 审核者 | 结果 | 简短证据或问题定位 |
|---|---|---|---|
| 内容清单与来源原页 | 本章作者对照印刷页 PNG | 通过 | (8.1)–(8.43)、Theorem 8.5 / 8.10、Corollary 8.7 / 8.12、Lemma 8.6 / 8.8 / 8.11 / 8.13 / 8.14、Example 8.1–8.4 / 8.9、Figure 8.1–8.5、Exercises 8.1–8.9 均已入清单。Notes 按 §§8.1–8.4 转写；§8.5 不进 Notes。 |
| 数学、假设与维度 | 本章作者对照印刷页 PNG | 通过 | Weyl 只控制特征值；Theorem 8.5 在算子范数等于间隙一半的对角反例处唯一性失败；(8.20) 与 (8.32) 的标度分别为 $\sqrt{d/n}$ 与 $\sqrt{s\log d/n}$。未把 (8.7) 的平方写成已证恒等式。 |
| 结构、可访问性、链接与渲染 | 本章作者对照印刷页 PNG | 通过 | 七个读者栏目齐全；标题无跳级；Notes 汉语 / Solutions 英语；来源定位链到 `../solutions/ch08-solutions.qmd`。自测 `<details>` 含「参考答案」。 |

## 派生产物

| 产物 | 请求范围 | 状态 | 自身检查证据或受阻原因 |
|---|---|---|---|
| PPT | 未请求 | 未请求 | 用户未请求 PPT。 |
| Solutions | 全部习题（§8.5 Exercises 8.1–8.9） | 完成 | 题号由印刷页 256–258 PNG 锁定。8.1 Courant–Fischer；8.2 酉不变范数（(iv) 反例、对称规范函数）；8.3 Weyl；8.4 前 $r$ 个特征向量及正确重构 $\sum_{j>r}\gamma_j$；8.5 幂法；8.6 混合模型换元 $\nu=1/\sigma^2$；8.7 $Z=yxx^T$；8.8–8.9 SDP 与原–对偶见证。 |

## 核对摘记

### 内容清单与来源原页

对照 `p-255.png`–`p-277.png` 逐条核对编号公式（OCR 不可信）：

- (8.1)–(8.3) 印刷页 236–237：总体 / 经验第一主成分。Notes 一致。
- (8.4)–(8.6) 印刷页 237：Eckart–Young–Mirsky 与 Frobenius 误差 $\sum_{j>r}\gamma_j^2(\Sigma)$。Notes 一致。Toeplitz 条目 PNG 为 $T_{jk}=e^{-\alpha\sqrt{|j-k|}}$（$\alpha=0.95$）；文本层丢掉根号，Notes 跟 PNG。
- (8.7) 印刷页 239：原页确有 $\sum_{j>r}\gamma_j^2(\Sigma)$。Notes 保留原文并标勘误待批；正确重构是 $\mathrm{tr}((I-\Pi)\Sigma)=\sum_{j>r}\gamma_j(\Sigma)$。
- (8.8) 与 $\Gamma=\theta^*\otimes\theta^*+\sigma^2 I_d$ 印刷页 240。Yale：$d=243\times 320=77760$，$n=165$。Notes 一致。
- (8.9)–(8.10) 印刷页 241：Weyl 与 $Q_\varepsilon$。$v_0=[0,1]^T$，$\varepsilon=0.01$ 时 $v_\varepsilon\approx[0.53,0.85]^T$。Notes 一致。
- (8.11)–(8.17) 印刷页 242–244：块分解、Theorem 8.5、Lemma 8.6、$\|\widehat\Delta\|_2=\sqrt{2(1-\varrho)}$。Notes 一致。
- (8.18)–(8.24) 印刷页 245–247：尖刺模型、Corollary 8.7、三项分解、Lemma 8.8。概率指数为 $n\min\{\sqrt{\nu}\,\delta,\nu\delta^2\}$。Notes 一致。
- (8.25a)–(8.31) 印刷页 249–251：SCOTLASS / 惩罚、一致偏差 (8.26)、Theorem 8.10（$c_0<1/6$）、锥 (8.31)。Notes 一致。
- (8.32)–(8.40) 印刷页 252–254：Corollary 8.12 把 $d$ 换成 $s\log d$；(8.33) 中 $c_0=1/8$。Notes 一致。
- (8.41)–(8.43) 印刷页 256–258：习题公式。Solutions 按 PNG 锁定。

§8.4 文献清单按地图指回教材。Figure 8.1–8.5 均入清单并在 Notes 中简要说明。

### 数学、假设与维度

**Weyl 对 Example 8.4。** $a=1.01$，特征值移动 $\frac12\bigl|(a-1)-\sqrt{(a-1)^2+4\varepsilon^2}\bigr|\le\varepsilon$，与 $\|P\|_{\mathrm{op}}=1$ 一致。特征向量移动不是 $O(\varepsilon)$。

**Theorem 8.5 的边界。** $\Sigma=\mathrm{diag}\{2,1\}$、$P=\mathrm{diag}\{-1/2,+1/2\}$ 给出 $\widehat\Sigma=\frac32 I_2$，此时 $\|P\|_{\mathrm{op}}=\nu/2$。Notes 未把严格不等式写成闭区间。

**(8.12) 的最后一步。** 由 $\sqrt{1-\varrho^2}\le 2\varrho\|\tilde p\|_2/(\nu-2\|P\|_{\mathrm{op}})$ 与 $\|\widehat\Delta\|_2=\sqrt{2(1-\varrho)}$，预因子 $\sqrt{2}\varrho/\sqrt{1+\varrho}\le 1$ 当且仅当 $2\varrho^2\le 1+\varrho$（$\varrho\in[0,1]$）。与原页一致。

**尖刺换元（Exercise 8.6）。** $\Gamma=\theta^*\theta^{*T}+\sigma^2 I_d$ 在 $\alpha=0.5$ 时成立。令 $\widetilde x=X/\sigma$，则 $\nu=1/\sigma^2$，Corollary 8.7 的前置 $\sqrt{(\nu+1)/\nu^2}\sqrt{d/n}=\sigma\sqrt{1+\sigma^2}\sqrt{d/n}\le 1/128$ 即 $n\gtrsim\sigma^2(1+\sigma^2)d$。误差同型。Solutions 按 $1+\sigma^2$ 读 $1++\sigma^2$。

**稀疏标度。** (8.26) 在锥 $\|\Delta\|_1\le 4\sqrt{s}\|\Delta\|_2$ 上把 $\varphi_\nu\|\Delta\|_1$ 变成 $\sqrt{s}\,\varphi_\nu\|\Delta\|_2$，除以 $\nu$ 即 (8.27)。Corollary 8.12 的 $\varphi_\nu\asymp\sqrt{(\nu+1)\log d/n}$ 给出 (8.32)。$s=\lfloor 0.25d\rfloor$ 并不自动让 $s\log d/n$ 变小；Notes 自测第 5 题钉住这一点。

**未发明定理。** Lemma 8.8 / 8.13 的证明留作第 2、6 章练习；Lemma 8.14 的子矩阵并指回教材。极小极大下界指向 Example 15.19。Davis–Kahan 名称标了「作者解释」。

### 结构、可访问性、链接与渲染

读者栏目：本章导览、学习目标（5 个可观察动词）、必要先修（特征间隙 / 算子范数 / 符号不定性）、常见错误、轻量自测（5 题，`<details>` 含「参考答案」）、本章小结、术语对照、来源定位。标题由 `#` 到 `##` 到 `###`，无跳级。Notes 汉语、英文术语首次给出；Solutions 英语。未把习题解写入 Notes。

`validate_chapter.rb --stage map` 与 `--stage notes` 均为零退出（结构合法，不说明数学正确）。

## 勘误待批

| 定位 | 原文 | 问题 | 处置 |
|---|---|---|---|
| (8.7) 印刷页 239 | $\mathbb E\|X-\Pi_{\mathbb V^*}(X)\|_2^2=\sum_{j>r}\gamma_j^2(\Sigma)$ | 向量重构应为 $\sum_{j>r}\gamma_j(\Sigma)$；平方属于 (8.6) | 保留原文；Notes / Exercise 8.4 标明 |
| Corollary 8.7 证明 印刷页 247 | $\phi(1/4,\delta/(3\sqrt{\nu}),\delta/16)$ | 刚选定的是 $(1/16,\,\delta/(4\sqrt{\nu}),\,\delta/16)$ | 按选定的 $\delta_i$ 读 |
| Lemma 8.6 证明 印刷页 243 | 右端等于 $-\Psi$ | 按 (8.13) 展开应等于 $\Psi$；绝对值挽救引理 | 按定义展开 |
| Corollary 8.12 证明 印刷页 253 | $\|\theta^*\|_1\le\nu\sqrt{n/\log d}$ | (8.25b) 写 $(n/\log d)^{1/4}$ | 各处原文并记；标度仍成立 |
| Exercise 8.2(a)(i) 印刷页 256 | Frobenium | 标准名为 Frobenius | Solutions 按 Frobenius |
| Exercise 8.6(a) 印刷页 257 | $1++\sigma^2$ | 应为 $1+\sigma^2$ | Solutions 按 $1+\sigma^2$ |

非阻断：Figure 8.2(c) 图注写“前 25 张特征脸”，正文写平均脸加上前 24 张主成分——25 张图的左上角是平均脸。Notes 跟正文。
