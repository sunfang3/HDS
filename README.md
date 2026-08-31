# HDS Companion

Wainwright 伴读 **Notes（汉语）** 与 **Solutions（英语）**（*High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series in Statistical and Probabilistic Mathematics, No. 48）。全书译名见 [`glossary.qmd`](glossary.qmd)。

- **站点**：<https://sunfang3.github.io/HDS/>
- **仓库**：<https://github.com/sunfang3/HDS>
- **源格式**：**Quarto**（`.qmd` + `_quarto.yml`）
- **渲染**：`quarto render` → `_site/`
- **读者起点**：已学陈希孺《概率论与数理统计》（本科）；本书还要补尾界 / 测度集中 / 一致大数定律 / 度量熵 / 随机矩阵
- **不含**原书 PDF（本地可自备，已由 `.gitignore` 排除）

```bash
# 本地预览
quarto preview
# 或只构建
quarto render
```

## 读者向文件

| 章 | Notes | Solutions |
|---|---|---|
| 1 Introduction | [notes/ch01-notes.qmd](notes/ch01-notes.qmd) | [solutions/ch01-solutions.qmd](solutions/ch01-solutions.qmd) |
| 2 Tail bounds | [notes/ch02-notes.qmd](notes/ch02-notes.qmd) | [solutions/ch02-solutions.qmd](solutions/ch02-solutions.qmd) |
| 3 Concentration of measure | [notes/ch03-notes.qmd](notes/ch03-notes.qmd) | [solutions/ch03-solutions.qmd](solutions/ch03-solutions.qmd) |
| 4 Uniform laws | [notes/ch04-notes.qmd](notes/ch04-notes.qmd) | [solutions/ch04-solutions.qmd](solutions/ch04-solutions.qmd) |
| 5 Metric entropy | [notes/ch05-notes.qmd](notes/ch05-notes.qmd) | [solutions/ch05-solutions.qmd](solutions/ch05-solutions.qmd) |
| 6 Random matrices | [notes/ch06-notes.qmd](notes/ch06-notes.qmd) | [solutions/ch06-solutions.qmd](solutions/ch06-solutions.qmd) |
| 7 Sparse linear models | [notes/ch07-notes.qmd](notes/ch07-notes.qmd) | [solutions/ch07-solutions.qmd](solutions/ch07-solutions.qmd) |
| 8 Principal component analysis | [notes/ch08-notes.qmd](notes/ch08-notes.qmd) | [solutions/ch08-solutions.qmd](solutions/ch08-solutions.qmd) |
| 9 Decomposability and RSC | [notes/ch09-notes.qmd](notes/ch09-notes.qmd) | [solutions/ch09-solutions.qmd](solutions/ch09-solutions.qmd) |
| 10 Rank-constrained matrices | [notes/ch10-notes.qmd](notes/ch10-notes.qmd) | [solutions/ch10-solutions.qmd](solutions/ch10-solutions.qmd) |
| 11 Graphical models | [notes/ch11-notes.qmd](notes/ch11-notes.qmd) | [solutions/ch11-solutions.qmd](solutions/ch11-solutions.qmd) |
| 12 RKHS | [notes/ch12-notes.qmd](notes/ch12-notes.qmd) | [solutions/ch12-solutions.qmd](solutions/ch12-solutions.qmd) |
| 13 Nonparametric least squares | [notes/ch13-notes.qmd](notes/ch13-notes.qmd) | [solutions/ch13-solutions.qmd](solutions/ch13-solutions.qmd) |
| 14 Localization | [notes/ch14-notes.qmd](notes/ch14-notes.qmd) | [solutions/ch14-solutions.qmd](solutions/ch14-solutions.qmd) |
| 15 Minimax lower bounds | [notes/ch15-notes.qmd](notes/ch15-notes.qmd) | [solutions/ch15-solutions.qmd](solutions/ch15-solutions.qmd) |

## 内部工件

内容清单与审核报告在 `docs/companion-notes/`。读者合同见 [`docs/companion-notes/AUTHORING-CONTRACT.md`](docs/companion-notes/AUTHORING-CONTRACT.md)。

## 页码

2019 精装第一版：正文 **PDF 页 = 印刷页 + 19**。第 1 章印刷页 1 对应 PDF 页 20。
