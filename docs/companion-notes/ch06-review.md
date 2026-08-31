---
chapter_id: "ch06"
chapter_title: "Random matrices and covariance estimation"
map_path: "docs/companion-notes/ch06-content-map.md"
notes_path: "notes/ch06-notes.qmd"
reviewed_at: "2026-08-31"
delivery_status: "Notes 质检通过"
ppt_status: "未请求"
solutions_status: "完成"
---

# 第 6 章审核报告

> 内部工件。本轮按章节独立复核教材原页 PNG（`scratch/ch06/p-178.png`–`p-212.png`）；文本层 `ch06.txt` 只用于定位，公式与定理框以 PNG 为准。

## 范围与结论

- 审核范围：第 6 章内容清单、`notes/ch06-notes.qmd` 与 `solutions/ch06-solutions.qmd`；§6.8 Exercises 6.1–6.16 已按原页锁定，并逐题提供英文独立解答。
- 主教材版本与页码：Martin J. Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series in Statistical and Probabilistic Mathematics No. 48, 2019, ISBN 978-1-108-49802-9；印刷页 159–193，PDF 页 178–212（PDF = 印刷 + 19）。
- 当前结论：三个检查面均通过。Notes 按 §§6.1–6.7 保留教材主线；Solutions 覆盖 Exercises 6.1–6.16，且已按独立重算复核。所有已知来源差异仍标为 `勘误待批`。
- 未关闭问题：清单中 Exercise 6.10 的对称膨胀零块、Ahlswede 拼写、Example 6.25 星图参数、Corollary 6.20 常数吸收及 Theorem 6.17 多余花括号仍待批准；均不阻断当前 Notes。
- 下一步允许动作：可继续保留勘误待批状态；PPT 未请求。

## 独立质检

| 检查面 | 审核者 | 结果 | 简短证据或问题定位 |
|---|---|---|---|
| 内容清单与来源原页 | 独立复核代理（本轮按原页重核） | 通过 | 章首、§§6.1–6.7、Definitions 6.6/6.9/6.10、Lemma 6.11–6.13、Theorem 6.1/6.15/6.17/6.23/6.27、Corollary 6.20/6.24、Examples 6.2–6.4/6.7–6.8/6.14/6.16/6.18–6.22/6.25、Figure 6.1，以及进入 Notes 的 (6.1)–(6.67) 编号式均在清单中逐项或按兼容连续范围登记。Notes 按原节序展开；§6.8 习题不进入 Notes。 |
| 数学、假设与维度 | 独立复核（与写作分离的重算） | 通过 | 原 Notes 的随机矩阵、Lieb 迹界和阈值协方差链条保持闭合。Solutions 逐题重算谱范数、Loewner 序、对称膨胀、矩阵 Bernstein、内在维数、随机 packing 与对角协方差尾界；6.10 的块维数错误只按条件膨胀读法处理。 |
| 结构、可访问性、链接与渲染 | 独立复核 | 通过 | `quarto render solutions/ch06-solutions.qmd` 成功生成 `_site/solutions/ch06-solutions.html`；16 个题号从 6.1 至 6.16 均进入 TOC，公式生成 MathJax 节点。重渲染 Notes 后，章节末链接解析为 `../solutions/ch06-solutions.html`。Notes 的 `zh-CN` 翻译警告为既有配置警告。 |

## 来源差异与勘误

| 定位 | 教材原式/原文 | 差异或纠正版 | 核验证据 | 决定与批准人 |
|---|---|---|---|---|
| Exercise 6.10，印刷页 191；PDF 页 210 | 对称膨胀的零块写成 $0_{d_1\times d_2}$ 与 $0_{d_2\times d_1}$ | 这两个块不能在一般 $d_1\ne d_2$ 时组成方阵；Notes 采用 (6.39) 的两个方阵零块。 | 原页 `p-210.png` 与 (6.39) `p-194.png` 对照，按块维数检查。 | `勘误待批`；未批准 |
| §6.7，印刷页 189；PDF 页 208 | “Alhswede and Winter” | 标准拼写为 Ahlswede–Winter；Notes 标明教材拼写差异。 | 原页 `p-208.png` 与通行人名拼写核对。 | `勘误待批`；未批准 |
| Example 6.25 / Figure 6.1，印刷页 182；PDF 页 201 | 星–辐图文字称连接 $s$ 个结点，但印刷式给 $\lVert A\rVert_2=1+\sqrt{s-1}$ | Notes 保留印刷式，同时解释辐条数为 $k$ 时为 $1+\sqrt{k}$，因此只作 $\sqrt s$ 量级比较。 | 原页 `p-201.png`；直接计算星图谱半径。 | `勘误待批`；未批准 |
| Corollary 6.20 证明，印刷页 179；PDF 页 198 | 证明得到 $\lVert Q_i\rVert\le2b$，但 (6.49) 直接使用较紧分母 | Notes 保留教材 (6.49)，并明确指出机械代入 $b'=2b$ 会改变线性项常数。 | 原页 `p-198.png`；从 (6.42) 代入参数独立复核。 | `勘误待批`；未批准 |
| Theorem 6.17，印刷页 176；PDF 页 195 | “$\{Q_i\}_{i=1}^n\}$” 多一个右花括号 | 仅排印问题，不改教材；Notes 未复制该排印错误。 | 原页 `p-195.png`。 | `勘误待批`；未批准 |

## 派生产物

| 产物 | 请求范围 | 状态 | 自身检查证据或受阻原因 |
|---|---|---|---|
| PPT | 未请求 | 未请求 | 用户未请求 PPT。 |
| Solutions | Exercises 6.1–6.16 的完整英文解答 | 完成 | `solutions/ch06-solutions.qmd` 含 16 个逐题 heading、abridged stem 与独立 Solution callout；HTML 已生成。6.10 的对称膨胀维数问题保留为 `勘误待批`。 |

## 核对摘记

### 内容清单与来源原页

- `p-178`–`p-184` 核对奇异值 / Rayleigh–Ritz、协方差设定、(6.6)–(6.7)、Theorem 6.1、(6.8)–(6.17) 和迹约束；Notes 逐项保留球面一致定律、有效维数及高斯比较的必要假设。
- `p-184`–`p-187` 核对行向次高斯定义、Theorem 6.5、(6.19a)–(6.23) 与 $1/8$-覆盖证明；Notes 明确交代 $17^d$ 如何进入 $4d$，并将次高斯协方差的常数与高斯情形区分。
- `p-187`–`p-199` 核对函数演算、矩阵 MGF、Lieb 独立和、Theorems 6.15/6.17、非对称膨胀、Corollary 6.20 及 Examples 6.16/6.18–6.22；Notes 保留必要的方差矩阵、秩因子和非交换性说明。
- `p-199`–`p-207` 核对硬阈值、Theorem 6.23、(6.54)–(6.56)、Example 6.25、$\ell_q$ 稀疏 Theorem 6.27 及 Gordon 附录骨架；习题 `p-208`–`p-212` 的 Exercises 6.1–6.16 全部在 map 中登记为 `不进入 Notes`。

### 数学、假设与维度

- Theorem 6.1：$X=W\sqrt\Sigma$ 后，最大奇异值映射的 Gaussian Lipschitz 常数至多 $\gamma_{\max}(\sqrt\Sigma)/\sqrt n$；比较过程给出 $\mathbb E\sigma_{\max}(X)\le\sqrt n\,\gamma_{\max}(\sqrt\Sigma)+\sqrt{\mathrm{tr}(\Sigma)}$，再与集中合成 (6.8)。标准高斯的 (6.11) 和共轭不等式正确推出 (6.12)。
- Theorem 6.5：$v=v^j+\Delta$ 时交叉项与二次项合计不超过 $\frac12\lVert Q\rVert_{\mathrm{op}}$，所以网格上界带因子 2；$2N\le e^{4d}$ 给出 MGF 中的 $4d$。固定方向的中心化平方变量用 (6.23) 与四阶矩级数，参数域与 (6.19a) 相符。
- 矩阵尾界：$e^{\lambda Q}$ 正定，所以最大特征值不超过迹；独立矩阵不能把 MGF 写成矩阵乘积，Lieb 凹性给出 (6.36)。对数单调性、方差尺度、秩前因子和对称膨胀的维数均按原式使用。
- 协方差与阈值：$Q_i=x_ix_i^T-\Sigma$ 的方差满足 $\mathrm{var}(Q_i)\preceq b\Sigma$；(6.54) 先给逐元误差再用非负矩阵的谱范数单调性，(6.55) 由 $\lVert A\rVert_{\mathrm{op}}\le s$ 得出；行 $\ell_q$ 的大 / 小坐标拆分给出 $4R_q\lambda_n^{1-q}$。
- Gordon 附录只保留证明骨架，没有把比较不等式冒充教材正文新定理；正定性与 $n\ge d$ 的边界在 Notes 中有明确说明。

### 结构、可访问性与渲染

实际生成的 HTML 包含定理 callout、公式、折叠式自测答案、术语表和中文正文。Notes 没有复制作图文件，Figure 6.1 采用文字说明并给出来源定位，因此不存在缺少图片替代文本的问题。项目级 `_quarto.yml` / 首页仍有导航不同步的既有事项，不影响本章文件本身放行。
