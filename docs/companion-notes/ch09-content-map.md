---
chapter_id: "ch09"
chapter_title: "Decomposability and restricted strong convexity"
source_title: "High-Dimensional Statistics: A Non-Asymptotic Viewpoint"
source_version: "Cambridge Series in Statistical and Probabilistic Mathematics, No. 48; first published 2019; ISBN 978-1-108-49802-9"
main_source_path: "High-Dimensional Statistics A Non-Asymptotic Viewpoint (Martin J. Wainwright) (z-library.sk, 1lib.sk, z-lib.sk).pdf"
printed_pages: "259–311"
pdf_pages: "278–330"
target_notes: "notes/ch09-notes.qmd"
language: "zh-CN"
learner_profile: "学过陈希孺《概率论与数理统计》本科教材；熟悉极大似然、Fisher 信息与凸性的微积分表述；第 7 章已见 ℓ₁ 与限制特征值。首次需要把套索提升为一般正则化 M 估计，并用可分解正则、限制强凸、组套索与重叠组把误差锥写清楚。"
map_status: "清单完成"
---

# 第 9 章内容清单

> 内部质量工件。正式内容逐项登记；例子与连续公式在处理方式相同时才聚合。习题全部进 Solutions，不进 Notes。

## 来源边界

- 教材权威来源：Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series No. 48
- 版本识别依据：封面 Cambridge Series；版权页 © Martin J. Wainwright 2019，First published 2019，ISBN 978-1-108-49802-9 Hardback，DOI 10.1017/9781108627771
- 目标章节与页码：第 9 章，印刷页 259–311；PDF 页 278–330（**PDF = 印刷 + 19**）
- 补充来源及用途：无（§9.11 独立求解）
- 已知来源限制：文本层可用但公式常错位；公式、图注、定理框须对照 `scratch/ch09/p-2XX.png` 与 `p-3XX.png`

## 内容清单

| 定位 | 类型 | 内容/范围 | 重要性 | Notes 处理 | 合并目标/排除理由 | 核验状态 |
|---|---|---|---|---|---|---|
| 章首 印刷页 259；PDF 页 278 | SECTION | Chapter 9：由第 7 章稀疏线性模型升到正则化 M 估计；两件套：可分解正则与代价的限制曲率 | 关键 | 完整讲解 |  | 原页已核 |
| §9.1 印刷页 259–268；PDF 页 278–287 | SECTION | A general regularized M-estimator | 关键 | 完整讲解 |  | 原页已核 |
| (9.1) 印刷页 259；PDF 页 278 | FORMULA | 总体代价 $\overline{\mathcal L}(\theta)=\mathbb E[\mathcal L_n(\theta;Z_1^n)]$ | 关键 | 完整讲解 |  | 原页已核 |
| (9.2) 印刷页 260；PDF 页 279 | FORMULA | 目标参数 $\theta^*=\arg\min_{\theta\in\Omega}\overline{\mathcal L}(\theta)$；允许误指定 | 关键 | 完整讲解 |  | 原页已核 |
| (9.3) 印刷页 260；PDF 页 279 | DEFINITION | 正则化 M 估计 $\widehat\theta\in\arg\min\{\mathcal L_n(\theta)+\lambda_n\Phi(\theta)\}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 9.1 印刷页 260–261；PDF 页 279–280 | EXAMPLE | 线性回归与套索；二次代价与总体二次型 | 关键 | 完整讲解 |  | 原页已核 |
| (9.4) 印刷页 261；PDF 页 280 | FORMULA | 套索作为 (9.3) 的特例 | 关键 | 完整讲解 |  | 原页已核 |
| Figure 9.1 印刷页 261；PDF 页 280 | FIGURE_TABLE | $\mathbb R^3$ 中 $\ell_1$、组套索、重叠组单位球 | 辅助 | 简要说明 |  | 原页已核 |
| Example 9.2 印刷页 261–262；PDF 页 280–281 | EXAMPLE | 广义线性模型与 $\ell_1$ 正则 | 关键 | 完整讲解 |  | 原页已核 |
| (9.5) 印刷页 261；PDF 页 280 | FORMULA | GLM 条件密度：尺度 $c(\sigma)$ 与配分 $\psi$ | 关键 | 完整讲解 |  | 原页已核 |
| (9.6)–(9.8) 印刷页 262；PDF 页 281 | FORMULA | 逻辑斯蒂对数优势；负对数似然 (9.7)；广义线性套索 (9.8) | 关键 | 完整讲解 |  | 原页已核 |
| Example 9.3 印刷页 262–263；PDF 页 281–282 | EXAMPLE | 不重叠组套索范数 (9.9)；标准组套索鼓励补集支撑 | 关键 | 完整讲解 |  | 原页已核 |
| (9.9) 印刷页 262；PDF 页 281 | FORMULA | $\Phi(\theta)=\sum_{g\in\mathcal G}\Vert\theta_g\Vert$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 9.2 印刷页 263；PDF 页 282 | FIGURE_TABLE | 标准组 vs 重叠组残差惩罚；重叠组单位球 | 辅助 | 简要说明 |  | 原页已核 |
| Figure 9.3 印刷页 264；PDF 页 283 | FIGURE_TABLE | (a) 不重叠划分；(b) 二叉树子树重叠组 | 辅助 | 简要说明 |  | 原页已核 |
| Example 9.4 印刷页 264–265；PDF 页 283–284 | EXAMPLE | 重叠组套索变分范数 (9.10)；诱导并支撑 | 关键 | 完整讲解 |  | 原页已核 |
| (9.10) 印刷页 264；PDF 页 283 | FORMULA | $\Phi_{\mathrm{over}}(\theta)=\inf_{\theta=\sum w_g}\sum\Vert w_g\Vert$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 9.5 印刷页 265；PDF 页 284 | EXAMPLE | 高斯图模型与图形套索 (9.11)–(9.12) | 辅助 | 简要说明 | 第 11 章展开 | 原页已核 |
| (9.11)–(9.12) 印刷页 265；PDF 页 284 | FORMULA | 精度矩阵密度；图形套索 | 辅助 | 简要说明 | 并入 Example 9.5 | 原页已核 |
| Example 9.6 印刷页 265–267；PDF 页 284–286 | EXAMPLE | 多元回归 $Y=Z\Theta^*+W$；行组套索 (9.13)–(9.14) | 关键 | 完整讲解 |  | 原页已核 |
| Figure 9.4 印刷页 266；PDF 页 285 | FIGURE_TABLE | 多元回归矩阵尺寸 | 辅助 | 简要说明 |  | 原页已核 |
| Example 9.7 印刷页 267；PDF 页 286 | EXAMPLE | 行稀疏加元素稀疏分解；(9.15)–(9.16) 重叠组 | 关键 | 完整讲解 |  | 原页已核 |
| Example 9.8 印刷页 267–268；PDF 页 286–287 | EXAMPLE | 核范数作为秩的凸松弛 | 辅助 | 简要说明 | 第 10 章展开 | 原页已核 |
| (9.17)–(9.19) 印刷页 268；PDF 页 287 | FORMULA | SVD、奇异值、核范数 $\Vert\Vert\vert\Theta\Vert\Vert\vert_{\mathrm{nuc}}=\sum\sigma_j$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 9.5 印刷页 268；PDF 页 287 | FIGURE_TABLE | 核范数球 vs 秩约束 / $\ell_q$ 球 | 辅助 | 简要说明 |  | 原页已核 |
| §9.2 印刷页 269–275；PDF 页 288–294 | SECTION | Decomposable regularizers and their utility | 关键 | 完整讲解 |  | 原页已核 |
| (9.20) 印刷页 269；PDF 页 288 | FORMULA | 子空间投影 $\theta_{\mathbb S}=\arg\min_{\widetilde\theta\in\mathbb S}\Vert\widetilde\theta-\theta\Vert^2$ | 关键 | 完整讲解 |  | 原页已核 |
| §9.2.1 印刷页 269–272；PDF 页 288–291 | SECTION | Definition and some examples | 关键 | 完整讲解 |  | 原页已核 |
| (9.21) 印刷页 269；PDF 页 288 | DEFINITION | 扰动子空间 $\overline{\mathbb M}^\perp=\{v:\langle u,v\rangle=0\ \forall u\in\overline{\mathbb M}\}$ | 关键 | 完整讲解 |  | 原页已核 |
| Definition 9.9 印刷页 269；PDF 页 288 | DEFINITION | 可分解正则：$\Phi(\alpha+\beta)=\Phi(\alpha)+\Phi(\beta)$，$\alpha\in\mathbb M$，$\beta\in\overline{\mathbb M}^\perp$ | 关键 | 完整讲解 |  | 原页已核 |
| (9.22) 印刷页 269；PDF 页 288 | FORMULA | 可分解恒等式 | 关键 | 并入相关内容 | Definition 9.9 | 原页已核 |
| Figure 9.6 印刷页 270；PDF 页 289 | FIGURE_TABLE | 理想情形 $\mathbb M=\overline{\mathbb M}$ 的正交分解几何 | 辅助 | 简要说明 |  | 原页已核 |
| Example 9.10 印刷页 270；PDF 页 289 | EXAMPLE | $\ell_1$ 对支撑子空间 $(\mathbb M(S),\mathbb M^\perp(S))$ 可分解；(9.23) | 关键 | 完整讲解 |  | 原页已核 |
| Example 9.11 印刷页 270–271；PDF 页 289–290 | EXAMPLE | 不重叠组范数对 $(\mathbb M(S_{\mathcal G}),\mathbb M^\perp(S_{\mathcal G}))$ 可分解；(9.24) | 关键 | 完整讲解 |  | 原页已核 |
| (9.25) 印刷页 271；PDF 页 290 | FORMULA | 重叠时普通组范数破坏可分解：$4>2+\sqrt{2}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 9.12 印刷页 271–272；PDF 页 290–291 | EXAMPLE | 重叠组：放大 $\widetilde S_{\mathcal G}$ 后对 $(\mathbb M(S_{\mathcal G}),\mathbb M^\perp(\widetilde S_{\mathcal G}))$ 可分解；(9.26) | 关键 | 完整讲解 |  | 原页已核 |
| §9.2.2 印刷页 272–275；PDF 页 291–294 | SECTION | A key consequence of decomposability | 关键 | 完整讲解 |  | 原页已核 |
| (9.27) 印刷页 272；PDF 页 291 | DEFINITION | 对偶范数 $\Phi^*(v)=\sup_{\Phi(u)\le 1}\langle u,v\rangle$ | 关键 | 完整讲解 |  | 原页已核 |
| Table 9.1 印刷页 273；PDF 页 292 | FIGURE_TABLE | 原–对偶正则对：$\ell_1/\ell_\infty$、组、核范数、重叠组、稀疏–低秩 | 关键 | 完整讲解 |  | 原页已核 |
| (9.28) 印刷页 273；PDF 页 292 | DEFINITION | 好事件 $\mathbb G(\lambda_n)=\{\Phi^*(\nabla\mathcal L_n(\theta^*))\le\lambda_n/2\}$ | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 9.13 印刷页 273；PDF 页 292 | PROPOSITION | 在 $\mathbb G(\lambda_n)$ 上误差落入 $C_{\theta^*}(\mathbb M,\overline{\mathbb M}^\perp)$ | 关键 | 完整讲解 |  | 原页已核 |
| (9.29)–(9.30) 印刷页 273–274；PDF 页 292–293 | FORMULA | 锥型约束集；$\theta^*\in\mathbb M$ 时 $\Phi(\widehat\Delta)\le 4\Phi(\widehat\Delta_{\overline{\mathbb M}})$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 9.7 印刷页 274；PDF 页 293 | FIGURE_TABLE | $C$ 在 $\theta^*\in\mathbb M$ 时为锥，否则为星形 | 辅助 | 简要说明 |  | 原页已核 |
| (9.31) 印刷页 274；PDF 页 293 | FORMULA | 基本不等式函数 $\mathcal F(\Delta)$ | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 9.14 印刷页 275；PDF 页 294 | LEMMA | 偏差不等式 (9.32)–(9.33)：正则差与凸代价差 | 关键 | 完整讲解 |  | 原页已核 |
| (9.34) 印刷页 275；PDF 页 294 | PROOF_DERIVATION | 可分解 + 三角不等式推出 (9.32)；Hölder 推出 (9.33) | 关键 | 完整讲解 |  | 原页已核 |
| §9.3 印刷页 276–279；PDF 页 295–298 | SECTION | Restricted curvature conditions | 关键 | 完整讲解 |  | 原页已核 |
| (9.35) 印刷页 276；PDF 页 295 | FORMULA | 负对数似然；样本 Fisher 与 Cramér–Rao 动机 | 辅助 | 简要说明 |  | 原页已核 |
| Figure 9.8 印刷页 276；PDF 页 295 | FIGURE_TABLE | $d>n$ 时代价沿 $d-n$ 个方向二阶平坦 | 辅助 | 简要说明 |  | 原页已核 |
| §9.3.1 印刷页 277–279；PDF 页 296–298 | SECTION | Restricted strong convexity | 关键 | 完整讲解 |  | 原页已核 |
| (9.36)–(9.37) 印刷页 277；PDF 页 296 | FORMULA | 一阶 Taylor 余项 $\mathcal E_n$；局部 $\kappa$-强凸 | 关键 | 完整讲解 |  | 原页已核 |
| Definition 9.15 印刷页 277；PDF 页 296 | DEFINITION | RSC：$\mathcal E_n(\Delta)\ge(\kappa/2)\Vert\Delta\Vert^2-\tau_n^2\Phi^2(\Delta)$，$\Delta\in\mathbb B(R)$ | 关键 | 完整讲解 |  | 原页已核 |
| (9.38) 印刷页 277；PDF 页 296 | FORMULA | RSC 不等式 | 关键 | 并入相关内容 | Definition 9.15 | 原页已核 |
| Example 9.16 印刷页 278；PDF 页 297 | EXAMPLE | 最小二乘 RSC 即限制特征值；(9.39)；$\tau_n^2\asymp(\log d)/n$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 9.17 印刷页 278–279；PDF 页 297–298 | EXAMPLE | GLM 的 RSC；(9.40)–(9.42)；复杂度 $\mu_n(\Phi^*)$ | 关键 | 完整讲解 |  | 原页已核 |
| (9.41) 印刷页 278；PDF 页 297 | FORMULA | $\mu_n(\Phi^*)=\mathbb E[\Phi^*(n^{-1}\sum\varepsilon_i x_i)]$ | 关键 | 完整讲解 |  | 原页已核 |
| (9.43a)–(9.43b) 印刷页 279；PDF 页 298 | FORMULA | 组套索 $\mu_n\lesssim\sqrt{m/n}+\sqrt{(\log\lvert\mathcal G\rvert)/n}$；核范数 $\sqrt{d_1/n}+\sqrt{d_2/n}$ | 关键 | 完整讲解 |  | 原页已核 |
| Definition 9.18 印刷页 279；PDF 页 298 | DEFINITION | 子空间 Lipschitz 常数 $\Psi(\mathbb S)=\sup\Phi(u)/\Vert u\Vert$ | 关键 | 完整讲解 |  | 原页已核 |
| (9.44)–(9.45) 印刷页 279；PDF 页 298 | FORMULA | $\Psi$ 定义；锥上 $\Phi(\Delta)\le 4\Psi(\overline{\mathbb M})\Vert\Delta\Vert$；稀疏时 $\Psi=\sqrt{s}$ | 关键 | 完整讲解 |  | 原页已核 |
| §9.4 印刷页 279–286；PDF 页 298–305 | SECTION | Some general theorems | 关键 | 完整讲解 |  | 原页已核 |
| §9.4.1 印刷页 280–284；PDF 页 299–303 | SECTION | Guarantees under restricted strong convexity | 关键 | 完整讲解 |  | 原页已核 |
| (A1)(A2) 印刷页 280；PDF 页 299 | ASSUMPTION | 凸代价 + 局部 RSC；正则在 $(\mathbb M,\overline{\mathbb M}^\perp)$ 可分解 | 关键 | 完整讲解 |  | 原页已核 |
| (9.46)–(9.47) 印刷页 280；PDF 页 299 | FORMULA | 好事件；估计–逼近误差分解 $\varepsilon_n^2$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 9.19 印刷页 280；PDF 页 299 | THEOREM | 一般模型误差界 (9.48a)–(9.48b)；确定性神谕不等式 | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 9.20 印刷页 281；PDF 页 300 | COROLLARY | $\theta^*\in\mathbb M$ 时 $\Phi$ 界 $6(\lambda_n/\kappa)\Psi^2$，$\Vert\cdot\Vert^2$ 界 $9(\lambda_n^2/\kappa^2)\Psi^2$ | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 9.21 印刷页 282；PDF 页 301 | LEMMA | 若 $\mathcal F>0$ 于 $K(\delta)$ 则 $\Vert\widehat\Delta\Vert\le\delta$；星形 + Jensen | 关键 | 完整讲解 |  | 原页已核 |
| Figure 9.9 印刷页 282；PDF 页 301 | FIGURE_TABLE | 星形集与半径 $\delta$ 球面的交点 | 辅助 | 简要说明 |  | 原页已核 |
| (9.50)–(9.53) 印刷页 283–284；PDF 页 302–303 | PROOF_DERIVATION | Theorem 9.19(b) 证明：RSC、Hölder、$\Psi$、配平方得 $\varepsilon_n^2$ | 关键 | 简要说明 | 关键代数进 Notes，细节指回教材 | 原页已核 |
| §9.4.2 印刷页 284–286；PDF 页 303–305 | SECTION | Bounds under $\Phi^*$-curvature | 关键 | 完整讲解 |  | 原页已核 |
| (9.54) 印刷页 284；PDF 页 303 | FORMULA | 强凸的梯度形式 $\langle\nabla\mathcal L_n(\theta^*+\Delta)-\nabla\mathcal L_n(\theta^*),\Delta\rangle\ge\kappa\Vert\Delta\Vert^2$ | 关键 | 完整讲解 |  | 原页已核 |
| Definition 9.22 印刷页 284；PDF 页 303 | DEFINITION | $\Phi^*$ 范数曲率 (9.55) | 关键 | 完整讲解 |  | 原页已核 |
| Example 9.23 印刷页 284–285；PDF 页 303–304 | EXAMPLE | 最小二乘 $\ell_\infty$ 曲率 (9.56) 与 $\ell_\infty$-RE (9.57) | 关键 | 完整讲解 |  | 原页已核 |
| (A1') 印刷页 285；PDF 页 304 | ASSUMPTION | $\Phi^*$ 曲率参数 $(\kappa,\tau_n;R)$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 9.24 印刷页 285；PDF 页 304 | THEOREM | $\theta^*\in\mathbb M$ 且 $\tau_n\Psi^2<\kappa/32$ 时 $\Phi^*(\widehat\theta-\theta^*)\le 3\lambda_n/\kappa$ | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 9.25 印刷页 286；PDF 页 305 | LEMMA | $\theta^*\in\mathbb M$ 时锥上 $\Phi(\Delta)\le 16\Psi^2(\overline{\mathbb M})\Phi^*(\Delta)$ | 关键 | 完整讲解 |  | 原页已核 |
| (9.59)–(9.60) 印刷页 286；PDF 页 305 | FORMULA | 最优性 + 次梯度对偶有界得 (9.59)；引理 (9.60) | 关键 | 并入相关内容 | Theorem 9.24 与 Lemma 9.25 | 原页已核 |
| §9.5 印刷页 286–289；PDF 页 305–308 | SECTION | Bounds for sparse vector regression | 关键 | 完整讲解 |  | 原页已核 |
| §9.5.1 印刷页 286–287；PDF 页 305–306 | SECTION | GLM with sparsity；(G1) 列标准化；(G2) $\Vert\psi''\Vert_\infty\le B^2$ | 关键 | 完整讲解 |  | 原页已核 |
| (G1)(G2) 印刷页 287；PDF 页 306 | ASSUMPTION | 列标准化常数 $C$；配分二阶导数有界 | 关键 | 完整讲解 |  | 原页已核 |
| (9.61) 印刷页 287；PDF 页 306 | FORMULA | GLM 套索 | 关键 | 完整讲解 |  | 原页已核 |
| §9.5.2 印刷页 287–288；PDF 页 306–307 | SECTION | Bounds under RSC | 关键 | 完整讲解 |  | 原页已核 |
| (9.62) 印刷页 287；PDF 页 306 | FORMULA | GLM 的 $\ell_1$-RSC | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 9.26 印刷页 287；PDF 页 306 | COROLLARY | $s$-稀疏 GLM 套索：$\Vert\cdot\Vert_2^2\le(9/4)s\lambda_n^2/\kappa^2$，$\Vert\cdot\Vert_1\le(6/\kappa)s\lambda_n$ | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 9.26 证明 印刷页 288；PDF 页 307 | PROOF_DERIVATION | 用 Corollary 9.20；得分次高斯参数 $BC/\sqrt n$；$\lambda_n=4BC\{\sqrt{(\log d)/n}+\delta\}$ | 关键 | 简要说明 | 尾界步骤进 Notes | 原页已核 |
| §9.5.3 印刷页 288–289；PDF 页 307–308 | SECTION | Bounds under $\ell_\infty$-curvature | 关键 | 完整讲解 |  | 原页已核 |
| (9.64) 印刷页 289；PDF 页 308 | FORMULA | GLM 的 $\ell_\infty$ 曲率 | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 9.27 印刷页 289；PDF 页 308 | COROLLARY | $n>c_0^2 s^2\log d$ 时 $\Vert\widehat\theta-\theta^*\Vert_\infty\le 3\lambda_n/\kappa$ | 关键 | 完整讲解 |  | 原页已核 |
| §9.6 印刷页 290–292；PDF 页 309–311 | SECTION | Bounds for group-structured sparsity | 关键 | 完整讲解 |  | 原页已核 |
| (9.66) 印刷页 290；PDF 页 309 | FORMULA | 组 GLM 套索 | 关键 | 完整讲解 |  | 原页已核 |
| (G1') 印刷页 290；PDF 页 309 | ASSUMPTION | 组标准化 $\max_g\Vert\Vert\vert X_g\Vert\Vert\vert_2/\sqrt n\le C$ | 关键 | 完整讲解 |  | 原页已核 |
| (9.67) 印刷页 290；PDF 页 309 | FORMULA | 组 RSC：容差 $m/n+(\log\lvert\mathcal G\rvert)/n$ | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 9.28 印刷页 290；PDF 页 309 | COROLLARY | 组支撑 $S_{\mathcal G}$：$\Vert\cdot\Vert_2^2\le(9/4)\lvert S_{\mathcal G}\rvert\lambda_n^2/\kappa^2$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 9.29 印刷页 291；PDF 页 310 | EXAMPLE | 多元回归：元素 $\ell_1$ 率 (9.69a) vs 组率 (9.69b) | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 9.28 证明 印刷页 291–292；PDF 页 310–311 | PROOF_DERIVATION | $\Psi=\sqrt{\lvert S_{\mathcal G}\rvert}$；球面 $1/2$-覆盖与次高斯尾 | 辅助 | 简要说明 |  | 原页已核 |
| §9.7 印刷页 293–296；PDF 页 312–315 | SECTION | Bounds for overlapping decomposition-based norms | 关键 | 完整讲解 |  | 原页已核 |
| Example 9.30 印刷页 293–294；PDF 页 312–313 | EXAMPLE | 行稀疏假设失败时组套索劣于普通套索；(9.70)–(9.71) | 关键 | 完整讲解 |  | 原页已核 |
| Figure 9.10 印刷页 293；PDF 页 312 | FIGURE_TABLE | $\Theta^*=\Omega^*+\Gamma^*$ 分解卡通 | 辅助 | 简要说明 |  | 原页已核 |
| (9.72)–(9.76) 印刷页 294；PDF 页 313 | FORMULA | $\Phi_\omega$；权重 $\omega$；自适应组 GLM 套索与 RSC | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 9.31 印刷页 295；PDF 页 314 | COROLLARY | 自适应界 $\Vert\cdot\Vert_2^2\le(36\lambda_n^2/\kappa^2)(\sqrt{\lvert S_{\mathrm{elt}}\rvert}+\omega\sqrt{\lvert S_{\mathcal G}\rvert})^2$ | 关键 | 完整讲解 |  | 原页已核 |
| (9.77)–(9.79) 印刷页 295–296；PDF 页 314–315 | PROOF_DERIVATION | 对偶范数 $\max(\Vert v\Vert_\infty,\omega^{-1}\max\Vert v_g\Vert_2)$；锥 (9.78)；好事件 (9.79) | 关键 | 简要说明 | 适应机制进 Notes | 原页已核 |
| §9.8 印刷页 297–305；PDF 页 316–324 | SECTION | Techniques for proving restricted strong convexity | 关键 | 完整讲解 |  | 原页已核 |
| (9.81)–(9.84) 印刷页 298；PDF 页 317 | FORMULA | 总体 Taylor 余项；总体局部强凸；一致 LLN 目标；最小二乘特例 | 关键 | 完整讲解 |  | 原页已核 |
| Example 9.32 印刷页 298；PDF 页 317 | EXAMPLE | 最小二乘：算子范数 vs 限制特征值 | 辅助 | 简要说明 |  | 原页已核 |
| §9.8.1 印刷页 298–302；PDF 页 317–321 | SECTION | Lipschitz cost functions and Rademacher complexity | 关键 | 完整讲解 |  | 原页已核 |
| (9.85) 印刷页 299；PDF 页 318 | DEFINITION | 局部 $L$-Lipschitz：对线性预测 Lipschitz | 关键 | 完整讲解 |  | 原页已核 |
| Example 9.33 印刷页 299；PDF 页 318 | EXAMPLE | 逻辑斯蒂 $L=2$；铰链 $L=1$；最小二乘与指数一般非 Lipschitz | 关键 | 完整讲解 |  | 原页已核 |
| (9.86)–(9.89) 印刷页 299；PDF 页 318 | FORMULA | 逻辑斯蒂、铰链、$\Phi^*(\bar x_n)$、圆环 $\mathbb B_2(R_\ell,R_u)$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 9.34 印刷页 300；PDF 页 319 | THEOREM | Lipschitz 代价：$\lvert\mathcal E_n-\overline{\mathcal E}\rvert\le 16L\Phi(\Delta)\delta$ 于圆环 | 关键 | 完整讲解 |  | 原页已核 |
| Example 9.35 印刷页 300；PDF 页 319 | EXAMPLE | 组套索 + 高斯设计的 Lipschitz RSC | 辅助 | 简要说明 |  | 原页已核 |
| Theorem 9.34 证明 印刷页 301–302；PDF 页 320–321 | PROOF_DERIVATION | Taylor 余项 2L-Lipschitz；对称化 + 收缩；剥离 | 辅助 | 指回教材 | 技术细节长，Notes 只留策略 | 原页已核 |
| §9.8.2 印刷页 302–305；PDF 页 321–324 | SECTION | A one-sided bound via truncation | 关键 | 完整讲解 |  | 原页已核 |
| (9.94) 印刷页 303；PDF 页 322 | ASSUMPTION | 协变量二、四阶矩：$\mathbb E\langle\Delta,x\rangle^2\ge\alpha$，$\mathbb E\langle\Delta,x\rangle^4\le\beta$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 9.36 印刷页 303；PDF 页 322 | THEOREM | GLM 截断 RSC：$\mathcal E_n(\Delta)\ge(\kappa/2)\Vert\Delta\Vert_2^2-c_0\mu_n^2(\Phi^*)\Phi^2(\Delta)$ | 关键 | 完整讲解 |  | 原页已核 |
| (9.95)–(9.99) 印刷页 303–305；PDF 页 322–324 | PROOF_DERIVATION | Taylor 余项截断、期望下界、泛函 Hoeffding、收缩 | 辅助 | 指回教材 | 策略进 Notes，代数指回 | 原页已核 |
| §9.9 印刷页 306；PDF 页 325 | SECTION | Appendix: Star-shaped property | 关键 | 简要说明 |  | 原页已核 |
| §9.9 证明 印刷页 306；PDF 页 325 | PROOF_DERIVATION | $t\Delta$ 的投影齐性；$\theta^*\notin\mathbb M$ 时 $4t\Phi(\theta^*_{\overline{\mathbb M}^\perp})\le 4\Phi$ | 辅助 | 简要说明 |  | 原页已核 |
| §9.10 印刷页 306–307；PDF 页 325–326 | PROSE_RANGE | Bibliographic details：Negahban et al.、组套索文献、对偶范数界 | 辅助 | 指回教材 | 文献清单不抄入 Notes | 原页已核 |
| §9.11 印刷页 307–311；PDF 页 326–330 | SECTION | Exercises 9.1–9.14 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 9.1 印刷页 307；PDF 页 326 | EXERCISE | 重叠组变分式是范数 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 9.2 印刷页 307；PDF 页 326 | EXERCISE | 支撑子空间与行列空间子空间的投影 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 9.3 印刷页 308；PDF 页 327 | EXERCISE | 高斯与 Poisson GLM 核验 (9.5) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 9.4 印刷页 308；PDF 页 327 | EXERCISE | $\ell_1$、组 $\ell_p$、核范数的对偶 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 9.5 印刷页 308；PDF 页 327 | EXERCISE | 重叠组范数的对偶表示 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 9.6 印刷页 308；PDF 页 327 | EXERCISE | 次梯度满足 $\Phi^*(z)\le 1$ | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 9.7 印刷页 308–309；PDF 页 327–328 | EXERCISE | Hölder：一般对偶、$\ell_p$、Mahalanobis | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 9.8 印刷页 309；PDF 页 328 | EXERCISE | $\mu_n(\Phi^*)$：组套索与核范数 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 9.9 印刷页 309；PDF 页 328 | EXERCISE | 强凸的两种等价形式 (9.100) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 9.10 印刷页 309；PDF 页 328 | EXERCISE | 局部强凸推出球外线性曲率 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 9.11 印刷页 309；PDF 页 328 | EXERCISE | $\ell_\infty$ 曲率推出 $\ell_\infty$-RE | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 9.12 印刷页 309–310；PDF 页 328–329 | EXERCISE | 正交设计型 $\ell_1$ 与软阈值 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 9.13 印刷页 310；PDF 页 329 | EXERCISE | 由 $\ell_\infty$ 界推 $\ell_1$ 与 $\ell_2$ | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 9.14 印刷页 310–311；PDF 页 329–330 | EXERCISE | Lipschitz 代价的 $\ell_\infty$ 曲率 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |

## 来源异常与勘误

| 定位 | 问题类型 | 原式/原文 | 核验证据 | 处置 | 数学复核人 | 批准人 |
|---|---|---|---|---|---|---|
| Example 9.3 印刷页 262；PDF 页 281 | 笔误嫌疑 | “See panel (a) in Figure 9.3 for an example of a collection of overlapping groups.” | 原页 Figure 9.3(a) 图注写 non-overlapping disjoint partition；重叠组在 (b)，且 Example 9.4 正确指向 (b) | 保留原文；Notes 按不重叠读 (a)；`勘误待批` | 作者 | 未批 |
| Definition 9.18 讨论 印刷页 279；PDF 页 298 | 笔误嫌疑 | 同页先写 $\Vert\Delta\Vert_1\le 4\sqrt{s}\Vert\Delta\Vert_2$，随后称 “familiar inequality $\Vert\Delta\Vert_2\le 4\sqrt{s}\Vert\Delta\Vert_1$” | 原页；(9.45) 与第 7 章锥不等式均为 $\ell_1\le 4\sqrt{s}\,\ell_2$ | 保留两处原文；Notes 标明后一式与 (9.45) 左右对调；`勘误待批` | 作者 | 未批 |
| Corollary 9.20 vs 9.26 印刷页 281 与 287；PDF 页 300 与 306 | 常数不一致 | (9.49b) 为 $9(\lambda_n^2/\kappa^2)\Psi^2$； (9.63) 为 $(9/4)s\lambda_n^2/\kappa^2$。9.26 证明写应用 9.20，却用 $9\Psi^2\lambda_n^2/(4\kappa^2)<1$ | 原页两框；$\Psi^2(\mathbb M)=s$ 时应同为 9 或同为 9/4 | 两式均按原页抄入；Notes 标明常数不衔接；`勘误待批` | 作者 | 未批 |
| (9.82) 印刷页 298；PDF 页 317 | 笔误嫌疑 | $\mathbb B_2(R):=\{\Delta\in\Omega:\Vert\theta\Vert_2\le R\}$ | 原页；同页 $\overline{\mathcal E}(\Delta)$ 与 $\Delta\in\mathbb B_2(R)$ 的 dummy 应为 $\Delta$ | 保留原文；Notes 按 $\Vert\Delta\Vert_2\le R$ 解读；`勘误待批` | 作者 | 未批 |
| Exercise 9.14(a) 印刷页 310；PDF 页 329 | 常数嫌疑 | 称 (9.101) 以 $L=B^2/2$ 成立 | 原页；(G2) 为 $\Vert\psi''\Vert_\infty\le B^2$；$\partial_{\theta_j}\mathcal L=(\psi'(\langle x,\theta\rangle)-y)x_j$，差的界是 $B^2\lvert x_j\langle x,\theta-\overline\theta\rangle\rvert$ | 题解按链规则给出 $L=B^2$，并保留书中 $B^2/2$；`勘误待批` | 作者 | 未批 |
| Exercise 9.14(b) 印刷页 310；PDF 页 329 | 符号不一致 | 集合名为 $\mathbb T(R;\rho)$，定义里半径是 $r$，随后 $V_j$ 又写 $\mathbb T(r;\rho)$ | 原页同一段 | 题解统一用半径 $r$；`勘误待批` | 作者 | 未批 |

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
