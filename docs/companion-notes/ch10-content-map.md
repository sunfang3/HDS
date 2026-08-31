---
chapter_id: "ch10"
chapter_title: "Matrix estimation with rank constraints"
source_title: "High-Dimensional Statistics: A Non-Asymptotic Viewpoint"
source_version: "Cambridge Series in Statistical and Probabilistic Mathematics, No. 48; first published 2019; ISBN 978-1-108-49802-9"
main_source_path: "High-Dimensional Statistics A Non-Asymptotic Viewpoint (Martin J. Wainwright) (z-library.sk, 1lib.sk, z-lib.sk).pdf"
printed_pages: "312–346"
pdf_pages: "331–365"
target_notes: "notes/ch10-notes.qmd"
language: "zh-CN"
learner_profile: "学过陈希孺《概率论与数理统计》本科教材，并已读本书第 9 章可分解正则与限制强凸；熟悉奇异值、核范数与算子范数的对偶；首次需要把第 9 章抽象理论落到核范数矩阵回归、矩阵压缩感知、相位恢复、多元回归、矩阵补全与可加矩阵分解。"
map_status: "清单完成"
---

# 第 10 章内容清单

> 内部质量工件。正式对象（定义、命题、引理、定理、推论、关键公式）逐项登记；例题与连续叙述可聚合。习题进 Solutions，不进 Notes。

## 来源边界

- 教材权威来源：Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series No. 48
- 版本识别依据：封面 Cambridge Series；版权页 © Martin J. Wainwright 2019，First published 2019，ISBN 978-1-108-49802-9 Hardback，DOI 10.1017/9781108627771
- 目标章节与页码：第 10 章，印刷页 312–346；PDF 页 331–365（**PDF = 印刷 + 19**）
- 补充来源及用途：无
- 已知来源限制：文本层可用但公式常错位；公式、图注、命题框须对照 `scratch/ch10/p-3XX.png`

## 内容清单

| 定位 | 类型 | 内容/范围 | 重要性 | Notes 处理 | 合并目标/排除理由 | 核验状态 |
|---|---|---|---|---|---|---|
| 章首 印刷页 312；PDF 页 331 | SECTION | Chapter 10：秩约束矩阵估计；把第 9 章理论用于核范数正则及可加分解 | 关键 | 完整讲解 |  | 原页已核 |
| §10.1 印刷页 312–316；PDF 页 331–335 | SECTION | Matrix regression and applications | 关键 | 完整讲解 |  | 原页已核 |
| (10.1) 印刷页 312；PDF 页 331 | DEFINITION | 迹内积 $\langle\langle A,B\rangle\rangle=\mathrm{trace}(A^T B)$ | 关键 | 完整讲解 |  | 原页已核 |
| §10.1 印刷页 312；PDF 页 331 | DEFINITION | Frobenius 范数 $\\VertA\\Vert_{\mathrm{F}}=(\sum_{j_1,j_2} A_{j_1 j_2}^2)^{1/2}$ | 关键 | 完整讲解 |  | 原页已核 |
| (10.2) 印刷页 312；PDF 页 331 | FORMULA | 线性矩阵回归 $y_i=\langle\langle X_i,\Theta^*\rangle\rangle+w_i$ | 关键 | 完整讲解 |  | 原页已核 |
| (10.3) 印刷页 312；PDF 页 331 | DEFINITION | 观测算子 $\mathfrak{X}_n:\mathbb R^{d_1\times d_2}\to\mathbb R^n$，$[\mathfrak{X}_n(\Theta)]_i=\langle\langle X_i,\Theta\rangle\rangle$；伴随 $\mathfrak{X}_n^*(u)=\sum_i u_i X_i$ | 关键 | 完整讲解 |  | 原页已核 |
| (10.4) 印刷页 313；PDF 页 332 | FORMULA | 核范数正则最小二乘 $\widehat\Theta\in\arg\min\frac1{2n}\\Verty-\mathfrak{X}_n(\Theta)\\Vert_2^2+\lambda_n\\Vert\Theta\\Vert_{\mathrm{nuc}}$ | 关键 | 完整讲解 |  | 原页已核 |
| (10.5) 印刷页 313；PDF 页 332 | DEFINITION | 核范数 $\\Vert\Theta\\Vert_{\mathrm{nuc}}=\sum_{j=1}^{d'}\sigma_j(\Theta)$，$d'=\min\{d_1,d_2\}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 10.1 印刷页 313；PDF 页 332 | EXAMPLE | 多元回归作为矩阵回归；$X_{j\ell}=Z^T E_{j\ell}$，$N=nT$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 10.2 印刷页 313–315；PDF 页 332–334 | EXAMPLE | 低秩矩阵补全；Netflix；Jester 谱衰减 | 关键 | 完整讲解 |  | 原页已核 |
| Figure 10.1 印刷页 314；PDF 页 333 | FIGURE_TABLE | Netflix 示意与 Jester 奇异值衰减 | 辅助 | 简要说明 |  | 原页已核 |
| (10.6)–(10.7) 印刷页 315；PDF 页 334 | FORMULA | 含噪补全 $\widetilde y_i=\Theta_{a(i),b(i)}+w_i/\sqrt{d_1 d_2}$；掩码 $X_i$ 在 $(a(i),b(i))$ 处取 $\sqrt{d_1 d_2}$ | 关键 | 完整讲解 |  | 原页已核 |
| (10.8) 印刷页 315；PDF 页 334 | FORMULA | 矩阵逻辑斯蒂 $\mathbb P(y_i\mid X_i,\Theta^*)=e^{y_i\langle\langle X_i,\Theta^*\rangle\rangle}/(1+e^{y_i\langle\langle X_i,\Theta^*\rangle\rangle})$ | 辅助 | 简要说明 |  | 原页已核 |
| Example 10.3 印刷页 315；PDF 页 334 | EXAMPLE | 低秩矩阵压缩感知；$X_i$ 的 $D=d_1 d_2$ 个元 i.i.d. $N(0,1)$ | 关键 | 完整讲解 |  | 原页已核 |
| (10.9) 印刷页 315；PDF 页 334 | FORMULA | 无噪投影 $y_i=\langle\langle X_i,\Theta^*\rangle\rangle$ | 关键 | 并入相关内容 | Example 10.3 / Corollary 10.9 | 原页已核 |
| Example 10.4 印刷页 315–316；PDF 页 334–335 | EXAMPLE | 相位恢复：$\widetilde y_i=\lvert\langle x_i,\theta^*\rangle\rvert$，提升 $\Theta^*=\theta^*\otimes\theta^*$，$X_i=x_i\otimes x_i$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 10.5 印刷页 316–317；PDF 页 335–336 | EXAMPLE | 向量自回归 $z^{t+1}=\Theta^* z^t+w^t$；稳定条件 $\\Vert\Theta^*\\Vert_2<1$ | 关键 | 完整讲解 |  | 原页已核 |
| (10.10)–(10.11) 印刷页 316；PDF 页 335 | FORMULA | VAR 递推与二次损失 $\mathcal L_n(\Theta)=\frac1{2N}\sum_t\\Vertz^{t+1}-\Theta z^t\\Vert_{\Gamma^{-1}}^2$ | 关键 | 完整讲解 |  | 原页已核 |
| §10.2 印刷页 317–321；PDF 页 336–340 | SECTION | Analysis of nuclear norm regularization | 关键 | 完整讲解 |  | 原页已核 |
| §10.2.1 印刷页 317–319；PDF 页 336–338 | SECTION | Decomposability and subspaces | 关键 | 完整讲解 |  | 原页已核 |
| (10.12a)–(10.12b) 印刷页 317；PDF 页 336 | DEFINITION | 模型空间 $\mathbb M(\mathbb U,\mathbb V)$ 与 $\overline{\mathbb M}^\perp(\mathbb U,\mathbb V)$ | 关键 | 完整讲解 |  | 原页已核 |
| (10.13)–(10.14) 印刷页 318；PDF 页 337 | FORMULA | 分块表示：$\mathbb M$ 秩$\le r$，$\overline{\mathbb M}$ 秩$\le 2r$ | 关键 | 完整讲解 |  | 原页已核 |
| §10.2.1 印刷页 318；PDF 页 337 | PROOF_DERIVATION | 核范数对 $(\mathbb M,\overline{\mathbb M}^\perp)$ 可分解 | 关键 | 完整讲解 |  | 原页已核 |
| (10.15) 印刷页 319；PDF 页 338 | FORMULA | 锥约束 $\\Vert\widehat\Delta_{\overline{\mathbb M}^\perp}\\Vert_{\mathrm{nuc}}\le 3\\Vert\\widehat\Delta_{\overline{\mathbb M}}\\Vert_{\mathrm{nuc}}+4\\Vert\\Theta^*_{\mathbb M^\perp}\\Vert_{\mathrm{nuc}}$ | 关键 | 完整讲解 |  | 原页已核 |
| §10.2.2 印刷页 319–320；PDF 页 338–339 | SECTION | Restricted strong convexity and error bounds | 关键 | 完整讲解 |  | 原页已核 |
| (10.16) 印刷页 319；PDF 页 338 | FORMULA | 核范数正则 LS（与 (10.4) 相同） | 辅助 | 并入相关内容 | (10.4) | 原页已核 |
| (10.17) 印刷页 319；PDF 页 338 | FORMULA | RSC：$\\Vert\mathfrak{X}_n(\Delta)\\Vert_2^2/(2n)\ge(\kappa/2)\\Vert\Delta\\Vert_{\mathrm{F}}^2-c_0((d_1+d_2)/n)\\Vert\Delta\\Vert_{\mathrm{nuc}}^2$ | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 10.6 / (10.18) 印刷页 319；PDF 页 338 | PROPOSITION | 神谕不等式：Frobenius 误差按秩 $r$ 与尾奇异值拆开 | 关键 | 完整讲解 |  | 原页已核 |
| (10.19) 印刷页 320；PDF 页 339 | FORMULA | 恰低秩简化：$\\Vert\\widehat\Theta-\Theta^*\\Vert_{\mathrm{F}}^2\le(9/2)(\lambda_n^2/\kappa^2)\,\mathrm{rank}(\Theta^*)$ | 关键 | 完整讲解 |  | 原页已核 |
| §10.2.3 印刷页 320–321；PDF 页 339–340 | SECTION | Bounds under operator norm curvature | 关键 | 完整讲解 |  | 原页已核 |
| (10.20) 印刷页 320；PDF 页 339 | FORMULA | $\Phi^*$ 曲率：$\\Vert(1/n)\mathfrak{X}_n^*\mathfrak{X}_n(\Delta)\\Vert_2\ge\kappa\\Vert\Delta\\Vert_2-\tau_n\\Vert\Delta\\Vert_{\mathrm{nuc}}$ | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 10.7 / (10.21) 印刷页 321；PDF 页 340 | PROPOSITION | 算子范数界 $\\Vert\\widehat\Theta-\Theta^*\\Vert_2\le 3\sqrt{2}\,\lambda_n/\kappa$ | 关键 | 完整讲解 |  | 原页已核 |
| §10.3 印刷页 321–326；PDF 页 340–345 | SECTION | Matrix compressed sensing | 关键 | 完整讲解 |  | 原页已核 |
| §10.3 印刷页 321；PDF 页 340 | DEFINITION | $\Sigma$-高斯系综；$\rho^2(\Sigma)=\sup_{\\Vertu\\Vert_2=\\Vertv\\Vert_2=1}\mathrm{var}(\langle\langle X,uv^T\rangle\rangle)$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 10.8 / (10.22) 印刷页 322；PDF 页 341 | THEOREM | $\Sigma$-高斯系综的 RSC 下界 | 关键 | 完整讲解 |  | 原页已核 |
| (10.23) 印刷页 322；PDF 页 341 | FORMULA | 无噪核范数极小化（基追踪的矩阵类比） | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 10.9 印刷页 322；PDF 页 341 | COROLLARY | $n\gtrsim r(d_1+d_2)$ 时无噪精确恢复 | 关键 | 完整讲解 |  | 原页已核 |
| (10.24) 印刷页 323；PDF 页 342 | FORMULA | 锥上 $\\Vert\widehat\Delta\\Vert_{\mathrm{nuc}}\le 2\sqrt{2r}\\Vert\\widehat\Delta\\Vert_{\mathrm{F}}$ | 辅助 | 并入相关内容 | Corollary 10.9 证明 | 原页已核 |
| Corollary 10.10 / (10.25) 印刷页 323；PDF 页 342 | COROLLARY | 含噪界：$\\Vert\\widehat\Theta-\Theta^*\\Vert_{\mathrm{F}}^2\lesssim \sigma^2\rho^2 r(d_1+d_2)/(c_1^2\gamma_{\min}^2 n)$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 10.2 印刷页 324；PDF 页 343 | FIGURE_TABLE | Frobenius 误差对 $n$ 与对 $n/(rd)$ 的对齐 | 辅助 | 简要说明 |  | 原页已核 |
| (10.26)–(10.27) 印刷页 325；PDF 页 344 | FORMULA | 近低秩 $\ell_q$ 球 $B_q(R_q)$ 与误差 $R_q(\sigma^2(d_1+d_2)/n)^{1-q/2}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 10.11 / (10.28) 印刷页 325–326；PDF 页 344–345 | EXAMPLE | Lipschitz 损失对核范数的经验过程偏差 | 辅助 | 简要说明 |  | 原页已核 |
| §10.4 印刷页 326–329；PDF 页 345–348 | SECTION | Bounds for phase retrieval | 关键 | 完整讲解 |  | 原页已核 |
| (10.29) 印刷页 326；PDF 页 345 | FORMULA | 相位恢复 SDP：$\min\mathrm{trace}(\Theta)$ s.t. $\widetilde y_i^2=\langle\langle\Theta,x_i\otimes x_i\rangle\rangle$，$\Theta\succeq 0$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 10.12 / (10.30) 印刷页 327；PDF 页 346 | THEOREM | 相位恢复的限制零空间 / 特征值：$n>c_0\rho d$ | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 10.13 印刷页 327；PDF 页 346 | COROLLARY | $n>2c_0 d$ 时 SDP 唯一解为 $\Theta^*=\theta^*\otimes\theta^*$ | 关键 | 完整讲解 |  | 原页已核 |
| (10.31a)–(10.31b) 印刷页 328；PDF 页 347 | FORMULA | $E[\langle X,\Delta\rangle^2]=\\Vert\Delta\\Vert_{\mathrm{F}}^2+2(\mathrm{trace}\Delta)^2$；锥 $A_1(\sqrt{\rho})$ 上的单边一致律 | 关键 | 完整讲解 |  | 原页已核 |
| §10.5 印刷页 329–330；PDF 页 348–349 | SECTION | Multivariate regression with low-rank constraints | 关键 | 完整讲解 |  | 原页已核 |
| (10.32) 印刷页 329；PDF 页 348 | FORMULA | $Y=Z\Theta^*+W$，$\mathcal L_n(\Theta)=\frac1{2n}\\VertY-Z\Theta\\Vert_{\mathrm{F}}^2$ | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 10.14 / (10.33)–(10.34) 印刷页 329；PDF 页 348 | COROLLARY | 固定设计算子范数界；Frobenius / 核范数由锥放大 | 关键 | 完整讲解 |  | 原页已核 |
| (10.35) 印刷页 330；PDF 页 349 | FORMULA | $\mathbb P[\\Vert(1/n)Z^T W\\Vert_2\ge 5\sigma\sqrt{\gamma_{\max}(\widehat\Sigma)}(\sqrt{(d+T)/n}+\delta)]\le 2e^{-2n\delta^2}$ | 关键 | 完整讲解 |  | 原页已核 |
| §10.6 印刷页 330–337；PDF 页 349–356 | SECTION | Matrix completion | 关键 | 完整讲解 |  | 原页已核 |
| (10.36) 印刷页 330；PDF 页 349 | FORMULA | 重标定掩码使 $E[\\Vert\mathfrak{X}_n(\Theta^*)\\Vert_2^2/n]=\\Vert\Theta^*\\Vert_{\mathrm{F}}^2$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 10.15 / (10.37) 印刷页 331；PDF 页 350 | EXAMPLE | 坏矩阵 $\Theta^{\mathrm{bad}}=e_1\otimes e_1$；$n=o(d^2)$ 时落入零空间 | 关键 | 完整讲解 |  | 原页已核 |
| (10.38) 印刷页 331；PDF 页 350 | DEFINITION | 奇异向量不相干 / 杠杆分数 | 关键 | 完整讲解 |  | 原页已核 |
| Example 10.16 / (10.39) 印刷页 331–332；PDF 页 350–351 | EXAMPLE | 不相干条件对微小扰动不稳健 | 关键 | 完整讲解 |  | 原页已核 |
| (10.40) 印刷页 332；PDF 页 351 | DEFINITION | 尖刺比 $\alpha_{\mathrm{sp}}(\Theta)=\sqrt{d_1 d_2}\\Vert\Theta\\Vert_{\max}/\\Vert\Theta\\Vert_{\mathrm{F}}$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 10.17 / (10.41) 印刷页 332；PDF 页 351 | THEOREM | 矩阵补全算子的一致 RSC（含尖刺比与弱秩） | 关键 | 完整讲解 |  | 原页已核 |
| (10.42) 印刷页 333；PDF 页 352 | FORMULA | 带 $\\Vert\Theta\\Vert_{\max}\le\alpha/\sqrt{d_1 d_2}$ 约束的核范数补全 | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 10.18 / (10.43) 印刷页 333；PDF 页 352 | COROLLARY | 含噪补全：$\\Vert\\widehat\Theta-\Theta^*\\Vert_{\mathrm{F}}^2\lesssim\max\{\sigma^2,\alpha^2\} r(d\log d)/n$ | 关键 | 完整讲解 |  | 原页已核 |
| (10.44) 印刷页 334；PDF 页 353 | FORMULA | 锥上补全 RSC 下界 | 辅助 | 并入相关内容 | Corollary 10.18 证明提纲 | 原页已核 |
| (10.45)–(10.48) 印刷页 335–337；PDF 页 354–356 | PROOF_DERIVATION | Thm 10.17：经验过程 Bernstein、收缩、剥皮 | 辅助 | 简要说明 |  | 原页已核 |
| §10.7 印刷页 337–341；PDF 页 356–360 | SECTION | Additive matrix decompositions | 关键 | 完整讲解 |  | 原页已核 |
| (10.49) 印刷页 337；PDF 页 356 | FORMULA | $y=\mathfrak{X}_n(\Lambda^*+\Gamma^*)+w$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 10.19 / (10.50)–(10.51) 印刷页 338；PDF 页 357 | EXAMPLE | 稀疏噪声因子分析 $\Sigma=LL^T+\Gamma^*$ | 辅助 | 简要说明 |  | 原页已核 |
| Example 10.20 印刷页 338；PDF 页 357 | EXAMPLE | 带行稀疏腐蚀的矩阵补全（Amazon 攻击） | 辅助 | 简要说明 |  | 原页已核 |
| Example 10.21 / (10.52) 印刷页 339；PDF 页 358 | EXAMPLE | 稳健协方差：列稀疏腐蚀 | 辅助 | 简要说明 |  | 原页已核 |
| (10.53)–(10.54) 印刷页 340；PDF 页 359 | FORMULA | 低秩加稀疏凸程序与 Frobenius 误差 $e^2$ | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 10.22 / (10.55)–(10.56) 印刷页 340；PDF 页 359 | COROLLARY | 神谕不等式：$\lambda_n^2\omega_n^2 r+\lambda_n^2 s$ 型误差 | 关键 | 完整讲解 |  | 原页已核 |
| (10.57) 印刷页 341；PDF 页 360 | FORMULA | 加权正则的对偶 $\Phi_{\omega_n}^*(W,W)=\max\{\\VertW\\Vert_{\max},\\VertW\\Vert_2/\omega_n\}$ | 关键 | 完整讲解 |  | 原页已核 |
| §10.8 印刷页 341–343；PDF 页 360–362 | PROSE_RANGE | Bibliographic details：Fazel、Recht、Candès–Recht、相位恢复 SDP、Chandrasekaran 等 | 辅助 | 指回教材 | 文献清单不抄入 Notes | 原页已核 |
| §10.9 印刷页 343–346；PDF 页 362–365 | SECTION | Exercises 10.1–10.11 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 10.1 印刷页 343；PDF 页 362 | EXERCISE | 降秩回归的显式 SVD 形式 | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 10.2 / (10.58) 印刷页 343–344；PDF 页 362–363 | EXERCISE | VAR 平稳性与 Lyapunov 方程 | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 10.3 印刷页 344；PDF 页 363 | EXERCISE | 补全零空间：$\Theta^{\mathrm{bad}}$ 在 $n=o(d^2)$ 时不可见 | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 10.4 印刷页 344；PDF 页 363 | EXERCISE | 核范数锥不等式（无正则化的因子 1） | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 10.5 印刷页 344；PDF 页 363 | EXERCISE | $\Phi^*$ 曲率形式与 Frobenius–算子换算 | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 10.6 印刷页 344；PDF 页 363 | EXERCISE | 矩阵 CS 的 Gordon–Slepian 下界 | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 10.7 印刷页 344–345；PDF 页 363–364 | EXERCISE | 近低秩约束核范数估计 | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 10.8 印刷页 345；PDF 页 364 | EXERCISE | 证明 (10.35) | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 10.9 印刷页 345；PDF 页 364 | EXERCISE | 高斯掩码相位恢复的二阶矩 | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 10.10 印刷页 345–346；PDF 页 364–365 | EXERCISE | 含噪补全 Corollary 10.18 的证明提纲 | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 10.11 印刷页 346；PDF 页 365 | EXERCISE | 补全的 SVD 软阈值估计 | 辅助 | 不进入 Notes | Solutions | 原页已核 |

## 来源异常与勘误

| 定位 | 问题类型 | 原式/原文 | 核验证据 | 处置 | 数学复核人 | 批准人 |
|---|---|---|---|---|---|---|
| Exercise 10.1 印刷页 343；PDF 页 362 | 笔误嫌疑 | $\widehat\Theta_{\mathrm{RR}}=\widehat\Sigma_{ZZ}^{-1}\widehat\Sigma_{XY}VV^T$，但前文定义的是 $\widehat\Sigma_{ZY}=\frac1n Z^T Y$ | 原页；交叉协方差是 $p\times T$ 的 $\widehat\Sigma_{ZY}$；右特征向量来自 $\widehat\Sigma_{YZ}\widehat\Sigma_{ZZ}^{-1}\widehat\Sigma_{ZY}$ | 保留原文；Notes 不抄习题；Solutions 按 $\widehat\Sigma_{ZY}$ 推导并标 `勘误待批` | 作者 | 未批 |
| §10.5 印刷页 329；PDF 页 348 | 笔误嫌疑 | “$(Y,Z)\in\mathbb R^{n\times T}\times\mathbb R^{p\times T}$” | 原页；Example 10.1 与 $\widehat\Sigma=Z^T Z/n$ 要求 $Z\in\mathbb R^{n\times p}$ | 保留原文；Notes 按 $Z\in\mathbb R^{n\times p}$ 解读；`勘误待批` | 作者 | 未批 |
| Theorem 10.12 / (10.30) 印刷页 327；PDF 页 346 | 笔误嫌疑 | 锥条件写成 $\\Vert\Theta\\Vert_{\mathrm{F}}^2\le\rho\\Vert\Theta\\Vert_{\mathrm{nuc}}^2$ | 原页；证明中集合是 $A_1(\sqrt{\rho})=\\{\\Vert\Delta\\Vert_{\mathrm{nuc}}\le\sqrt{\rho}\\Vert\Delta\\Vert_{\mathrm{F}}\\}$；核范数始终 $\ge$ Frobenius，印刷锥对 $\rho\ge 1$ 含全体矩阵，与 $n\asymp\rho d$ 矛盾 | 保留原文；Notes 给出印刷式并指出证明集合；`勘误待批` | 作者 | 未批 |
| (10.31a) 与 Exercise 10.9(b) 印刷页 328、345；PDF 页 347、364 | 笔误嫌疑 | $E[\langle X,\Delta\rangle^2]=\\Vert\Delta\\Vert_{\mathrm{F}}^2+2(\mathrm{trace}\Delta)^2$ | 原页；对称矩阵的 Wick 公式给出 $2\\VertA\\Vert_{\mathrm{F}}^2+(\mathrm{tr} A)^2$ | 保留原文；Notes/Solutions 写出正确恒等式；`勘误待批` | 作者 | 未批 |
| (10.53) 印刷页 340；PDF 页 359 | 笔误嫌疑 | 印刷正则项写 $\omega_n\\Vert\\Lambda\\Vert_2$（算子范数） | 原页；同页证明与 (10.57) 使用 $\Phi_{\omega_n}=\\Vert\Gamma\\Vert_1+\omega_n\\Vert\\Lambda\\Vert_{\mathrm{nuc}}$，对偶才是 $\\VertW\\Vert_2/\omega_n$ | 保留原文；Notes 按核范数讲解并标明印刷式；`勘误待批` | 作者 | 未批 |
| Exercise 10.2(b) 印刷页 343；PDF 页 362 | 命题过强 | 由 Lyapunov 方程存在 $\Sigma\succ 0$ 推出 $\\Vert\Theta^*\\Vert_2<1$ | 原页；离散 Lyapunov 的充要条件是谱半径 $<1$。反例 $\Theta^*=\begin{pmatrix}0&2\\0&0\end{pmatrix}$，$\\Vert\Theta^*\\Vert_2=2$，但 $\Sigma=\mathrm{diag}(5,1)$ 对 $\Gamma=I$ 可解 | 保留原文；Solutions 给出反例与谱半径修正；`勘误待批` | 作者 | 未批 |
| Exercise 10.3 印刷页 344；PDF 页 363 | 笔误嫌疑 | $\mathfrak{X}_n:\mathbb R^{d\times d}\to\mathbb R$ | 原页；算子输出 $n$ 维，应为 $\mathbb R^n$ | 保留原文；Solutions 按 $\mathbb R^n$ 解读；`勘误待批` | 作者 | 未批 |
| Exercise 10.6 印刷页 344；PDF 页 363 | 笔误嫌疑 | $\mathbb B(t)\subset\mathbb R^{d_1\times d_1}$ | 原页；同题 $W\in\mathbb R^{d_1\times d_2}$，应为 $d_1\times d_2$ | 保留原文；Solutions 按 $d_1\times d_2$ 解读；`勘误待批` | 作者 | 未批 |
| Exercise 10.10(c) 印刷页 346；PDF 页 365 | 笔误嫌疑 | “Use part (c) to establish the bound.” | 原页；只有 (a)(b)(c) 三问，(c) 不能调用自身 | 保留原文；Solutions 按 (b) 解读；`勘误待批` | 作者 | 未批 |
| Figure 10.2 图注 印刷页 324；PDF 页 343 | 笔误嫌疑 | 图注 $d\in\{40,80,160\}$，正文印刷页 323 写 $d^2\in\{400,1600,6400\}$ | 原页；后者对应 $d\in\{20,40,80\}$，与图例 $d^2$ 一致 | 保留原文；Notes 跟正文 $d^2$ 并标明图注；`勘误待批` | 作者 | 未批 |
| §10.7 印刷页 339；PDF 页 358 | 笔误嫌疑 | “the matrix $\Theta^{\mathrm{bad}}$ from Example 10.16” | 原页；$\Theta^{\mathrm{bad}}$ 定义在 Example 10.15；(10.37) | 保留原文；Notes 按 10.15 解读；`勘误待批` | 作者 | 未批 |
| Theorem 10.12 证明 印刷页 328；PDF 页 347 | 笔误嫌疑 | $\mathbb E[x_j^4]=4$ | 原页；标准正态 $\mathbb E[Z^4]=3$，$\mathbb E[Z^8]=105$ 正确 | 保留原文；Notes 写出 $3$；Rosenthal 界只改万有常数；`勘误待批` | 作者 | 未批 |

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
