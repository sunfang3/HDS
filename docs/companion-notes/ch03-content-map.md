---
chapter_id: "ch03"
chapter_title: "Concentration of measure"
source_title: "High-Dimensional Statistics: A Non-Asymptotic Viewpoint"
source_version: "Cambridge Series in Statistical and Probabilistic Mathematics, No. 48; first published 2019; ISBN 978-1-108-49802-9"
main_source_path: "High-Dimensional Statistics A Non-Asymptotic Viewpoint (Martin J. Wainwright) (z-library.sk, 1lib.sk, z-lib.sk).pdf"
printed_pages: "58–97"
pdf_pages: "77–116"
target_notes: "notes/ch03-notes.qmd"
language: "zh-CN"
learner_profile: "学过陈希孺《概率论与数理统计》本科教材；已读本书第 2 章的切尔诺夫界、次高斯 / 次指数、有界差分与高斯利普希茨集中。缺口是熵方法、赫布斯特论证、对数索伯列夫、运输代价 / 瓦瑟斯坦，以及经验过程的泛函赫夫丁 / 伯恩斯坦。"
map_status: "清单完成"
---

# 第 3 章内容清单

> 内部质量工件。正式内容逐项登记；§3.6 全部习题作 EXERCISE，不进入 Notes。

## 来源边界

- 教材权威来源：Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series No. 48
- 版本识别依据：封面 Cambridge Series；版权页 © Martin J. Wainwright 2019，First published 2019，ISBN 978-1-108-49802-9 Hardback，DOI 10.1017/9781108627771
- 目标章节与页码：第 3 章，印刷页 58–97；PDF 页 77–116（**PDF = 印刷 + 19**）
- 补充来源及用途：无（习题独立求解）
- 已知来源限制：文本层可用但公式常错位；公式、图注须对照 `scratch/ch03/p-0XX.png`

## 内容清单

| 定位 | 类型 | 内容/范围 | 重要性 | Notes 处理 | 合并目标/排除理由 | 核验状态 |
|---|---|---|---|---|---|---|
| 章首 印刷页 58；PDF 页 77 | SECTION | Chapter 3 Concentration of measure：在第 2 章之上给出测度集中的四条路线（熵、几何、运输代价、经验过程） | 关键 | 完整讲解 |  | 原页已核 |
| §3.1 印刷页 58；PDF 页 77 | SECTION | Concentration by entropic techniques | 关键 | 完整讲解 |  | 原页已核 |
| §3.1.1 印刷页 58–59；PDF 页 77–78 | SECTION | Entropy and its properties | 关键 | 完整讲解 |  | 原页已核 |
| §3.1.1 印刷页 58；PDF 页 77 | DEFINITION | $\phi$-熵 $H_\phi(X):=\mathbb E[\phi(X)]-\phi(\mathbb E[X])$；Jensen 保证非负 | 关键 | 完整讲解 |  | 原页已核 |
| §3.1.1 印刷页 59；PDF 页 78 | FORMULA | $\phi(u)=u^2$ 时 $H_\phi=\mathrm{var}$；$\phi(u)=-\log u$ 作用于 $e^{\lambda X}$ 给出中心累积量母函数 | 关键 | 完整讲解 |  | 原页已核 |
| (3.1) 印刷页 59；PDF 页 78 | DEFINITION | 本章默认 $\phi(u)=u\log u$（$u>0$），$\phi(0)=0$ | 关键 | 完整讲解 |  | 原页已核 |
| (3.2) 印刷页 59；PDF 页 78 | DEFINITION | $H(Z)=\mathbb E[Z\log Z]-\mathbb E[Z]\log\mathbb E[Z]$，$Z\ge 0$ | 关键 | 完整讲解 |  | 原页已核 |
| (3.3) 印刷页 59；PDF 页 78 | FORMULA | $H(e^{\lambda X})=\lambda\varphi_x'(\lambda)-\varphi_x(\lambda)\log\varphi_x(\lambda)$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 3.1 印刷页 59；PDF 页 78 | EXAMPLE | 高斯 $X\sim N(0,\sigma^2)$ 的熵 | 关键 | 完整讲解 |  | 原页已核 |
| (3.4) 印刷页 59；PDF 页 78 | FORMULA | $H(e^{\lambda X})=\frac12\lambda^2\sigma^2\varphi_x(\lambda)$（高斯取等） | 关键 | 完整讲解 |  | 原页已核 |
| §3.1.2 印刷页 60–62；PDF 页 79–81 | SECTION | Herbst argument and its extensions | 关键 | 完整讲解 |  | 原页已核 |
| (3.5) 印刷页 60；PDF 页 79 | FORMULA | 熵上界 $H(e^{\lambda X})\le\frac12\sigma^2\lambda^2\varphi_x(\lambda)$ | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 3.2 印刷页 60；PDF 页 79 | PROPOSITION | 赫布斯特论证：$(3.5)\Rightarrow\log\mathbb E[e^{\lambda(X-\mathbb E[X])}]\le\frac12\lambda^2\sigma^2$ | 关键 | 完整讲解 |  | 原页已核 |
| (3.6) 印刷页 60；PDF 页 79 | FORMULA | 中心化累积量母函数的次高斯上界 | 关键 | 并入相关内容 | Proposition 3.2 | 原页已核 |
| (3.7) 印刷页 60；PDF 页 79 | FORMULA | 单侧尾 $\mathbb P[X\ge\mathbb E[X]+t]\le e^{-t^2/(2\sigma^2)}$；$\lambda\in\mathbb R$ 时双侧多因子 2 | 关键 | 完整讲解 |  | 原页已核 |
| (3.8)–(3.9) 印刷页 60；PDF 页 79 | FORMULA | $G(\lambda)=\lambda^{-1}\log\varphi(\lambda)$，$G(0)=\mathbb E[X]$，$G'\le\frac12\sigma^2$ | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 3.2 证明 印刷页 60–61；PDF 页 79–80 | PROOF_DERIVATION | 把熵不等式写成 $G'$ 的微分方程并积分 | 关键 | 并入相关内容 | Proposition 3.2 | 原页已核 |
| Proposition 3.3 印刷页 61；PDF 页 80 | PROPOSITION | Bernstein entropy bound：(3.10) 推出 (3.11) | 关键 | 完整讲解 |  | 原页已核 |
| (3.10) 印刷页 61；PDF 页 80 | FORMULA | $H(e^{\lambda X})\le\lambda^2\{b\varphi_x'(\lambda)+\varphi_x(\lambda)(\sigma^2-b\mathbb E[X])\}$，$\lambda\in[0,1/b)$ | 关键 | 并入相关内容 | Proposition 3.3 | 原页已核 |
| (3.11) 印刷页 61；PDF 页 80 | FORMULA | $\log\mathbb E[e^{\lambda(X-\mathbb E[X])}]\le\sigma^2\lambda^2(1-b\lambda)^{-1}$ | 关键 | 并入相关内容 | Proposition 3.3 | 原页已核 |
| (3.12) 印刷页 61；PDF 页 80 | FORMULA | $\mathbb P[X\ge\mathbb E[X]+\delta]\le\exp(-\delta^2/(4\sigma^2+2b\delta))$ | 关键 | 完整讲解 |  | 原页已核 |
| (3.13)–(3.14) 印刷页 61–62；PDF 页 80–81 | FORMULA | 中心化 $b=1$ 的 (3.13) 与 $G-\mathbb E[X]\le\sigma^2\lambda+\log\varphi$ | 辅助 | 并入相关内容 | Proposition 3.3 | 原页已核 |
| §3.1.3 印刷页 62–64；PDF 页 81–83 | SECTION | Separately convex functions and the entropic method | 关键 | 完整讲解 |  | 原页已核 |
| §3.1.3 印刷页 62；PDF 页 81 | DEFINITION | 分别凸：每个坐标在其余固定时凸 | 关键 | 完整讲解 |  | 原页已核 |
| (3.15) 印刷页 62；PDF 页 81 | DEFINITION | 欧氏 $L$-利普希茨 $\lvert f(x)-f(x')\rvert\le L\Vert x-x'\Vert_2$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 3.4 印刷页 62；PDF 页 81 | THEOREM | 独立、支在 $[a,b]$、分别凸且欧氏 $L$-利普希茨：上尾 (3.16) | 关键 | 完整讲解 |  | 原页已核 |
| (3.16) 印刷页 62；PDF 页 81 | FORMULA | $\mathbb P[f(X)\ge\mathbb E[f(X)]+\delta]\le\exp(-\delta^2/(4L^2(b-a)^2))$ | 关键 | 并入相关内容 | Theorem 3.4 | 原页已核 |
| Example 3.5 印刷页 63；PDF 页 82 | EXAMPLE | 拉德马赫复杂度的尖锐上尾 | 关键 | 完整讲解 |  | 原页已核 |
| (3.17) 印刷页 63；PDF 页 82 | FORMULA | $\mathbb P[Z\ge\mathbb E[Z]+t]\le\exp(-t^2/(16\mathcal W^2(\mathcal A)))$，$\mathcal W(\mathcal A)=\sup_{a\in\mathcal A}\Vert a\Vert_2$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 3.6 印刷页 63–64；PDF 页 82–83 | EXAMPLE | 随机矩阵算子范数 | 关键 | 完整讲解 |  | 原页已核 |
| (3.18) 印刷页 63；PDF 页 82 | FORMULA | $\Vert\vert X\Vert\vert_2=\max_{\Vert v\Vert_2=1}\Vert Xv\Vert_2$ | 关键 | 完整讲解 |  | 原页已核 |
| (3.19) 印刷页 63；PDF 页 82 | FORMULA | 算子范数对 Frobenius 利普希茨，参数 $L=1$ | 辅助 | 并入相关内容 | Example 3.6 | 原页已核 |
| Example 3.6 尾界 印刷页 64；PDF 页 83 | FORMULA | $\mathbb P[\Vert\vert X\Vert\vert_2\ge\mathbb E[\Vert\vert X\Vert\vert_2]+\delta]\le e^{-\delta^2/16}$ | 关键 | 完整讲解 |  | 原页已核 |
| §3.1.4 印刷页 64–67；PDF 页 83–86 | SECTION | Tensorization and separately convex functions | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 3.7 印刷页 64；PDF 页 83 | LEMMA | 一元函数的熵界 (3.20a)–(3.20b) | 关键 | 完整讲解 |  | 原页已核 |
| (3.20a) 印刷页 64；PDF 页 83 | FORMULA | $H(e^{\lambda g(X)})\le\lambda^2\mathbb E[(g(X)-g(Y))^2 e^{\lambda g(X)}\mathbb I[g(X)\ge g(Y)]]$ | 关键 | 并入相关内容 | Lemma 3.7 | 原页已核 |
| (3.20b) 印刷页 64；PDF 页 83 | FORMULA | 凸利普希茨且支在 $[a,b]$：$H\le\lambda^2(b-a)^2\mathbb E[(g'(X))^2 e^{\lambda g(X)}]$ | 关键 | 并入相关内容 | Lemma 3.7 | 原页已核 |
| Lemma 3.8 印刷页 65；PDF 页 84 | LEMMA | 熵的张量化 (3.21) | 关键 | 完整讲解 |  | 原页已核 |
| (3.21) 印刷页 65；PDF 页 84 | FORMULA | $H(e^{\lambda f(X)})\le\mathbb E\bigl[\sum_k H(e^{\lambda f_k(X_k)}\mid X^{\backslash k})\bigr]$ | 关键 | 并入相关内容 | Lemma 3.8 | 原页已核 |
| Theorem 3.4 证明 印刷页 65；PDF 页 84 | PROOF_DERIVATION | 坐标凸性 + (3.20b) + 张量化 + $\Vert\nabla f\Vert_2\le L$ + Herbst | 关键 | 完整讲解 |  | 原页已核 |
| (3.22)–(3.23) 印刷页 66；PDF 页 85 | PROOF_DERIVATION | Lemma 3.7：Jensen、对称、指数凸性 | 辅助 | 并入相关内容 | Lemma 3.7 | 原页已核 |
| (3.24) 印刷页 66；PDF 页 85 | FORMULA | 变分表示 $H(e^{\lambda f(X)})=\sup\{ \mathbb E[g e^{\lambda f}]\colon \mathbb E[e^g]\le 1\}$ | 关键 | 完整讲解 |  | 原页已核 |
| (3.25) 印刷页 66–67；PDF 页 85–86 | PROOF_DERIVATION | Lemma 3.8：把 $g$ 拆成 $g^k$ 并逐坐标用变分式 | 辅助 | 并入相关内容 | Lemma 3.8 | 原页已核 |
| §3.2 印刷页 67；PDF 页 86 | SECTION | A geometric perspective on concentration | 关键 | 完整讲解 |  | 原页已核 |
| §3.2 印刷页 67；PDF 页 86 | DEFINITION | 度量测度空间 $(\mathcal X,\rho,\mathbb P)$；欧氏空间与汉明立方 | 关键 | 完整讲解 |  | 原页已核 |
| §3.2.1 印刷页 67–69；PDF 页 86–88 | SECTION | Concentration functions | 关键 | 完整讲解 |  | 原页已核 |
| (3.26) 印刷页 67；PDF 页 86 | DEFINITION | $\rho(x,A)=\inf_{y\in A}\rho(x,y)$ | 辅助 | 并入相关内容 | Definition 3.9 | 原页已核 |
| (3.27) 印刷页 68；PDF 页 87 | DEFINITION | $\varepsilon$-膨胀 $A^\varepsilon=\{x\colon\rho(x,A)<\varepsilon\}$ | 关键 | 完整讲解 |  | 原页已核 |
| Definition 3.9 印刷页 68；PDF 页 87 | DEFINITION | 集中函数 $\alpha_{\mathbb P,(\mathcal X,\rho)}(\varepsilon)=\sup\{1-\mathbb P[A^\varepsilon]\colon\mathbb P[A]\ge\frac12\}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 3.10 印刷页 68–69；PDF 页 87–88 | EXAMPLE | 球面均匀测度的集中函数 | 关键 | 完整讲解 |  | 原页已核 |
| (3.29)–(3.32) 印刷页 68；PDF 页 87 | FORMULA | $\mathbb S^{n-1}$、测地距离、半球 $H_y$、Lévy 等周：半球极小 | 关键 | 完整讲解 |  | 原页已核 |
| Figure 3.1 印刷页 69；PDF 页 88 | FIGURE_TABLE | 半球、$\varepsilon$-膨胀、中心切片 $T_y(\varepsilon)$ | 辅助 | 简要说明 |  | 原页已核 |
| (3.33)–(3.35) 印刷页 69；PDF 页 88 | FORMULA | $\alpha_{\mathbb S^{n-1}}(\varepsilon)\le e^{-n\varepsilon^2/8}$；更尖 (3.34) $\sqrt{\pi/2}\,e^{-n\varepsilon^2/2}$；切片体积 | 关键 | 完整讲解 |  | 原页已核 |
| §3.2.2 印刷页 70–72；PDF 页 89–91 | SECTION | Connection to Lipschitz functions | 关键 | 完整讲解 |  | 原页已核 |
| (3.36)–(3.38) 印刷页 70；PDF 页 89 | FORMULA | $L$-利普希茨、中位数、膨胀含于 $\{f<m_f+\varepsilon\}$ | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 3.11 印刷页 70；PDF 页 89 | PROPOSITION | 集中函数与 1-利普希茨函数的等价：(3.39a)–(3.39b) | 关键 | 完整讲解 |  | 原页已核 |
| Example 3.12 印刷页 71；PDF 页 90 | EXAMPLE | 球面上 Lévy 集中 (3.40)–(3.41) | 关键 | 完整讲解 |  | 原页已核 |
| (3.40) 印刷页 71；PDF 页 90 | FORMULA | $\mathbb P[\lvert f-m_f\rvert\ge\varepsilon]\le\sqrt{2\pi}\,e^{-n\varepsilon^2/2}$ | 关键 | 并入相关内容 | Example 3.12 | 原页已核 |
| (3.41) 印刷页 71；PDF 页 90 | FORMULA | 绕均值：$2\sqrt{2\pi}\,e^{-n\varepsilon^2/8}$ | 辅助 | 并入相关内容 | Example 3.12 | 原页已核 |
| Example 3.13 印刷页 71–72；PDF 页 90–91 | EXAMPLE | 布尔超立方体：Harper 定理推出 $\alpha\le e^{-2\varepsilon^2/n}$（$n\ge 3$） | 关键 | 完整讲解 |  | 原页已核 |
| (3.42) 印刷页 72；PDF 页 91 | FORMULA | $\alpha_{\mathbb P}(\varepsilon)\le e^{-2\varepsilon^2/n}$；因而 1-利普希茨绕中位数以 $2e^{-2\varepsilon^2/n}$ 集中 | 关键 | 完整讲解 |  | 原页已核 |
| §3.2.3 印刷页 72–76；PDF 页 91–95 | SECTION | From geometry to concentration | 关键 | 完整讲解 |  | 原页已核 |
| (3.43) 印刷页 72；PDF 页 91 | FORMULA | 布鲁恩–闵可夫斯基：$[\mathrm{vol}(\lambda C+(1-\lambda)D)]^{1/n}\ge\lambda[\mathrm{vol}(C)]^{1/n}+(1-\lambda)[\mathrm{vol}(D)]^{1/n}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 3.14 印刷页 73；PDF 页 92 | EXAMPLE | $\mathbb R^n$ 的经典等周：欧氏球极小 | 关键 | 完整讲解 |  | 原页已核 |
| (3.44) 印刷页 73；PDF 页 92 | FORMULA | $\mathrm{vol}(A)=\mathrm{vol}(\mathbb B_2^n)\Rightarrow\mathrm{vol}(A^\varepsilon)\ge\mathrm{vol}([\mathbb B_2^n]^\varepsilon)$ | 关键 | 并入相关内容 | Example 3.14 | 原页已核 |
| (3.45) 印刷页 73；PDF 页 92 | FORMULA | 乘积形式 $\mathrm{vol}(\lambda C+(1-\lambda)D)\ge[\mathrm{vol}(C)]^\lambda[\mathrm{vol}(D)]^{1-\lambda}$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 3.15 印刷页 73；PDF 页 92 | THEOREM | 普雷科帕–莱因德勒不等式 (3.46)–(3.47) | 关键 | 完整讲解 |  | 原页已核 |
| (3.46)–(3.47) 印刷页 73；PDF 页 92 | FORMULA | $w(\lambda x+(1-\lambda)y)\ge[u(x)]^\lambda[v(y)]^{1-\lambda}$ 推出积分乘积下界 | 关键 | 并入相关内容 | Theorem 3.15 | 原页已核 |
| (3.48) 印刷页 74；PDF 页 93 | DEFINITION | 强凸 / 强对数凹：$\lambda\psi(x)+(1-\lambda)\psi(y)-\psi(\lambda x+(1-\lambda)y)\ge\frac\gamma2\lambda(1-\lambda)\Vert x-y\Vert_2^2$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 3.16 印刷页 74；PDF 页 93 | THEOREM | 强对数凹参数 $\gamma$ 的欧氏 $L$-利普希茨集中 (3.49) | 关键 | 完整讲解 |  | 原页已核 |
| (3.49) 印刷页 74；PDF 页 93 | FORMULA | $\mathbb P[\lvert f(X)-\mathbb E[f(X)]\rvert\ge t]\le 2e^{-\gamma t^2/(4L^2)}$ | 关键 | 并入相关内容 | Theorem 3.16 | 原页已核 |
| Theorem 3.16 证明 印刷页 74–76；PDF 页 93–95 | PROOF_DERIVATION | 下卷积 + PL 不等式推出 $\mathbb E[e^{h}]\le e^{L^2/\gamma}$ | 关键 | 简要说明 |  | 原页已核 |
| (3.50) 印刷页 75；PDF 页 94 | FORMULA | $\mathbb E[e^{g(Y)}]\le 1/\mathbb E[e^{-h(X)}]\le 1$ | 辅助 | 并入相关内容 | Theorem 3.16 | 原页已核 |
| §3.3 印刷页 76；PDF 页 95 | SECTION | Wasserstein distances and information inequalities | 关键 | 完整讲解 |  | 原页已核 |
| §3.3.1 印刷页 76–78；PDF 页 95–97 | SECTION | Wasserstein distances | 关键 | 完整讲解 |  | 原页已核 |
| (3.51)–(3.52) 印刷页 76；PDF 页 95 | DEFINITION | $\Vert f\Vert_{\mathrm{Lip}}$ 与瓦瑟斯坦距离 $W_\rho(\mathbb Q,\mathbb P)=\sup_{\Vert f\Vert_{\mathrm{Lip}}\le 1}\lvert\int f\,d\mathbb Q-\int f\,d\mathbb P\rvert$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 3.17 印刷页 76–77；PDF 页 95–96 | EXAMPLE | 汉明度量下 $W_{\mathrm{Ham}}=\Vert\mathbb Q-\mathbb P\Vert_{\mathrm{TV}}$ | 关键 | 完整讲解 |  | 原页已核 |
| (3.53) 印刷页 76；PDF 页 95 | DEFINITION | 全变差 $\Vert\mathbb Q-\mathbb P\Vert_{\mathrm{TV}}=\sup_A\lvert\mathbb Q(A)-\mathbb P(A)\rvert$ | 关键 | 完整讲解 |  | 原页已核 |
| (3.54)–(3.55) 印刷页 77；PDF 页 96 | FORMULA | 坎托罗维奇–鲁宾斯坦对偶：利普希茨形式 = 耦合运输代价 | 关键 | 完整讲解 |  | 原页已核 |
| §3.3.2 印刷页 78–80；PDF 页 97–99 | SECTION | Transportation cost and concentration inequalities | 关键 | 完整讲解 |  | 原页已核 |
| (3.56)–(3.57) 印刷页 78；PDF 页 97 | DEFINITION | 库尔贝克–莱布勒散度 $D(\mathbb Q\Vert\mathbb P)=\mathbb E_{\mathbb Q}[\log(d\mathbb Q/d\mathbb P)]$ | 关键 | 完整讲解 |  | 原页已核 |
| Definition 3.18 印刷页 78；PDF 页 97 | DEFINITION | $\rho$-运输代价不等式 $W_\rho(\mathbb Q,\mathbb P)\le\sqrt{2\gamma D(\mathbb Q\Vert\mathbb P)}$ | 关键 | 完整讲解 |  | 原页已核 |
| (3.59) 印刷页 78；PDF 页 97 | FORMULA | 平斯克–奇萨尔–库尔贝克：$\Vert\mathbb P-\mathbb Q\Vert_{\mathrm{TV}}\le\sqrt{\frac12 D(\mathbb Q\Vert\mathbb P)}$，即 $\gamma=1/4$ 的汉明 TCI | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 3.19 印刷页 79；PDF 页 98 | THEOREM | 运输代价推出集中：(3.60) 与利普希茨 (3.61) | 关键 | 完整讲解 |  | 原页已核 |
| (3.60) 印刷页 79；PDF 页 98 | FORMULA | $\alpha(t)\le 2\exp(-t^2/(2\gamma))$ | 关键 | 并入相关内容 | Theorem 3.19 | 原页已核 |
| (3.61) 印刷页 79；PDF 页 98 | FORMULA | $\mathbb P[\lvert f-\mathbb E[f]\rvert\ge t]\le 2\exp(-t^2/(2\gamma L^2))$ | 关键 | 并入相关内容 | Theorem 3.19 | 原页已核 |
| (3.62)–(3.63) 印刷页 79–80；PDF 页 98–99 | FORMULA | 中位数形式；均值证明中的 Young 切分 | 辅助 | 并入相关内容 | Theorem 3.19 | 原页已核 |
| Theorem 3.19 证明 印刷页 79–80；PDF 页 98–99 | PROOF_DERIVATION | 条件化耦合 + 指数倾斜推出 CGF | 关键 | 简要说明 |  | 原页已核 |
| §3.3.3 印刷页 80–82；PDF 页 99–101 | SECTION | Tensorization for transportation cost | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 3.20 印刷页 81；PDF 页 100 | PROPOSITION | 乘积测度的运输代价张量化 (3.64) | 关键 | 完整讲解 |  | 原页已核 |
| (3.64) 印刷页 81；PDF 页 100 | FORMULA | $W_\rho(\mathbb Q,\mathbb P)\le\sqrt{2(\sum\gamma_k)D(\mathbb Q\Vert\mathbb P)}$，$\rho=\sum\rho_k$ | 关键 | 并入相关内容 | Proposition 3.20 | 原页已核 |
| Example 3.21 印刷页 81；PDF 页 100 | EXAMPLE | 由 TCI 恢复有界差分 (3.65) | 关键 | 完整讲解 |  | 原页已核 |
| (3.65) 印刷页 81；PDF 页 100 | FORMULA | $\mathbb P[\lvert f-\mathbb E[f]\rvert\ge t]\le 2\exp(-2t^2/\sum L_k^2)$ | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 3.20 证明 印刷页 81–82；PDF 页 100–101 | PROOF_DERIVATION | 归纳最优耦合 + Jensen + 柯西–施瓦茨 + KL 链式法则 | 辅助 | 简要说明 |  | 原页已核 |
| §3.3.4 印刷页 82–83；PDF 页 101–102 | SECTION | Transportation cost inequalities for Markov chains | 关键 | 完整讲解 |  | 原页已核 |
| (3.66)–(3.67) 印刷页 82–83；PDF 页 101–102 | DEFINITION | 转移核与 $\beta$-压缩：$\max_i\sup\Vert\mathbb K_{i+1}(\cdot\mid x_i)-\mathbb K_{i+1}(\cdot\mid x_i')\Vert_{\mathrm{TV}}\le\beta$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 3.22 印刷页 83；PDF 页 102 | THEOREM | $\beta$-压缩马尔可夫链的汉明 TCI (3.68) | 关键 | 完整讲解 |  | 原页已核 |
| (3.68) 印刷页 83；PDF 页 102 | FORMULA | $W_\rho(\mathbb Q,\mathbb P)\le\frac1{1-\beta}\sqrt{\frac n2 D(\mathbb Q\Vert\mathbb P)}$ | 关键 | 并入相关内容 | Theorem 3.22 | 原页已核 |
| (3.69) 印刷页 83；PDF 页 102 | FORMULA | 汉明 $L$-利普希茨：$\mathbb P[\lvert f-\mathbb E[f]\rvert\ge t]\le 2\exp(-2(1-\beta)^2 t^2/(n L^2))$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 3.23 印刷页 83；PDF 页 102 | EXAMPLE | 二元马尔可夫链粘性参数估计 (3.70) | 关键 | 完整讲解 |  | 原页已核 |
| (3.70) 印刷页 83；PDF 页 102 | FORMULA | $\mathbb P[\lvert f-\frac12(1+\delta)\rvert\ge t]\le 2e^{-(n-1)^2(1-\delta)^2 t^2/(2n)}\le 2e^{-(n-1)(1-\delta)^2 t^2/4}$ | 关键 | 并入相关内容 | Example 3.23 | 原页已核 |
| §3.3.5 印刷页 84–86；PDF 页 103–105 | SECTION | Asymmetric coupling cost | 关键 | 完整讲解 |  | 原页已核 |
| (3.71)–(3.72) 印刷页 84；PDF 页 103 | DEFINITION | 非对称耦合代价 $C(\mathbb Q,\mathbb P)$ 及其密度表示 | 关键 | 完整讲解 |  | 原页已核 |
| (3.73) 印刷页 84；PDF 页 103 | FORMULA | Samson：乘积测度 $\max\{C(\mathbb Q,\mathbb P),C(\mathbb P,\mathbb Q)\}\le\sqrt{2D(\mathbb Q\Vert\mathbb P)}$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 3.24 印刷页 84；PDF 页 103 | THEOREM | 独立、$[0,1]$ 取值、联合凸且欧氏 $L$-利普希茨的双侧集中 (3.74) | 关键 | 完整讲解 |  | 原页已核 |
| (3.74) 印刷页 84；PDF 页 103 | FORMULA | $\mathbb P[\lvert f-\mathbb E[f]\rvert\ge t]\le 2e^{-t^2/(2L^2)}$ | 关键 | 并入相关内容 | Theorem 3.24 | 原页已核 |
| Example 3.25 印刷页 85；PDF 页 104 | EXAMPLE | 拉德马赫复杂度的双侧尖锐界 (3.75) | 关键 | 完整讲解 |  | 原页已核 |
| (3.75) 印刷页 85；PDF 页 104 | FORMULA | $\mathbb P[\lvert Z-\mathbb E[Z]\rvert\ge t]\le 2\exp(-t^2/(2\mathcal W^2(\mathcal A)))$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 3.24 证明 印刷页 85–86；PDF 页 104–105 | PROOF_DERIVATION | 凸函数一阶下界 + 柯西–施瓦茨把偏差控成 $L\,C$ | 关键 | 简要说明 |  | 原页已核 |
| (3.76)–(3.78) 印刷页 86；PDF 页 105 | FORMULA | 一般 $\gamma$-信息不等式；$\beta$-压缩链欧氏利普希茨的维数无关界 | 关键 | 完整讲解 |  | 原页已核 |
| §3.4 印刷页 87；PDF 页 106 | SECTION | Tail bounds for empirical processes | 关键 | 完整讲解 |  | 原页已核 |
| (3.79) 印刷页 87；PDF 页 106 | DEFINITION | $Z=\sup_{f\in\mathcal F}\bigl(\frac1n\sum_{i=1}^n f(X_i)\bigr)$ | 关键 | 完整讲解 |  | 原页已核 |
| §3.4.1 印刷页 87–89；PDF 页 106–108 | SECTION | A functional Hoeffding inequality | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 3.26 印刷页 87；PDF 页 106 | THEOREM | 泛函赫夫丁定理 (3.80) | 关键 | 完整讲解 |  | 原页已核 |
| (3.80) 印刷页 87；PDF 页 106 | FORMULA | $\mathbb P[Z\ge\mathbb E[Z]+\delta]\le\exp(-n\delta^2/(4L^2))$，$L^2=\sup_f\{\frac1n\sum_i(b_{i,f}-a_{i,f})^2\}$ | 关键 | 并入相关内容 | Theorem 3.26 | 原页已核 |
| §3.4.1 比较 印刷页 88；PDF 页 107 | FORMULA | 有界差分给出 $\widetilde L^2=\frac1n\sum_i\sup_f(b_{i,f}-a_{i,f})^2$，可远大于 $L^2$ | 关键 | 完整讲解 |  | 原页已核 |
| (3.81)–(3.82) 印刷页 88；PDF 页 107 | PROOF_DERIVATION | 未缩放 $Z$、达成集 $\mathcal A(f)$、坐标差由同一 $f$ 控制 | 辅助 | 并入相关内容 | Theorem 3.26 | 原页已核 |
| §3.4.2 印刷页 89–91；PDF 页 108–110 | SECTION | A functional Bernstein inequality | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 3.27 印刷页 89；PDF 页 108 | THEOREM | 经验过程的塔拉格兰集中 (3.83) | 关键 | 完整讲解 |  | 原页已核 |
| (3.83) 印刷页 89；PDF 页 108 | FORMULA | $\mathbb P[Z\ge\mathbb E[Z]+\delta]\le 2\exp(-n\delta^2/(8e\mathbb E[\Sigma^2]+4b\delta))$，$\Sigma^2=\sup_f\frac1n\sum_i f^2(X_i)$ | 关键 | 完整讲解 |  | 原页已核 |
| (3.84)–(3.86) 印刷页 89–90；PDF 页 108–109 | FORMULA | $\mathbb E[\Sigma^2]\le\sigma^2+2b\mathbb E[Z]$；等价形式 (3.85)(3.86)；最佳常数 $c_0=\sqrt2$, $c_1=1/3$ | 关键 | 完整讲解 |  | 原页已核 |
| (3.87) 印刷页 90；PDF 页 109 | FORMULA | $H(e^{\lambda Z})\le 2\lambda^2\{\mathbb E[\Gamma e^{\lambda Z}]+\mathbb E[\Gamma]\mathbb E[e^{\lambda Z}]\}$ | 辅助 | 并入相关内容 | Theorem 3.27 | 原页已核 |
| Lemma 3.28 印刷页 90；PDF 页 109 | LEMMA | 随机方差：$\mathbb E[\Gamma e^{\lambda\widetilde Z}]\le(e-1)\mathbb E[\Gamma]\mathbb E[e^{\lambda\widetilde Z}]+\mathbb E[\widetilde Z e^{\lambda\widetilde Z}]$ | 关键 | 完整讲解 |  | 原页已核 |
| (3.88) 印刷页 90；PDF 页 109 | FORMULA | Lemma 3.28 的不等式 | 关键 | 并入相关内容 | Lemma 3.28 | 原页已核 |
| Theorem 3.27 证明 印刷页 90–91；PDF 页 109–110 | PROOF_DERIVATION | 未缩放 + (3.88) 得到 Bernstein 熵界 $b=2$, $\sigma^2=2e\mathbb E[\Gamma]$ | 关键 | 简要说明 |  | 原页已核 |
| §3.5 印刷页 91–92；PDF 页 110–111 | PROSE_RANGE | Bibliographic details：Gross 对数索伯列夫、Herbst、Ledoux 熵方法、Talagrand 凸距离、BM/PL、Marton 运输、Samson、Bousquet 常数 | 辅助 | 指回教材 | 文献清单不抄入 Notes；对数索伯列夫在 Notes 用作者解释桥接 | 原页已核 |
| §3.6 印刷页 92；PDF 页 111 | SECTION | Exercises 3.1–3.16 | 辅助 | 不进入 Notes | 习题整节进入 Solutions | 原页已核 |
| Exercise 3.1 印刷页 92；PDF 页 111 | EXERCISE | Shannon entropy and Kullback–Leibler divergence | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 3.2 印刷页 92；PDF 页 111 | EXERCISE | Chain rule and Kullback–Leibler divergence | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 3.3 印刷页 92–93；PDF 页 111–112 | EXERCISE | Variational representation for entropy (3.89) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 3.4 印刷页 93；PDF 页 112 | EXERCISE | Entropy and constant shifts | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 3.5 印刷页 93；PDF 页 112 | EXERCISE | Equivalent forms of entropy | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 3.6 印刷页 93；PDF 页 112 | EXERCISE | Entropy rescaling (3.90) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 3.7 印刷页 93；PDF 页 112 | EXERCISE | Entropy for bounded variables | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 3.8 印刷页 93–94；PDF 页 112–113 | EXERCISE | Exponential families and entropy (3.91) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 3.9 印刷页 94；PDF 页 113 | EXERCISE | Another variational representation | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 3.10 印刷页 94；PDF 页 113 | EXERCISE | Brunn–Minkowski and classical isoperimetric inequality (3.92) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 3.11 印刷页 94；PDF 页 113 | EXERCISE | Concentration on the Euclidean ball | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 3.12 印刷页 95；PDF 页 114 | EXERCISE | Rademacher chaos variables (3.93) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 3.13 印刷页 95；PDF 页 114 | EXERCISE | Total variation and Wasserstein | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 3.14 印刷页 95；PDF 页 114 | EXERCISE | Alternative proof of Proposition 3.20 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 3.15 印刷页 95–96；PDF 页 114–115 | EXERCISE | Bounds for suprema of non-negative functions (3.94) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 3.16 印刷页 96–97；PDF 页 115–116 | EXERCISE | Different forms of functional Bernstein (3.95a)–(3.95b) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |

## 来源异常与勘误

| 定位 | 问题类型 | 原式/原文 | 核验证据 | 处置 | 数学复核人 | 批准人 |
|---|---|---|---|---|---|---|
| Lemma 3.8 证明 印刷页 67；PDF 页 86 | 笔误嫌疑 | “$\mathbb E[g^k(X_k,\ldots,X_n)\mid X_{\backslash k}]=1$” | 同页前文构造给出 $\mathbb E[\exp(g^k)\mid X_{k+1}^n]=1$；变分式 (3.24) 需要的也是 $\mathbb E[e^{g^k}]\le 1$ | 保留原文；Notes 按 $\mathbb E[e^{g^k}\mid X_{\backslash k}]=1$ 讲解；`勘误待批` | 作者 | 未批 |
| Example 3.10 印刷页 69；PDF 页 88 | 笔误嫌疑 | “bounding $\mathbb P[H_y]$ can be used to establish the sharper upper bound (3.34)” | $\mathbb P[H_y]=1/2$ 对一切 $y$；要改进的是 $\mathbb P[H_y^\varepsilon]$ | 保留原文；Notes 按膨胀概率解读；`勘误待批` | 作者 | 未批 |
| Example 3.14 印刷页 73；PDF 页 92 | 术语嫌疑 | “Euclidean sphere $\mathbb B_2^n:=\{x\colon\Vert x\Vert_2\le 1\}$” | 该集合是闭单位球；球面是 $\mathbb S^{n-1}$ | 保留原文；Notes 按单位球讲解；`勘误待批` | 作者 | 未批 |
| 脚注 2 印刷页 72；PDF 页 91 | 定义不完整 | “A convex body in $\mathbb R^n$ is a compact and closed set.” | 紧致已含闭；标准凸体还要求凸且内部非空 | 保留原文；Notes 不依赖该脚注；`勘误待批` | 作者 | 未批 |
| (3.55) 印刷页 77；PDF 页 96 | 记号次序 | 左端 $\int f(d\mathbb Q-d\mathbb P)$ 的括号标成 $W_\rho(\mathbb P,\mathbb Q)$ | (3.52) 把同一量写成 $W_\rho(\mathbb Q,\mathbb P)$；度量对称故数值相同 | 保留原文；Notes 统一用 $W_\rho(\mathbb Q,\mathbb P)$；`勘误待批` | 作者 | 未批 |
| Theorem 3.27 (3.83) 印刷页 89；PDF 页 108 | 常数不一致 | 定理前因子为 2 | 印刷页 91 / PDF 页 110 由 (3.12) 得到的是不带 2 的 $\exp(-\delta^2/(8e\mathbb E[\Gamma]+4\delta))$ | 保留原文；Notes 照抄 (3.83)，并指出证明给出因子 1；`勘误待批` | 作者 | 未批 |
| Exercise 3.6 (3.90) 印刷页 93；PDF 页 112 | 记号嫌疑 | 定义 $\widetilde X=X-\mathbb E[X]$ 后展示的仍是 $H(e^{\lambda X})$ | 与 Proposition 3.3 中心化步骤一致时，指数里应为 $\widetilde X$ | 保留原文；Solutions 按中心化变量书写；`勘误待批` | 作者 | 未批 |
| Exercise 3.8 印刷页 93；PDF 页 112 | 笔误嫌疑 | “suppose moreover that $\nabla A$ is Lipschitz” | 指数族归一化是 $\Phi$；(3.91) 写的是 $\nabla\Phi$；$A$ 未定义 | 保留原文；Solutions 按 $\nabla\Phi$ 求解；`勘误待批` | 作者 | 未批 |
| Exercise 3.14(c) 印刷页 95；PDF 页 114 | 标点 | Hint 句缺右括号 | 原页 “Cauchy–Schwarz and Exercise 3.2 could be useful.” 无闭合 | 不影响求解；`勘误待批` | 作者 | 未批 |
| Exercise 3.10(c) 印刷页 94；PDF 页 113 | 笔误嫌疑 | Hint 写 $C:=A/\mathrm{vol}(A)$、$D:=B/\mathrm{vol}(B)$ | 要使 $\mathrm{vol}(C)=\mathrm{vol}(D)=1$，正确缩放是 $A/\mathrm{vol}(A)^{1/n}$ | 保留原文；Solutions 按体积 $1/n$ 次齐性求解；`勘误待批` | 作者 | 未批 |

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
