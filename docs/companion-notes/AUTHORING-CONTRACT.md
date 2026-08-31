# HDS Companion 读者合同（后续章复用）

面向已学陈希孺《概率论与数理统计》的读者。不要重写教材，补齐高维非渐近语言（尾界 / 测度集中 / 一致大数定律 / 度量熵 / 随机矩阵）以及低维结构（稀疏、低秩、可加）如何驱动估计。

布局与 p21（van de Geer EPME）相同：Notes 汉语、Solutions 英语、一章一文件。

## 路径

- Notes：`notes/chXX-notes.qmd`
- Solutions：`solutions/chXX-solutions.qmd`
- 清单：`docs/companion-notes/chXX-content-map.md`
- 审核：`docs/companion-notes/chXX-review.md`
- 教材 PDF（勿提交）：`/home/fang/Project/zhihu-paper/p22/High-Dimensional Statistics A Non-Asymptotic Viewpoint (Martin J. Wainwright) (z-library.sk, 1lib.sk, z-lib.sk).pdf`
- 页码：正文 **PDF = 印刷 + 19**（Ch1 印刷 1 = PDF 20）
- 文本层可用但公式常错位；**每一条进入 Notes 的公式必须对照 `pdftoppm` 原页 PNG**，不要盲信 `pdftotext`

## 版本

Martin J. Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series in Statistical and Probabilistic Mathematics, No. 48。First published 2019；ISBN 978-1-108-49802-9 Hardback；DOI 10.1017/9781108627771；LCCN 2018043475。

## 章界（印刷页 → PDF 页）

| 章 | 印刷页 | PDF 页 |
|---|---|---|
| 1 Introduction | 1–20 | 20–39 |
| 2 Basic tail and concentration bounds | 21–57 | 40–76 |
| 3 Concentration of measure | 58–97 | 77–116 |
| 4 Uniform laws of large numbers | 98–120 | 117–139 |
| 5 Metric entropy and its uses | 121–158 | 140–177 |
| 6 Random matrices and covariance estimation | 159–193 | 178–212 |
| 7 Sparse linear models in high dimensions | 194–235 | 213–254 |
| 8 Principal component analysis in high dimensions | 236–258 | 255–277 |
| 9 Decomposability and restricted strong convexity | 259–311 | 278–330 |
| 10 Matrix estimation with rank constraints | 312–346 | 331–365 |
| 11 Graphical models for high-dimensional data | 347–382 | 366–401 |
| 12 Reproducing kernel Hilbert spaces | 383–415 | 402–434 |
| 13 Nonparametric least squares | 416–452 | 435–471 |
| 14 Localization and uniform laws | 453–484 | 472–503 |
| 15 Minimax lower bounds | 485–523 | 504–542 |

参考文献印刷 524 起 = PDF 543 起。每章末 *Exercises* 进 Solutions，不进 Notes。第 1 章无编号习题；正文把 (1.14) 留给读者，写入 Solutions。

## Notes 写法

对照 `notes/ch01-notes.qmd`：

- **Notes 用汉语**；英文术语首次给出。
- 保留原书节号与主线。
- 关键定义/定理用 `::: {.callout-important}`；作者补充标 `作者解释`。
- 每条关键公式写教材定位（节、印刷页、PDF 页）。
- 3–7 个可观察学习目标；常见错误；3–5 道自测（答案放 `<details>`，须含「参考答案」字样）。
- 章末必须有 `## 术语对照`；新词合并进 `glossary.qmd`（由父代理合并，子代理不要改 `glossary.qmd` / `_quarto.yml` / `index.qmd`）。
- 中文从名词委，英文从教材/国际通行用法；陈希孺别名只写备注。
- 不把全部习题解写进 Notes。
- front matter 含 `execute: enabled: false` 与 `lang: zh-CN`。
- 标题层级不可跳级（`#` 后不可直接 `###`）。
- Markdown 表单元格里不要写未转义的 `|`。

## Solutions 写法

对照 `solutions/ch01-solutions.qmd`：

- **Solutions 用英语。**
- 每题 `### Exercise x.y`，Stem (abridged) + Solution callouts。
- 独立求解；书中给的数值答案要验算。
- 多小问按 (a)(b)… 展开。
- 先从原书习题页锁定题号列表，再解题。

## 质量

- 公式对照 PDF 原页 PNG，不要盲信文本层。
- 不修改已有 ch01 文件，不提交 PDF。
- 子代理只写自己的 `notes/chXX-notes.qmd`、`solutions/chXX-solutions.qmd`、`docs/companion-notes/chXX-*`。
- 怀疑教材错误：保留原文与页码，标 `勘误待批`，不要写成已批准勘误。
- 写完后跑结构校验：

```text
ruby ~/.grok/skills/build-book-companion-notes/scripts/validate_chapter.rb \
  --stage map --map docs/companion-notes/chXX-content-map.md
ruby ~/.grok/skills/build-book-companion-notes/scripts/validate_chapter.rb \
  --stage notes --map docs/companion-notes/chXX-content-map.md \
  --notes notes/chXX-notes.qmd
```

零退出只说明结构合法，不说明数学或来源正确。
