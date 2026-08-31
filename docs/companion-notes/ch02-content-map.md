---
chapter_id: "ch02"
chapter_title: "Basic tail and concentration bounds"
source_title: "High-Dimensional Statistics: A Non-Asymptotic Viewpoint"
source_version: "Cambridge Series in Statistical and Probabilistic Mathematics, No. 48; first published 2019; ISBN 978-1-108-49802-9"
main_source_path: "High-Dimensional Statistics A Non-Asymptotic Viewpoint (Martin J. Wainwright) (z-library.sk, 1lib.sk, z-lib.sk).pdf"
printed_pages: "21–57"
pdf_pages: "40–76"
target_notes: "notes/ch02-notes.qmd"
language: "zh-CN"
learner_profile: "学过陈希孺《概率论与数理统计》本科教材；已掌握马尔可夫、切比雪夫、矩母函数与切尔诺夫思路，不从零重讲；需要把这些工具升级为次高斯/次指数语言，并接到霍夫丁、伯恩斯坦、鞅差与高斯利普希茨集中。"
map_status: "清单完成"
---

# 第 2 章内容清单

> 内部质量工件。正式内容（定义、命题、引理、定理、推论与关键编号公式）逐项登记。§2.7 习题 2.1–2.22 作为 EXERCISE 不进入 Notes。

## 来源边界

- 教材权威来源：Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series No. 48
- 版本识别依据：封面 Cambridge Series；版权页 © Martin J. Wainwright 2019，First published 2019，ISBN 978-1-108-49802-9 Hardback，DOI 10.1017/9781108627771
- 目标章节与页码：第 2 章，印刷页 21–57；PDF 页 40–76（**PDF = 印刷 + 19**）
- 补充来源及用途：无（习题独立求解）
- 已知来源限制：文本层可用但公式常错位；公式须对照 `scratch/ch02/p-040.png`–`p-076.png`

## 内容清单

| 定位 | 类型 | 内容/范围 | 重要性 | Notes 处理 | 合并目标/排除理由 | 核验状态 |
|---|---|---|---|---|---|---|
| 章首 印刷页 21；PDF 页 40 | SECTION | Chapter 2 Basic tail and concentration bounds：偏差界与集中不等式入口 | 关键 | 完整讲解 |  | 原页已核 |
| §2.1 印刷页 21–32；PDF 页 40–51 | SECTION | Classical bounds | 关键 | 完整讲解 |  | 原页已核 |
| §2.1.1 印刷页 21–22；PDF 页 40–41 | SECTION | From Markov to Chernoff | 关键 | 完整讲解 |  | 原页已核 |
| (2.1) 印刷页 21；PDF 页 40 | FORMULA | 马尔可夫不等式：非负 $X$ 有 $\mathbb P[X\ge t]\le\mathbb E[X]/t$ | 关键 | 完整讲解 |  | 原页已核 |
| (2.2) 印刷页 21；PDF 页 40 | FORMULA | 切比雪夫不等式：$\mathbb P[\lvert X-\mu\rvert\ge t]\le\mathrm{var}(X)/t^2$ | 关键 | 完整讲解 |  | 原页已核 |
| (2.3) 印刷页 21；PDF 页 40 | FORMULA | $k$ 阶中心矩马尔可夫：$\mathbb P[\lvert X-\mu\rvert\ge t]\le\mathbb E[\lvert X-\mu\rvert^k]/t^k$ | 关键 | 完整讲解 |  | 原页已核 |
| (2.4) 印刷页 22；PDF 页 41 | FORMULA | 指数马尔可夫：$\mathbb P[X-\mu\ge t]\le\mathbb E[e^{\lambda(X-\mu)}]/e^{\lambda t}$，$\lambda\in[0,b]$ | 关键 | 完整讲解 |  | 原页已核 |
| (2.5) 印刷页 22；PDF 页 41 | FORMULA | 切尔诺夫界：$\log\mathbb P[X-\mu\ge t]\le\inf_{\lambda\in[0,b]}\{\log\mathbb E[e^{\lambda(X-\mu)}]-\lambda t\}$ | 关键 | 完整讲解 |  | 原页已核 |
| §2.1.2 印刷页 22–25；PDF 页 41–44 | SECTION | Sub-Gaussian variables and Hoeffding bounds | 关键 | 完整讲解 |  | 原页已核 |
| Example 2.1 印刷页 22；PDF 页 41 | EXAMPLE | 高斯尾界：$N(\mu,\sigma^2)$ 的矩母函数 (2.6) 与上尾 (2.7) | 关键 | 完整讲解 |  | 原页已核 |
| (2.6) 印刷页 22；PDF 页 41 | FORMULA | $\mathbb E[e^{\lambda X}]=e^{\mu\lambda+\sigma^2\lambda^2/2}$，对一切 $\lambda\in\mathbb R$ | 关键 | 并入相关内容 | Example 2.1 | 原页已核 |
| (2.7) 印刷页 22；PDF 页 41 | FORMULA | $\mathbb P[X\ge\mu+t]\le e^{-t^2/(2\sigma^2)}$，$t\ge 0$ | 关键 | 完整讲解 |  | 原页已核 |
| Definition 2.2 印刷页 23；PDF 页 42 | DEFINITION | 次高斯：$\mathbb E[e^{\lambda(X-\mu)}]\le e^{\sigma^2\lambda^2/2}$，对一切 $\lambda\in\mathbb R$（2.8） | 关键 | 完整讲解 |  | 原页已核 |
| (2.8) 印刷页 23；PDF 页 42 | FORMULA | 次高斯矩母函数上界 | 关键 | 并入相关内容 | Definition 2.2 | 原页已核 |
| (2.9) 印刷页 23；PDF 页 42 | FORMULA | 次高斯集中：$\mathbb P[\lvert X-\mu\rvert\ge t]\le 2e^{-t^2/(2\sigma^2)}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 2.3 印刷页 23；PDF 页 42 | EXAMPLE | 拉德马赫变量 $\varepsilon\in\{\pm 1\}$ 等概率，次高斯参数 $\sigma=1$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 2.4 印刷页 24；PDF 页 43 | EXAMPLE | 有界零均值 $X\in[a,b]$：对称化给出 $\sigma\le b-a$；Exercise 2.4 锐化到 $(b-a)/2$ | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 2.5 印刷页 24；PDF 页 43 | PROPOSITION | 霍夫丁界：独立次高斯和的上尾 (2.10) | 关键 | 完整讲解 |  | 原页已核 |
| (2.10) 印刷页 24；PDF 页 43 | FORMULA | $\mathbb P[\sum(X_i-\mu_i)\ge t]\le\exp(-t^2/(2\sum\sigma_i^2))$ | 关键 | 并入相关内容 | Proposition 2.5 | 原页已核 |
| (2.11) 印刷页 25；PDF 页 44 | FORMULA | 有界霍夫丁：$\mathbb P[\sum(X_i-\mu_i)\ge t]\le e^{-2t^2/(n(b-a)^2)}$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 2.6 印刷页 25；PDF 页 44 | THEOREM | 次高斯四条等价刻画 (2.12a)–(2.12d) | 关键 | 完整讲解 |  | 原页已核 |
| (2.12a) 印刷页 25；PDF 页 44 | FORMULA | (I) 矩母函数 $\mathbb E[e^{\lambda X}]\le e^{\lambda^2\sigma^2/2}$ | 关键 | 并入相关内容 | Theorem 2.6 | 原页已核 |
| (2.12b) 印刷页 25；PDF 页 44 | FORMULA | (II) 被某高斯 $Z\sim N(0,\tau^2)$ 控制尾概率 | 关键 | 并入相关内容 | Theorem 2.6 | 原页已核 |
| (2.12c) 印刷页 25；PDF 页 44 | FORMULA | (III) 偶矩 $\mathbb E[X^{2k}]\le (2k)!\,\theta^{2k}/(2^k k!)$ | 关键 | 并入相关内容 | Theorem 2.6 | 原页已核 |
| (2.12d) 印刷页 25；PDF 页 44 | FORMULA | (IV) $\mathbb E[e^{\lambda X^2/(2\sigma^2)}]\le 1/\sqrt{1-\lambda}$，$\lambda\in[0,1)$ | 关键 | 并入相关内容 | Theorem 2.6 | 原页已核 |
| §2.1.3 印刷页 25–31；PDF 页 44–50 | SECTION | Sub-exponential variables and Bernstein bounds | 关键 | 完整讲解 |  | 原页已核 |
| Definition 2.7 印刷页 26；PDF 页 45 | DEFINITION | 次指数：$\mathbb E[e^{\lambda(X-\mu)}]\le e^{\nu^2\lambda^2/2}$，对 $\lvert\lambda\rvert<1/\alpha$（2.13） | 关键 | 完整讲解 |  | 原页已核 |
| (2.13) 印刷页 26；PDF 页 45 | FORMULA | 次指数矩母函数上界 | 关键 | 并入相关内容 | Definition 2.7 | 原页已核 |
| Example 2.8 印刷页 26；PDF 页 45 | EXAMPLE | $X=Z^2$、$Z\sim N(0,1)$：非次高斯，次指数参数 $(\nu,\alpha)=(2,4)$；(2.14) | 关键 | 完整讲解 |  | 原页已核 |
| (2.14) 印刷页 26；PDF 页 45 | FORMULA | $e^{-\lambda}/\sqrt{1-2\lambda}\le e^{2\lambda^2}=e^{4\lambda^2/2}$，$\lvert\lambda\rvert<1/4$ | 辅助 | 并入相关内容 | Example 2.8 | 原页已核 |
| Proposition 2.9 印刷页 26；PDF 页 45 | PROPOSITION | 次指数尾界：二次区制 $t\le\nu^2/\alpha$，线性区制 $t>\nu^2/\alpha$ | 关键 | 完整讲解 |  | 原页已核 |
| (2.15) 印刷页 27；PDF 页 46 | FORMULA | 伯恩斯坦条件：$\lvert\mathbb E[(X-\mu)^k]\rvert\le\frac12 k!\,\sigma^2 b^{k-2}$，$k\ge 2$ | 关键 | 完整讲解 |  | 原页已核 |
| (2.16) 印刷页 28；PDF 页 47 | FORMULA | 由 (2.15) 得 $\mathbb E[e^{\lambda(X-\mu)}]\le\exp((\lambda^2\sigma^2/2)/(1-b\lvert\lambda\rvert))$，$\lvert\lambda\rvert<1/b$ | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 2.10 印刷页 28；PDF 页 47 | PROPOSITION | 伯恩斯坦型界：(2.17a) 矩母函数与 (2.17b) 集中 | 关键 | 完整讲解 |  | 原页已核 |
| (2.17a) 印刷页 28；PDF 页 47 | FORMULA | $\mathbb E[e^{\lambda(X-\mu)}]\le\exp((\lambda^2\sigma^2/2)/(1-b\lvert\lambda\rvert))$，$\lvert\lambda\rvert<1/b$ | 关键 | 并入相关内容 | Proposition 2.10 | 原页已核 |
| (2.17b) 印刷页 28；PDF 页 47 | FORMULA | $\mathbb P[\lvert X-\mu\rvert\ge t]\le 2e^{-t^2/(2(\sigma^2+bt))}$ | 关键 | 并入相关内容 | Proposition 2.10 | 原页已核 |
| §2.1.3 印刷页 28–29；PDF 页 47–48 | FORMULA | 独立次指数和：参数 $(\nu_*,\alpha_*)$，$\alpha_*=\max\alpha_k$，$\nu_*=\sqrt{\sum\nu_k^2}$ | 关键 | 完整讲解 |  | 原页已核 |
| (2.18) 印刷页 29；PDF 页 48 | FORMULA | 样本均值的次指数上尾：二次/线性两段 | 关键 | 完整讲解 |  | 原页已核 |
| Example 2.11 印刷页 29；PDF 页 48 | EXAMPLE | $\chi^2_n$：参数 $(2\sqrt n,4)$，两尾 (2.19) | 关键 | 完整讲解 |  | 原页已核 |
| (2.19) 印刷页 29；PDF 页 48 | FORMULA | $\mathbb P[\lvert n^{-1}\sum Z_k^2-1\rvert\ge t]\le 2e^{-nt^2/8}$，$t\in(0,1)$ | 关键 | 并入相关内容 | Example 2.11 | 原页已核 |
| Example 2.12 印刷页 29–30；PDF 页 48–49 | EXAMPLE | 约翰逊–林登施特劳斯嵌入：随机高斯投影保持两两距离 | 关键 | 完整讲解 |  | 原页已核 |
| (2.20) 印刷页 30；PDF 页 49 | FORMULA | $(1-\delta)\le\lVert F(u^i)-F(u^j)\rVert_2^2/\lVert u^i-u^j\rVert_2^2\le(1+\delta)$；需 $m\gtrsim\delta^{-2}\log N$ | 关键 | 并入相关内容 | Example 2.12 | 原页已核 |
| Theorem 2.13 印刷页 31；PDF 页 50 | THEOREM | 次指数四条等价刻画 (2.21a)–(2.21b) 与 $\gamma=\sup_k(\mathbb E[\lvert X\rvert^k]/k!)^{1/k}<\infty$ | 关键 | 完整讲解 |  | 原页已核 |
| (2.21a) 印刷页 31；PDF 页 50 | FORMULA | (I) $\mathbb E[e^{\lambda X}]\le e^{\nu^2\lambda^2/2}$，$\lvert\lambda\rvert<1/\alpha$ | 关键 | 并入相关内容 | Theorem 2.13 | 原页已核 |
| (2.21b) 印刷页 31；PDF 页 50 | FORMULA | (III) $\mathbb P[\lvert X\rvert\ge t]\le c_1 e^{-c_2 t}$ | 关键 | 并入相关内容 | Theorem 2.13 | 原页已核 |
| §2.1.4 印刷页 31–32；PDF 页 50–51 | SECTION | Some one-sided results | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 2.14 印刷页 31；PDF 页 50 | PROPOSITION | 单侧伯恩斯坦：(2.22a) 矩母函数与 (2.22b) 独立和上尾 | 关键 | 完整讲解 |  | 原页已核 |
| (2.22a) 印刷页 31；PDF 页 50 | FORMULA | $X\le b$ a.s. 时 $\mathbb E[e^{\lambda(X-\mathbb E X)}]\le\exp((\lambda^2\mathbb E[X^2]/2)/(1-b\lambda/3))$，$\lambda\in[0,3/b)$ | 关键 | 并入相关内容 | Proposition 2.14 | 原页已核 |
| (2.22b) 印刷页 31；PDF 页 50 | FORMULA | $\mathbb P[\sum(X_i-\mathbb E X_i)\ge n\delta]\le\exp(-n\delta^2/(2(n^{-1}\sum\mathbb E[X_i^2]+b\delta/3)))$ | 关键 | 并入相关内容 | Proposition 2.14 | 原页已核 |
| (2.23) 印刷页 31；PDF 页 50 | FORMULA | 非负变量下尾：$\mathbb P[\sum(Y_i-\mathbb E Y_i)\le -n\delta]\le\exp(-n\delta^2/(2 n^{-1}\sum\mathbb E[Y_i^2]))$ | 关键 | 完整讲解 |  | 原页已核 |
| §2.2 印刷页 32–40；PDF 页 51–59 | SECTION | Martingale-based methods | 关键 | 完整讲解 |  | 原页已核 |
| §2.2.1 印刷页 33–35；PDF 页 52–54 | SECTION | Background：过滤、适应、杜布鞅、鞅差 | 关键 | 完整讲解 |  | 原页已核 |
| (2.24) 印刷页 33；PDF 页 52 | FORMULA | 杜布鞅：$Y_k=\mathbb E[f(X)\mid X_1,\ldots,X_k]$ | 关键 | 完整讲解 |  | 原页已核 |
| Definition 2.15 印刷页 33；PDF 页 52 | DEFINITION | 鞅：$\mathbb E[\lvert Y_k\rvert]<\infty$ 且 $\mathbb E[Y_{k+1}\mid\mathcal F_k]=Y_k$（2.25） | 关键 | 完整讲解 |  | 原页已核 |
| (2.25) 印刷页 33；PDF 页 52 | FORMULA | 鞅定义等式 | 关键 | 并入相关内容 | Definition 2.15 | 原页已核 |
| Example 2.16 印刷页 33–34；PDF 页 52–53 | EXAMPLE | i.i.d. 部分和 $S_k-k\mu$ 是鞅 | 辅助 | 简要说明 |  | 原页已核 |
| Example 2.17 印刷页 34；PDF 页 53 | EXAMPLE | 杜布构造：$Y_k=\mathbb E[f(X)\mid X_1^k]$ 在 $\mathbb E[\lvert f\rvert]<\infty$ 时是鞅 | 关键 | 完整讲解 |  | 原页已核 |
| Example 2.18 印刷页 34；PDF 页 53 | EXAMPLE | 似然比 $Y_k=\prod_{\ell=1}^k g(X_\ell)/f(X_\ell)$ 是鞅 | 辅助 | 简要说明 |  | 原页已核 |
| (2.26) 印刷页 34；PDF 页 53 | DEFINITION | 鞅差：$\mathbb E[\lvert D_k\rvert]<\infty$ 且 $\mathbb E[D_{k+1}\mid\mathcal F_k]=0$ | 关键 | 完整讲解 |  | 原页已核 |
| (2.27) 印刷页 35；PDF 页 54 | FORMULA | 望远镜：$Y_n-Y_0=\sum_{k=1}^n D_k$ | 关键 | 完整讲解 |  | 原页已核 |
| §2.2.2 印刷页 35–40；PDF 页 54–59 | SECTION | Concentration bounds for martingale difference sequences | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 2.19 印刷页 35；PDF 页 54 | THEOREM | 条件次指数鞅差之和仍次指数；两尾 (2.28) | 关键 | 完整讲解 |  | 原页已核 |
| (2.28) 印刷页 35；PDF 页 54 | FORMULA | $\mathbb P[\lvert\sum D_k\rvert\ge t]$ 的二次/线性两段，系数 2 | 关键 | 并入相关内容 | Theorem 2.19 | 原页已核 |
| (2.29) 印刷页 36；PDF 页 55 | FORMULA | 迭代条件期望控制鞅差和的矩母函数 | 辅助 | 并入相关内容 | Theorem 2.19 | 原页已核 |
| Corollary 2.20 印刷页 36；PDF 页 55 | COROLLARY | 阿祖马–霍夫丁：$D_k\in[a_k,b_k]$ 时 (2.30) | 关键 | 完整讲解 |  | 原页已核 |
| (2.30) 印刷页 36；PDF 页 55 | FORMULA | $\mathbb P[\lvert\sum D_k\rvert\ge t]\le 2e^{-2t^2/\sum(b_k-a_k)^2}$ | 关键 | 并入相关内容 | Corollary 2.20 | 原页已核 |
| (2.31) 印刷页 36；PDF 页 55 | FORMULA | 改第 $k$ 坐标：$x^{\backslash k}$ | 辅助 | 并入相关内容 | Corollary 2.21 | 原页已核 |
| (2.32) 印刷页 36；PDF 页 55 | DEFINITION | 有界差分：$\lvert f(x)-f(x^{\backslash k})\rvert\le L_k$ | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 2.21 印刷页 37；PDF 页 56 | COROLLARY | 有界差分不等式（McDiarmid）：独立坐标下 (2.33) | 关键 | 完整讲解 |  | 原页已核 |
| (2.33) 印刷页 37；PDF 页 56 | FORMULA | $\mathbb P[\lvert f(X)-\mathbb E f(X)\rvert\ge t]\le 2e^{-2t^2/\sum L_k^2}$ | 关键 | 并入相关内容 | Corollary 2.21 | 原页已核 |
| (2.34) 印刷页 37；PDF 页 56 | FORMULA | 杜布鞅差 $D_k=\mathbb E[f\mid X_1^k]-\mathbb E[f\mid X_1^{k-1}]$ | 辅助 | 并入相关内容 | Corollary 2.21 | 原页已核 |
| (2.35) 印刷页 37；PDF 页 56 | FORMULA | 汉明利普希茨特例：$2e^{-2t^2/(n L^2)}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 2.22 印刷页 38；PDF 页 57 | EXAMPLE | 由有界差分回收经典霍夫丁 (2.11) | 辅助 | 简要说明 |  | 原页已核 |
| Example 2.23 印刷页 38；PDF 页 57 | EXAMPLE | 成对 $U$-统计量 (2.36)：$\lvert g\rvert_\infty\le b$ 时 $L_k=4b/n$，尾 $2e^{-nt^2/(8b^2)}$ | 关键 | 完整讲解 |  | 原页已核 |
| (2.36) 印刷页 38；PDF 页 57 | FORMULA | $U=\binom n2^{-1}\sum_{j<k}g(X_j,X_k)$ | 关键 | 并入相关内容 | Example 2.23 | 原页已核 |
| Example 2.24 印刷页 39；PDF 页 58 | EXAMPLE | 埃尔德什–雷尼图的团数：改一条边团数最多变 1 | 辅助 | 简要说明 |  | 原页已核 |
| Example 2.25 印刷页 39–40；PDF 页 58–59 | EXAMPLE | 拉德马赫复杂度 $Z=\sup_{a\in\mathcal A}\langle a,\varepsilon\rangle$（2.37）；次高斯参数 $2\sqrt{\sum_k\sup_a a_k^2}$ | 关键 | 完整讲解 |  | 原页已核 |
| (2.37) 印刷页 39；PDF 页 58 | FORMULA | 拉德马赫复杂度随机变量 | 关键 | 并入相关内容 | Example 2.25 | 原页已核 |
| §2.3 印刷页 40–45；PDF 页 59–64 | SECTION | Lipschitz functions of Gaussian variables | 关键 | 完整讲解 |  | 原页已核 |
| (2.38) 印刷页 40；PDF 页 59 | DEFINITION | 欧氏利普希茨：$\lvert f(x)-f(y)\rvert\le L\lVert x-y\rVert_2$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 2.26 印刷页 40；PDF 页 59 | THEOREM | 标准高斯向量的 $L$-利普希茨函数是参数 $\le L$ 的次高斯；(2.39) | 关键 | 完整讲解 |  | 原页已核 |
| (2.39) 印刷页 40；PDF 页 59 | FORMULA | $\mathbb P[\lvert f(X)-\mathbb E f(X)\rvert\ge t]\le 2e^{-t^2/(2L^2)}$ | 关键 | 并入相关内容 | Theorem 2.26 | 原页已核 |
| Lemma 2.27 印刷页 41；PDF 页 60 | LEMMA | 凸 $\phi$ 的高斯插值：$\mathbb E[\phi(f(X)-\mathbb E f)]\le\mathbb E[\phi((\pi/2)\langle\nabla f(X),Y\rangle)]$（2.40） | 关键 | 完整讲解 |  | 原页已核 |
| (2.40) 印刷页 41；PDF 页 60 | FORMULA | Lemma 2.27 的不等式 | 关键 | 并入相关内容 | Lemma 2.27 | 原页已核 |
| (2.41)–(2.43) 印刷页 41–42；PDF 页 60–61 | PROOF_DERIVATION | 旋转不变插值：$Z(\theta)=X\sin\theta+Y\cos\theta$，Jensen 与 $\theta$-积分 | 关键 | 简要说明 |  | 原页已核 |
| Example 2.28 印刷页 42–43；PDF 页 61–62 | EXAMPLE | 经利普希茨得到 $\chi^2$ 上尾 (2.44)，常数劣于 Example 2.11 | 关键 | 完整讲解 |  | 原页已核 |
| (2.44) 印刷页 43；PDF 页 62 | FORMULA | $\mathbb P[Y\ge n(1+t)]\le e^{-nt^2/18}$，$t\in[0,3]$ | 关键 | 并入相关内容 | Example 2.28 | 原页已核 |
| Example 2.29 印刷页 43；PDF 页 62 | EXAMPLE | 次序统计量 (2.45) 是 1-利普希茨，故高斯时 $\delta^2/2$ 次高斯尾 | 辅助 | 简要说明 |  | 原页已核 |
| (2.45) 印刷页 43；PDF 页 62 | FORMULA | $X_{(1)}\le\cdots\le X_{(n)}$ | 辅助 | 并入相关内容 | Example 2.29 | 原页已核 |
| Example 2.30 印刷页 43；PDF 页 62 | EXAMPLE | 高斯复杂度 (2.46)；利普希茨常数 $D(\mathcal A)=\sup_{a\in\mathcal A}\lVert a\rVert_2$；(2.47) | 关键 | 完整讲解 |  | 原页已核 |
| (2.46) 印刷页 43；PDF 页 62 | FORMULA | $Z=\sup_{a\in\mathcal A}\langle a,W\rangle$ | 关键 | 并入相关内容 | Example 2.30 | 原页已核 |
| (2.47) 印刷页 43；PDF 页 62 | FORMULA | $\mathbb P[\lvert Z-\mathbb E Z\rvert\ge\delta]\le 2\exp(-\delta^2/(2D^2(\mathcal A)))$ | 关键 | 并入相关内容 | Example 2.30 | 原页已核 |
| Example 2.31 印刷页 44；PDF 页 63 | EXAMPLE | 解耦高斯混沌 $Z=w^T Q\widetilde w$：次指数尾，算子范数与弗罗贝尼乌斯范数 (2.48)–(2.50) | 辅助 | 简要说明 |  | 原页已核 |
| (2.48) 印刷页 44；PDF 页 63 | FORMULA | 条件高斯尾 $\mathbb P[\lvert Z\rvert\ge\delta\mid\widetilde w]\le 2e^{-\delta^2/(2\lVert Q\widetilde w\rVert_2^2)}$ | 辅助 | 并入相关内容 | Example 2.31 | 原页已核 |
| (2.49) 印刷页 44；PDF 页 63 | FORMULA | $\ell_2$-算子范数 $\lvert\lvert\lvert Q\rvert\rvert\rvert_2=\sup_{\lVert u\rVert_2=1}\lVert Qu\rVert_2$ | 辅助 | 并入相关内容 | Example 2.31 | 原页已核 |
| (2.50) 印刷页 44；PDF 页 63 | FORMULA | 弗罗贝尼乌斯范数 $\lvert\lvert\lvert Q\rvert\rvert\rvert_F=(\sum_{i,j}Q_{ij}^2)^{1/2}$ | 辅助 | 并入相关内容 | Example 2.31 | 原页已核 |
| Example 2.32 印刷页 44–45；PDF 页 63–64 | EXAMPLE | 高斯矩阵奇异值：Weyl (2.51) 给出 1-利普希茨，故 (2.52) | 辅助 | 简要说明 |  | 原页已核 |
| (2.51) 印刷页 45；PDF 页 64 | FORMULA | $\max_k\lvert\sigma_k(X)-\sigma_k(Y)\rvert\le\lvert\lvert\lvert X-Y\rvert\rvert\rvert_2\le\lvert\lvert\lvert X-Y\rvert\rvert\rvert_F$ | 辅助 | 并入相关内容 | Example 2.32 | 原页已核 |
| (2.52) 印刷页 45；PDF 页 64 | FORMULA | $\mathbb P[\lvert\sigma_k(X)-\mathbb E\sigma_k(X)\rvert\ge\delta]\le 2e^{-\delta^2/2}$ | 辅助 | 并入相关内容 | Example 2.32 | 原页已核 |
| §2.4 印刷页 45–48；PDF 页 64–67 | SECTION | Appendix A：Theorem 2.6 的等价性证明 | 关键 | 简要说明 |  | 原页已核 |
| (2.53) 印刷页 45；PDF 页 64 | FORMULA | $N(0,2\sigma^2)$ 的米尔斯比下界 | 辅助 | 并入相关内容 | §2.4 Appendix A | 原页已核 |
| (2.54) 印刷页 46；PDF 页 65 | FORMULA | 高斯偶矩 $\mathbb E[Z^{2k}]=(2k)!\,\tau^{2k}/(2^k k!)$ | 辅助 | 并入相关内容 | §2.4 Appendix A | 原页已核 |
| §2.5 印刷页 48–49；PDF 页 67–68 | SECTION | Appendix B：Theorem 2.13 的等价性证明 | 关键 | 简要说明 |  | 原页已核 |
| (2.58) 印刷页 49；PDF 页 68 | FORMULA | 次指数矩母函数幂级数与收敛半径 | 辅助 | 并入相关内容 | §2.5 Appendix B | 原页已核 |
| §2.6 印刷页 49–50；PDF 页 68–69 | PROSE_RANGE | Bibliographic details：Bernstein、Chernoff、Hoeffding、Azuma、JL、U-统计、高斯集中、Hanson–Wright、Ising | 辅助 | 指回教材 | 文献清单不抄入 Notes | 原页已核 |
| §2.7 印刷页 50–57；PDF 页 69–76 | SECTION | Exercises 2.1–2.22 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.1 印刷页 50；PDF 页 69 | EXERCISE | Tightness of Markov and Chebyshev | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.2 印刷页 50；PDF 页 69 | EXERCISE | Mills ratio (2.59) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.3 印刷页 50–51；PDF 页 69–70 | EXERCISE | Polynomial Markov versus Chernoff (2.60) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.4 印刷页 51；PDF 页 70 | EXERCISE | Sharp sub-Gaussian parameter $(b-a)/2$ | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.5 印刷页 51；PDF 页 70 | EXERCISE | Sub-Gaussian bounds and means/variances (2.61) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.6 印刷页 51；PDF 页 70 | EXERCISE | Lower bounds on squared sub-Gaussians | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.7 印刷页 51；PDF 页 70 | EXERCISE | Bennett's inequality (2.62) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.8 印刷页 52；PDF 页 71 | EXERCISE | Bernstein and expectations (2.63) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.9 印刷页 52；PDF 页 71 | EXERCISE | Sharp upper bounds on binomial tails (2.64) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.10 印刷页 52；PDF 页 71 | EXERCISE | Lower bounds on binomial tails (2.65a)–(2.65b) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.11 印刷页 53；PDF 页 72 | EXERCISE | Upper and lower bounds for Gaussian maxima | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.12 印刷页 53；PDF 页 72 | EXERCISE | Upper bounds for sub-Gaussian maxima (2.66)–(2.67) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.13 印刷页 53；PDF 页 72 | EXERCISE | Operations on sub-Gaussian variables | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.14 印刷页 53–54；PDF 页 72–73 | EXERCISE | Concentration around medians and means (2.68)–(2.69) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.15 印刷页 54；PDF 页 73 | EXERCISE | Kernel density estimation $L^1$ concentration | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.16 印刷页 54；PDF 页 73 | EXERCISE | Deviation inequalities in a Hilbert space | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.17 印刷页 54–55；PDF 页 73–74 | EXERCISE | Hanson–Wright inequality (2.70)–(2.71)，高斯特例 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.18 印刷页 55；PDF 页 74 | EXERCISE | Orlicz norms (2.72)–(2.73) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.19 印刷页 55；PDF 页 74 | EXERCISE | Maxima of Orlicz variables | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.20 印刷页 55；PDF 页 74 | EXERCISE | Tail bounds under moment conditions，Rosenthal | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.21 印刷页 55–56；PDF 页 74–75 | EXERCISE | Concentration and data compression，Bernoulli 率失真 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 2.22 印刷页 56–57；PDF 页 75–76 | EXERCISE | Concentration for spin glasses，SK/Ising 自由能 (2.74)–(2.76) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |

## 来源异常与勘误

| 定位 | 问题类型 | 原式/原文 | 核验证据 | 处置 | 数学复核人 | 批准人 |
|---|---|---|---|---|---|---|
| Example 2.24 印刷页 39；PDF 页 58 | 记号缺口 | 写出 $\mathbb P[n^{-1}\lvert C(G)-\mathbb E C(G)\rvert\ge\delta]\le 2e^{-2n\delta^2}$，本例未定义 $n$ | 原页；边指示向量维数是 $\binom d2$，(2.35) 的 $n$ 应为此 | 保留原文；Notes 标明 $n=\binom d2$；`勘误待批` | 作者 | 未批 |
| 印刷页 28 段末；PDF 页 47 | 笔误嫌疑 | 正文 “any bounded variable satisfies the Bernstein condition (2.16)” | 原页；(2.15) 才是伯恩斯坦条件，(2.16) 是其矩母函数推论 | 保留原文；Notes 按 (2.15) 解读；`勘误待批` | 作者 | 未批 |
| Exercise 2.21(b)(ii) 印刷页 56；PDF 页 75 | 笔误嫌疑 | “show that $\mathbb P[V\ge 1]\to+\infty$ as $n\to+\infty$” | 原页；概率不能趋于 $+\infty$；由 (i) 与 Exercise 2.10 应得 $\to 1$ | 保留原文；Solutions 按 $\to 1$ 证明并记录；`勘误待批` | 作者 | 未批 |
| Exercise 2.22(b) 印刷页 56；PDF 页 75 | 记号嫌疑 | $\lVert F_d(\theta)-F_d(\theta')\rVert_2\le\sqrt d\,\lVert\theta-\theta'\rVert_2$ | 原页；$F_d$ 是标量，左端应为绝对值 | 保留原文；Solutions 按绝对值理解；`勘误待批` | 作者 | 未批 |
| Exercise 2.22 (2.76) 印刷页 56；PDF 页 75 | 常数嫌疑 | 印刷尾界 $2e^{-\beta d t^2/2}$ | 原页；标准高斯利普希茨给出 $2\exp(-d t^2/(2\beta^2))$，指数中 $\beta$ 的位置不同 | 保留原文；Solutions 独立推导并对照；`勘误待批` | 作者 | 未批 |

## 完成检查

- [x] 主教材可读、版本可识别，且目标章节已定位。
- [x] 目标语言、学习者起点和 Notes 唯一路径均已确认。
- [x] 章节全部内容均有处理去向。
- [x] 定义、假设、命题、引理、定理、推论和关键公式均逐项登记。
- [x] 聚合条目仅覆盖处理方式相同的连续内容。
- [x] 所有 `并入相关内容` 条目均有明确合并目标。
- [x] 所有 `不进入 Notes` 条目均有理由，且不含正式内容。
- [x] Notes 实际转写的公式、表格、图形及低置信内容均已对照原页。
- [x] 作者补充的桥接推导均已完成独立数学复核。
- [x] 所有勘误均保留原文、证据、复核记录及明确批准。
- [x] 纳入 Notes 的来源公式均不再处于 `待核`、`勘误待批` 或 `受阻`。
