---
chapter_id: "ch04"
chapter_title: "Uniform laws of large numbers"
map_path: "docs/companion-notes/ch04-content-map.md"
notes_path: "notes/ch04-notes.qmd"
reviewed_at: "2026-08-31"
delivery_status: "Notes 质检通过"
ppt_status: "未请求"
solutions_status: "完成"
---

# 第 4 章审核报告

> 内部工件。本轮按章节独立复核教材原页 PNG（`scratch/ch04/p-117.png`–`p-139.png`）；文本层 `ch04.txt` 只用于定位，公式与定理框以 PNG 为准。

## 范围与结论

- 审核范围：第 4 章内容清单、`notes/ch04-notes.qmd` 与 `solutions/ch04-solutions.qmd`；§4.5 Exercises 4.1–4.17 已按原页锁定，并逐题提供英文独立解答。
- 主教材版本与页码：Martin J. Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series in Statistical and Probabilistic Mathematics No. 48, 2019, ISBN 978-1-108-49802-9；印刷页 98–120，PDF 页 117–139（PDF = 印刷 + 19）。
- 当前结论：三个检查面均通过。Notes 保留章首至 §§4.1–4.4 的顺序；Solutions 覆盖 Exercises 4.1–4.17，且已按独立重算复核。习题整节不进入 Notes；已知来源差异仍标为 `勘误待批`，没有把待批读法伪装成教材改正。
- 未关闭问题：清单中 (4.24)、Example 4.22、Example 4.17 以及习题页的 Bernoulli / `h_s` 记号差异仍待批准；这些问题不阻断当前 Notes。
- 下一步允许动作：可继续保留勘误待批状态；PPT 未请求。

## 独立质检

| 检查面 | 审核者 | 结果 | 简短证据或问题定位 |
|---|---|---|---|
| 内容清单与来源原页 | 独立复核代理（本轮按原页重核） | 通过 | 章首、§§4.1–4.4、Definition 4.5/4.13/4.16、Proposition 4.11/4.12/4.18/4.19/4.20、Lemma 4.14、Theorem 4.4/4.10、Corollary 4.15、Examples 4.1–4.3/4.6–4.9/4.17/4.21/4.22，以及 (4.1)–(4.31) 中进入 Notes 的编号式均在清单中逐项或按兼容连续范围登记。Notes 按原节序展开；§4.5 习题不进入 Notes。 |
| 数学、假设与维度 | 独立复核（与写作分离的重算） | 通过 | 原 Notes 的经验 CDF、ERM、对称化、Sauer--Shelah 等链条保持闭合。Solutions 逐题重算了泛函连续性、Rademacher 操作、VC 计数与几何构造、指数族风险及正弦类打散；4.14 与 4.16 的上界论证已在复核中修订。4.3 和 4.14 的原书疑点只按条件读法使用。 |
| 结构、可访问性、链接与渲染 | 独立复核 | 通过 | `quarto render solutions/ch04-solutions.qmd` 成功生成 `_site/solutions/ch04-solutions.html`；17 个题号从 4.1 至 4.17 均进入 TOC，公式生成 MathJax 节点。重渲染 Notes 后，章节末链接解析为 `../solutions/ch04-solutions.html`。Notes 的 `zh-CN` 翻译警告为既有配置警告。 |

## 来源差异与勘误

| 定位 | 教材原式/原文 | 差异或纠正版 | 核验证据 | 决定与批准人 |
|---|---|---|---|---|
| (4.24)，印刷页 110；PDF 页 129 | $mathcal R_n(\mathscr F)\le 2b\sqrt{\nu\log(n+1)/n}$ | Lemma 4.14 在 $D\le b$ 时给出 $4b$；Corollary 4.15 的 $8$ 也按 $4b$ 推出。Notes 保留印刷式并明确指出不一致。 | 原页 `p-129.png`；与 Lemma 4.14、(4.25) 逐式比较。 | `勘误待批`；未批准 |
| Example 4.22，印刷页 116；PDF 页 135 | 先写 $c\in\mathbb R^{d+1}$，但特征映射和维数为 $d+2$ | Notes 按同段的 $c\in\mathbb R^{d+2}$ 讲解，并保留教材差异说明。 | 原页 `p-135.png`；$\phi:\mathbb R^d\to\mathbb R^{d+2}$ 与正文相互核对。 | `勘误待批`；未批准 |
| Example 4.22 / Exercise 4.13，印刷页 116、120；PDF 页 135、139 | 把 $\{x:\lVert x-a\rVert_2\le b\}$ 称为 sphere | Notes 说明数学上这是闭球，未把教材用词写成已批准勘误。 | 原页 `p-135.png`、`p-139.png`。 | `勘误待批`；未批准 |
| Exercise 4.3(a)(i)，印刷页 118；PDF 页 137 | Bernoulli 质量函数分母写为 $1+e^{\theta x}$ | Notes 不含题解；清单记录指数族应为 $1+e^\theta$，待教师批准后方可用于 Solutions。 | 原页 `p-137.png`；在 $x\in\{0,1\}$ 上直接检验归一性。 | `勘误待批`；未批准 |
| Example 4.17 / Exercise 4.14，印刷页 112、120；PDF 页 131、139 | 左端点写法由 $(b,a]$ 变为 $(-b,a]$；函数下标出现 $h_s$ | Notes 仅采用不影响计数和定义的统一读法；Solutions 未请求。 | 原页 `p-131.png`、`p-139.png`。 | `勘误待批`；未批准 |

## 派生产物

| 产物 | 请求范围 | 状态 | 自身检查证据或受阻原因 |
|---|---|---|---|
| PPT | 未请求 | 未请求 | 用户未请求 PPT。 |
| Solutions | Exercises 4.1–4.17 的完整英文解答 | 完成 | `solutions/ch04-solutions.qmd` 含 17 个逐题 heading、abridged stem 与独立 Solution callout；HTML 已生成。4.3 的 Bernoulli 分母和 4.14 的下标差异保留为 `勘误待批`。 |

## 核对摘记

### 内容清单与来源原页

- `p-117`–`p-120` 核对了经验 CDF、插入泛函、分位数、拟合优度、一般函数类、有限子集反例和 ERM 设定；Notes 的 (4.1)–(4.10) 与原页一致，且明确区分逐点收敛与一致收敛。
- `p-123`–`p-128` 核对了限制集、经验/总体拉德马赫复杂度、Theorem 4.10、对称化与必要性命题；Notes 对 (4.11)–(4.22) 的处理保持原顺序，并将无界代价的适用边界标出。
- `p-129`–`p-135` 核对了多项式判别、Lemma 4.14、(4.24)–(4.31)、VC 打散、Sauer–Shelah、有限维子图类及两个几何例子；Notes 对 (4.24) 和 Example 4.22 的疑点均显式保留。
- 习题页 `p-136`–`p-139` 的 Exercises 4.1–4.17 全部在 map 中逐题登记为 `不进入 Notes`，没有把正式习题内容误当作正文遗漏。

### 数学、假设与维度

- Theorem 4.10：改一个坐标的 Lipschitz 常数是 $2b/n$，故 McDiarmid 给出 $\exp(-nt^2/(2b^2))$；独立副本对称化后拆成两项，得到 $2\mathcal R_n$。Notes 的推导链保留了这两个来源。
- Proposition 4.11/4.12：上界使用原函数类，下界使用中心化类；$\sup_f|\mathbb E f|/(2\sqrt n)$ 在一致有界假设下为可消失项。Notes 没有把必要性写成无条件的精确等价。
- Lemma 4.14 与 Corollary 4.15：样本限制集至多 $n+1$ 个取值，$D\le1$，因此经验复杂度为 $4\sqrt{\log(n+1)/n}$，再乘 Theorem 4.10 的 2 得 (4.25) 的 8；这也确认了 (4.24) 的待批常数差异。
- VC 部分：Sauer–Shelah 的递归按是否包含最后一点拆分；零水平子图的线性依赖关系确实给出有限维上界。Example 4.22 的特征映射有 $d+2$ 个坐标，Notes 以此作为待批差异的安全读法。

### 结构、可访问性与渲染

实际生成的 HTML 包含定理 callout、公式、折叠式自测答案、表格标题行和中文正文。Notes 不复制作图文件，只对 Figure 4.1 作有定位的文字说明，因此没有缺少图片替代文本的问题。项目级 `_quarto.yml` / 首页仍存在导航不同步的既有事项，不影响本章文件本身放行。
