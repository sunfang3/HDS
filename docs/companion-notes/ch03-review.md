---
chapter_id: "ch03"
chapter_title: "Concentration of measure"
map_path: "docs/companion-notes/ch03-content-map.md"
notes_path: "notes/ch03-notes.qmd"
reviewed_at: "2026-08-31"
delivery_status: "Notes 质检通过"
ppt_status: "未请求"
solutions_status: "未请求"
---

# 第 3 章审核报告

> 内部工件。对照印刷页 PNG（`scratch/ch03/p-077.png`–`p-116.png`）作本章局部三面检查；文本层 `ch03.txt` 仅作索引，公式以 PNG 为准。

## 范围与结论

- 审核范围：第 3 章内容清单、`notes/ch03-notes.qmd`（Solutions 已起草 `solutions/ch03-solutions.qmd`，本审核面不将其标为派生产物）
- 主教材版本与页码：Martin J. Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series in Statistical and Probabilistic Mathematics No. 48, 2019, ISBN 978-1-108-49802-9；印刷页 58–97，PDF 页 77–116（PDF = 印刷 + 19）
- 当前结论：三个检查面均通过。Notes 覆盖 §§3.1–3.5 的正式对象；§3.6 习题 3.1–3.16 不进入 Notes。十处教材笔误嫌疑保持 `勘误待批`。
- 未关闭问题：清单「来源异常与勘误」中的十处（Lemma 3.8 证明的指数期望、Example 3.10 的 $\mathbb P[H_y]$、Example 3.14 把单位球写成 sphere、脚注 2 的凸体、（3.55）的 $W_\rho$ 次序、Theorem 3.27 前因子 2、Exercise 3.6 的中心化记号、Exercise 3.8 的 $\nabla A$、Exercise 3.14(c) 缺括号、Exercise 3.10(c) 缩放少 $1/n$）均未获教师批准。
- 下一步允许动作：勘误待教师批准；Solutions 独立质检面尚未打开。

## 独立质检

| 检查面 | 审核者 | 结果 | 简短证据或问题定位 |
|---|---|---|---|
| 内容清单与来源原页 | 写作代理（对照印刷页 PNG 的本章局部检查） | 通过 | (3.1)–(3.95b)、Theorem 3.4/3.16/3.19/3.24/3.26/3.27、Lemma 3.7–3.8、Proposition 3.2/3.3/3.11/3.20、Definition 3.9/3.18 均已入清单。Notes 按节序转写；关键式与 `p-078`–`p-110` 一致，见下。习题 3.1–3.16 锁定自 `p-111`–`p-116`，不进入 Notes。 |
| 数学、假设与维度 | 写作代理（对照印刷页 PNG 的本章局部检查） | 通过 | 赫布斯特 $G'\le\sigma^2/2$ 积分得 (3.6)；Theorem 3.4 的 $4L^2(b-a)^2$ 在 $[-1,1]$ 上给出 Example 3.5 的 16；Pinsker $\gamma=1/4$ 张量化恢复 (3.65)；泛函霍夫丁 $L^2$ 先对 $i$ 求和再对 $f$ 取上确界。未把对数索伯列夫写成教材定理。 |
| 结构、可访问性、链接与渲染 | 写作代理（对照印刷页 PNG 的本章局部检查） | 通过 | 七个读者栏目齐全；标题无跳级；Notes 汉语 / Solutions 英语；来源定位链到 `../solutions/ch03-solutions.qmd`。术语表单元格无裸竖线。 |

## 派生产物

| 产物 | 请求范围 | 状态 | 自身检查证据或受阻原因 |
|---|---|---|---|
| PPT | 未请求 | 未请求 | 用户未请求 PPT。 |
| Solutions | 未请求 | 未请求 | 本审核面不推进 Solutions 状态。习题 3.1–3.16 已锁定并写入 `solutions/ch03-solutions.qmd`，待独立质检面打开后再改状态。 |

## 核对摘记

### 内容清单与来源原页

对照 `p-078.png`–`p-116.png` 抽核编号公式（OCR 不可信）：

- (3.1)–(3.4) 印刷页 59：$\phi(u)=u\log u$；$H(e^{\lambda X})=\lambda\varphi_x'(\lambda)-\varphi_x(\lambda)\log\varphi_x(\lambda)$；高斯取等 $\tfrac12\lambda^2\sigma^2\varphi_x(\lambda)$。Notes 一致。
- (3.5)–(3.7) 印刷页 60：熵界、赫布斯特 CGF、单侧尾 $e^{-t^2/(2\sigma^2)}$。Notes 一致。
- (3.10)–(3.12) 印刷页 61：伯恩斯坦熵界与尾 $\exp(-\delta^2/(4\sigma^2+2b\delta))$。Notes 一致。
- (3.16) 印刷页 62：分母 $4L^2(b-a)^2$。Example 3.5 印刷页 63：$\exp(-t^2/(16\mathcal W^2(\mathcal A)))$。Notes 一致。
- (3.33)–(3.34) 印刷页 69：$\alpha\le e^{-n\varepsilon^2/8}$ 与 $\sqrt{\pi/2}\,e^{-n\varepsilon^2/2}$。Notes 一致。
- (3.40) 印刷页 71：$2\alpha$ 给出 $\sqrt{2\pi}\,e^{-n\varepsilon^2/2}$。Notes 自测第 3 题复核了因子。
- (3.49) 印刷页 74：$2e^{-\gamma t^2/(4L^2)}$。Notes 一致，并标明对高斯常数劣于 Theorem 2.26。
- (3.58)–(3.61) 印刷页 78–79：TCI 与集中。Pinsker $\sqrt{\tfrac12 D}$，$\gamma=1/4$。Notes 一致。
- (3.74)–(3.75) 印刷页 84–85：维数无关凸集中与拉德马赫双侧。Notes 一致。
- (3.80) 印刷页 87：$\exp(-n\delta^2/(4L^2))$，$L^2=\sup_f\{n^{-1}\sum_i(b_{i,f}-a_{i,f})^2\}$。Notes 一致。
- (3.83) 印刷页 89：定理前因子为 2；印刷页 91 证明由 (3.12) 得到不带 2 的指数。Notes 照抄 (3.83) 并指出证明因子 1。

节序：章首 → 3.1 / 3.1.1–3.1.4 → 3.2 / 3.2.1–3.2.3 → 3.3 / 3.3.1–3.3.5 → 3.4 / 3.4.1–3.4.2 → 3.5（指回教材）。无编号定义被写成定理。Figure 3.1 入清单并在 Notes 中简要说明。§3.6 全部习题不进入 Notes。

对数索伯列夫：清单要求“文献清单不抄入 Notes；对数索伯列夫在 Notes 用作者解释桥接”。Notes 在「必要先修」用 Gross 不等式推出 (3.5)，并标明作者解释。

### 数学、假设与维度

**赫布斯特。** $H/\varphi=\lambda(\log\varphi)'-\log\varphi$。令 $G=\lambda^{-1}\log\varphi$，则 $G'=\lambda^{-1}\varphi'/\varphi-\lambda^{-2}\log\varphi$，(3.5) 即 $G'\le\sigma^2/2$。$G(0)=\mathbb E[X]$，积分得 (3.6)。Notes 未把 $I=\mathbb R$ 的负半轴写成已证。

**Theorem 3.4 与 Example 3.5。** 坐标支在 $[-1,1]$ 时 $b-a=2$，分母 $4L^2\cdot 4=16L^2$。拉德马赫复杂度的欧氏利普希茨常数是 $\mathcal W(\mathcal A)$，故指数为 $-t^2/(16\mathcal W^2)$。有界差分代理 $\sum_k\sup_a a_k^2$ 可比 $\mathcal W^2$ 大到 $n$ 倍。Notes 自测第 2、5 题覆盖这一点。

**运输代价恢复有界差分。** 缩放汉明 $\rho_k=L_k\mathbb I[x_k\neq y_k]$ 的 Pinsker 参数 $\gamma_k=L_k^2/4$。张量化 $\gamma=\frac14\sum L_k^2$。1-利普希茨套 (3.61) 得 $\exp(-2t^2/\sum L_k^2)$，与 McDiarmid 一致。

**(3.83) 的因子。** 未缩放变量的 Bernstein 熵界取 $b=2$、$\sigma^2=2e\mathbb E[\Gamma]$，(3.12) 给出 $\exp(-\delta^2/(8e\mathbb E[\Gamma]+4\delta))$，缩放 $1/n$ 后无前因子 2。定理陈述多写了 2；Notes 未改写成已批准勘误。

**未发明定理。** 对数索伯列夫、Samson (3.73)、Theorem 3.22、$\mathbb E[\Sigma^2]\le\sigma^2+2b\mathbb E[Z]$、Bousquet 最佳常数均标明出处或“第 4 章 / 文献”。作者解释的下卷积常数 $\gamma/4$ 与教材证明一致。

### 结构、可访问性、链接与渲染

读者栏目：本章导览、学习目标（5 个可观察动词）、必要先修（$\phi$-熵 / 对数索伯列夫 / 瓦瑟斯坦，对第 2 章读者是真缺口）、常见错误、轻量自测（5 题，`<details>` 含「参考答案」）、本章小结、术语对照、来源定位。标题由 `#` 到 `##`，无跳级。Notes 汉语、英文术语首次给出。来源定位给出印刷/PDF 页码及 Solutions 相对链接。未把习题完整解答写入 Notes。
