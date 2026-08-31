# HDS Companion

Wainwright 伴读 **Notes（汉语）** 与 **Solutions（英语）**（*High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series in Statistical and Probabilistic Mathematics, No. 48）。全书译名见 [`glossary.qmd`](glossary.qmd)。

- **站点**：尚未部署（目标形态与 EPME 相同：`sunfang3.github.io/HDS/`）
- **仓库**：尚未创建
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
| 2 Tail bounds | [notes/ch02-notes.qmd](notes/ch02-notes.qmd) | 编写中 |
| 3–15 | 编写中 | 编写中 |

## 内部工件

内容清单与审核报告在 `docs/companion-notes/`。读者合同见 [`docs/companion-notes/AUTHORING-CONTRACT.md`](docs/companion-notes/AUTHORING-CONTRACT.md)。

## 页码

2019 精装第一版：正文 **PDF 页 = 印刷页 + 19**。第 1 章印刷页 1 对应 PDF 页 20。
