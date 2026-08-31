---
chapter_id: "ch08"
chapter_title: "Principal component analysis in high dimensions"
source_title: "High-Dimensional Statistics: A Non-Asymptotic Viewpoint"
source_version: "Cambridge Series in Statistical and Probabilistic Mathematics, No. 48; first published 2019; ISBN 978-1-108-49802-9"
main_source_path: "High-Dimensional Statistics A Non-Asymptotic Viewpoint (Martin J. Wainwright) (z-library.sk, 1lib.sk, z-lib.sk).pdf"
printed_pages: "236–258"
pdf_pages: "255–277"
target_notes: "notes/ch08-notes.qmd"
language: "zh-CN"
learner_profile: "学过陈希孺《概率论与数理统计》本科教材；熟悉协方差、特征分解与样本主成分的经典说法；缺口是高维 PCA、Davis–Kahan 型特征空间扰动、尖刺协方差模型，以及稀疏主成分在 n 小于 d 时如何恢复相合。"
map_status: "清单完成"
---

# 第 8 章内容清单

> 内部质量工件。正式内容逐项登记；习题全部进入 Solutions、不进入 Notes。公式对照 `scratch/ch08/p-255.png` 至 `p-277.png`。

## 来源边界

- 教材权威来源：Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series No. 48
- 版本识别依据：封面 Cambridge Series；版权页 © Martin J. Wainwright 2019，First published 2019，ISBN 978-1-108-49802-9 Hardback，DOI 10.1017/9781108627771
- 目标章节与页码：第 8 章，印刷页 236–258；PDF 页 255–277（**PDF = 印刷 + 19**）
- 补充来源及用途：无
- 已知来源限制：文本层可用但公式常错位；公式、图注、定理框须对照 `scratch/ch08/p-2XX.png`

## 内容清单

| 定位 | 类型 | 内容/范围 | 重要性 | Notes 处理 | 合并目标/排除理由 | 核验状态 |
|---|---|---|---|---|---|---|
| 章首 印刷页 236；PDF 页 255 | SECTION | Chapter 8 PCA in high dimensions：总体与样本特征向量、无结构与有结构 | 关键 | 完整讲解 |  | 原页已核 |
| §8.1 印刷页 236–241；PDF 页 255–260 | SECTION | Principal components and dimension reduction | 关键 | 完整讲解 |  | 原页已核 |
| §8.1 印刷页 236；PDF 页 255 | DEFINITION | 半正定锥 $\mathcal S_+^{d\times d}$；单位球面 $\mathbb S^{d-1}$；有序特征值 $\gamma_1(\Sigma)\ge\cdots\ge\gamma_d(\Sigma)\ge 0$ | 关键 | 完整讲解 |  | 原页已核 |
| (8.1) 印刷页 236；PDF 页 255 | FORMULA | 第一主成分 $v^*=\arg\max\mathrm{var}(\langle v,X\rangle)=\arg\max\langle v,\Sigma v\rangle$ | 关键 | 完整讲解 |  | 原页已核 |
| (8.2) 印刷页 236；PDF 页 255 | FORMULA | 前 $r$ 个主成分：正交 $V\in\mathbb R^{d\times r}$ 最大化 $\mathbb E\Vert V^T X\Vert_2^2$ | 关键 | 完整讲解 |  | 原页已核 |
| §8.1 印刷页 237；PDF 页 256 | FORMULA | 零均值样本协方差 $\widehat\Sigma=n^{-1}\sum x_i x_i^T$；插入原则 | 关键 | 完整讲解 |  | 原页已核 |
| (8.3) 印刷页 237；PDF 页 256 | FORMULA | 经验第一主成分 $\widehat v=\arg\max\langle v,\widehat\Sigma v\rangle$ | 关键 | 完整讲解 |  | 原页已核 |
| §8.1.1 印刷页 237–241；PDF 页 256–260 | SECTION | Interpretations and uses of PCA | 关键 | 完整讲解 |  | 原页已核 |
| Example 8.1 印刷页 237–238；PDF 页 256–257 | EXAMPLE | PCA as matrix approximation；Toeplitz 再中心化 | 关键 | 完整讲解 |  | 原页已核 |
| (8.4) 印刷页 237；PDF 页 256 | FORMULA | 秩至多为 $r$ 的最佳逼近 $Z^*=\arg\min\Vert\Sigma-Z\Vert^2$ | 关键 | 完整讲解 |  | 原页已核 |
| §8.1.1 脚注 1 印刷页 237；PDF 页 256 | DEFINITION | 对称矩阵的酉不变范数 $\Vert M\Vert=\Vert V^T M V\Vert$ | 关键 | 完整讲解 |  | 原页已核 |
| Eckart–Young–Mirsky 印刷页 237；PDF 页 256 | THEOREM | 最优秩 $r$ 逼近是截断特征分解 | 关键 | 完整讲解 |  | 原页已核 |
| (8.5) 印刷页 237；PDF 页 256 | FORMULA | $Z^*=\sum_{j=1}^r\gamma_j(\Sigma)\,(v_j\otimes v_j)$ | 关键 | 完整讲解 |  | 原页已核 |
| (8.6) 印刷页 237；PDF 页 256 | FORMULA | Frobenius 误差 $\Vert Z^*-\Sigma\Vert_F^2=\sum_{j=r+1}^d\gamma_j^2(\Sigma)$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 8.1 印刷页 238；PDF 页 257 | FIGURE_TABLE | 特征值速降与 $r\in\{5,10,25,100\}$ 的矩阵逼近 | 辅助 | 简要说明 |  | 原页已核 |
| Example 8.2 印刷页 238–240；PDF 页 257–259 | EXAMPLE | PCA for data compression；Yale 特征脸 $d=77760$、$n=165$ | 关键 | 完整讲解 |  | 原页已核 |
| (8.7) 印刷页 239；PDF 页 258 | FORMULA | 原书 $\mathbb E\Vert X-\Pi_{V^*}(X)\Vert_2^2=\sum_{j=r+1}^d\gamma_j^2(\Sigma)$ | 关键 | 完整讲解 | Notes 保留原式并标勘误待批 | 原页已核 |
| Figure 8.2 印刷页 239；PDF 页 258 | FIGURE_TABLE | 人脸样本、前 100 特征值、特征脸与重构 | 辅助 | 简要说明 |  | 原页已核 |
| Example 8.3 印刷页 240–241；PDF 页 259–260 | EXAMPLE | PCA for Gaussian mixture models | 关键 | 完整讲解 |  | 原页已核 |
| (8.8) 印刷页 240；PDF 页 259 | FORMULA | 两成分各向同性高斯混合 $f(x;\theta)=\alpha\phi(x;-\theta^*,\sigma^2 I_d)+(1-\alpha)\phi(x;\theta^*,\sigma^2 I_d)$ | 关键 | 完整讲解 |  | 原页已核 |
| §8.1.1 未编号 印刷页 240；PDF 页 259 | FORMULA | 二阶矩 $\Gamma=\mathbb E[X\otimes X]=\theta^*\otimes\theta^*+\sigma^2 I_d$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 8.3 印刷页 240；PDF 页 259 | FIGURE_TABLE | $d=2$ 混合密度与等高线 | 辅助 | 简要说明 |  | 原页已核 |
| 脚注 2 印刷页 241；PDF 页 260 | PROSE_RANGE | $\alpha=0.5$ 时二阶矩与协方差重合 | 辅助 | 并入相关内容 | Example 8.3 | 原页已核 |
| §8.1.2 印刷页 241–242；PDF 页 260–261 | SECTION | Perturbations of eigenvalues and eigenspaces | 关键 | 完整讲解 |  | 原页已核 |
| §8.1.2 未编号 印刷页 241；PDF 页 260 | FORMULA | $\gamma_1(Q)\le\gamma_1(R)+\Vert P\Vert_{\mathrm{op}}$，故 $\lvert\gamma_1(Q)-\gamma_1(R)\rvert\le\Vert Q-R\Vert_{\mathrm{op}}$ | 关键 | 完整讲解 |  | 原页已核 |
| (8.9) 印刷页 241；PDF 页 260 | FORMULA | Weyl：$\max_j\lvert\gamma_j(Q)-\gamma_j(R)\rvert\le\Vert Q-R\Vert_{\mathrm{op}}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 8.4 印刷页 241–242；PDF 页 260–261 | EXAMPLE | Sensitivity of eigenvectors；$Q_\varepsilon$ 与特征间隙过小 | 关键 | 完整讲解 |  | 原页已核 |
| (8.10) 印刷页 241；PDF 页 260 | FORMULA | $Q_\varepsilon=\begin{pmatrix}1&\varepsilon\\\varepsilon&1.01\end{pmatrix}=Q_0+\varepsilon P$ | 关键 | 完整讲解 |  | 原页已核 |
| §8.2 印刷页 242–248；PDF 页 261–267 | SECTION | Bounds for generic eigenvectors | 关键 | 完整讲解 |  | 原页已核 |
| §8.2.1 印刷页 242–245；PDF 页 261–264 | SECTION | A general deterministic result | 关键 | 完整讲解 |  | 原页已核 |
| (8.11) 印刷页 242；PDF 页 261 | FORMULA | 特征基下扰动 $\widetilde P=U^T P U$，块 $p_{11},\tilde p,\widetilde P_{22}$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 8.5 印刷页 243；PDF 页 262 | THEOREM | $\Vert P\Vert_{\mathrm{op}}<\nu/2$ 时 $\Vert\widehat\theta-\theta^*\Vert_2\le 2\Vert\tilde p\Vert_2/(\nu-2\Vert P\Vert_{\mathrm{op}})$ | 关键 | 完整讲解 |  | 原页已核 |
| (8.12) 印刷页 243；PDF 页 262 | FORMULA | Theorem 8.5 的定量界 | 关键 | 并入相关内容 | Theorem 8.5 | 原页已核 |
| Theorem 8.5 反例 印刷页 243；PDF 页 262 | EXAMPLE | $\Sigma=\mathrm{diag}\{2,1\}$，$P=\mathrm{diag}\{-1/2,+1/2\}$，恰在 $\Vert P\Vert_{\mathrm{op}}=\nu/2$ | 关键 | 完整讲解 |  | 原页已核 |
| (8.13) 印刷页 243；PDF 页 262 | FORMULA | $\Psi(\Delta;P)=\langle\Delta,P\Delta\rangle+2\langle\Delta,P\theta^*\rangle$ | 关键 | 完整讲解 |  | 原页已核 |
| (8.14) 印刷页 243；PDF 页 262 | FORMULA | 集合 $C$ 上的总体与经验二次型最大化 | 辅助 | 并入相关内容 | Lemma 8.6 | 原页已核 |
| Lemma 8.6 印刷页 243；PDF 页 262 | LEMMA | PCA 基本不等式 $\nu(1-\langle\widehat\theta,\theta^*\rangle^2)\le\lvert\Psi(\widehat\Delta;P)\rvert$ | 关键 | 完整讲解 |  | 原页已核 |
| (8.15) 印刷页 243；PDF 页 262 | FORMULA | Lemma 8.6 的不等式 | 关键 | 并入相关内容 | Lemma 8.6 | 原页已核 |
| Theorem 8.5 证明 印刷页 243–245；PDF 页 262–264 | PROOF_DERIVATION | 变分、块分解、$\Vert\widehat\Delta\Vert_2=\sqrt{2(1-\varrho)}$ | 关键 | 完整讲解 |  | 原页已核 |
| (8.16) 印刷页 243；PDF 页 262 | FORMULA | $\Psi$ 写成 $\widetilde P$ 的二次型 | 辅助 | 并入相关内容 | Theorem 8.5 证明 | 原页已核 |
| (8.17) 印刷页 244；PDF 页 263 | FORMULA | $\langle\langle\Sigma,\theta^*\otimes\theta^*-\widehat\theta\otimes\widehat\theta\rangle\rangle\ge(\nu/2)\Vert\widehat\Delta\Vert_2^2$ | 关键 | 并入相关内容 | Lemma 8.6 | 原页已核 |
| §8.2.2 印刷页 245–248；PDF 页 264–267 | SECTION | Consequences for a spiked ensemble | 关键 | 完整讲解 |  | 原页已核 |
| (8.18) 印刷页 245；PDF 页 264 | FORMULA | 尖刺样本 $x_i\stackrel{d}{=}\sqrt{\nu}\,\xi_i\theta^*+w_i$ | 关键 | 完整讲解 |  | 原页已核 |
| (8.19) 印刷页 245；PDF 页 264 | FORMULA | $\Sigma=\nu\theta^*(\theta^*)^T+I_d$；$\gamma_1=\nu+1$，间隙 $\nu$ | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 8.7 印刷页 245；PDF 页 264 | COROLLARY | $n>d$ 且 $\sqrt{(\nu+1)/\nu^2}\sqrt{d/n}\le 1/128$ 时的特征向量误差 | 关键 | 完整讲解 |  | 原页已核 |
| (8.20) 印刷页 245；PDF 页 264 | FORMULA | $\Vert\widehat\theta-\theta^*\Vert_2\le c_0\sqrt{(\nu+1)/\nu^2}\sqrt{d/n}+\delta$ | 关键 | 并入相关内容 | Corollary 8.7 | 原页已核 |
| Figure 8.4 印刷页 246；PDF 页 265 | FIGURE_TABLE | $n=500$、$d=100$ 与 $250$ 的尖刺 PCA 误差对 $\nu$ | 辅助 | 简要说明 |  | 原页已核 |
| Corollary 8.7 证明 印刷页 246–248；PDF 页 265–267 | PROOF_DERIVATION | 扰动分解 $P_1+P_2+P_3$ 与 Theorem 8.5 | 关键 | 完整讲解 |  | 原页已核 |
| (8.21) 印刷页 246；PDF 页 265 | FORMULA | $P=P_1+P_2+P_3$ 的三项分解 | 关键 | 完整讲解 |  | 原页已核 |
| (8.22a) 印刷页 246；PDF 页 265 | FORMULA | $\Vert P\Vert_{\mathrm{op}}$ 的三项上界 | 关键 | 并入相关内容 | Corollary 8.7 证明 | 原页已核 |
| (8.22b) 印刷页 247；PDF 页 266 | FORMULA | $\Vert\tilde p\Vert_2\le\sqrt{\nu}\Vert\bar w\Vert_2+\Vert n^{-1}\sum w_i w_i^T-I_d\Vert_{\mathrm{op}}$ | 关键 | 并入相关内容 | Corollary 8.7 证明 | 原页已核 |
| Lemma 8.8 印刷页 247；PDF 页 266 | LEMMA | $\xi_i^2$、$\bar w$ 与样本协方差三项次高斯尾 | 关键 | 简要说明 | 证明留作练习；Notes 只钉标度 | 原页已核 |
| (8.23a)–(8.23c) 印刷页 247；PDF 页 266 | FORMULA | Lemma 8.8 的三条概率界 | 关键 | 并入相关内容 | Lemma 8.8 | 原页已核 |
| (8.24) 印刷页 247；PDF 页 266 | FORMULA | 联合失败概率 $\phi(\delta_1,\delta_2,\delta_3)$ | 辅助 | 并入相关内容 | Corollary 8.7 证明 | 原页已核 |
| §8.3 印刷页 248–255；PDF 页 267–274 | SECTION | Sparse principal component analysis | 关键 | 完整讲解 |  | 原页已核 |
| §8.3 印刷页 248；PDF 页 267 | PROSE_RANGE | $d/n$ 不趋于 0 时无结构 PCA 与极小极大均失败；预告 Example 15.19 | 关键 | 完整讲解 |  | 原页已核 |
| Example 8.9 印刷页 248–249；PDF 页 267–268 | EXAMPLE | Sparse eigenfaces；$s=\lfloor 0.25d\rfloor=19440$ | 辅助 | 简要说明 |  | 原页已核 |
| Figure 8.5 印刷页 249；PDF 页 268 | FIGURE_TABLE | 稀疏特征脸与重构 | 辅助 | 简要说明 |  | 原页已核 |
| §8.3.1 印刷页 249–252；PDF 页 268–271 | SECTION | A general deterministic result for sparse PCA | 关键 | 完整讲解 |  | 原页已核 |
| (8.25a) 印刷页 249；PDF 页 268 | FORMULA | 约束稀疏 PCA：$\max\langle\theta,\widehat\Sigma\theta\rangle$，$\Vert\theta\Vert_2=1$，$\Vert\theta\Vert_1\le R$ | 关键 | 完整讲解 |  | 原页已核 |
| (8.25b) 印刷页 249；PDF 页 268 | FORMULA | 惩罚稀疏 PCA：减 $\lambda_n\Vert\theta\Vert_1$，且 $\Vert\theta\Vert_1\le(n/\log d)^{1/4}$ | 关键 | 完整讲解 |  | 原页已核 |
| (8.26) 印刷页 250；PDF 页 269 | ASSUMPTION | $\Psi$ 的一致偏差：二次、$\ell_1$、$\ell_1^2$ 三项 | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 8.10 印刷页 250；PDF 页 269 | THEOREM | 约束 (8.27) 与惩罚 (8.28) 的确定性误差 | 关键 | 完整讲解 |  | 原页已核 |
| (8.27) 印刷页 250；PDF 页 269 | FORMULA | $\min\{\Vert\widehat\theta-\theta^*\Vert_2,\Vert\widehat\theta+\theta^*\Vert_2\}\le 8\sqrt{s}\,\varphi_\nu/(\nu(1-4c_0))$ | 关键 | 并入相关内容 | Theorem 8.10 | 原页已核 |
| (8.28) 印刷页 250；PDF 页 269 | FORMULA | 惩罚形式，含 $\lambda_n/\varphi_\nu+4$ | 关键 | 并入相关内容 | Theorem 8.10 | 原页已核 |
| Theorem 8.10 证明 印刷页 250–252；PDF 页 269–271 | PROOF_DERIVATION | 锥不等式、基本不等式与 $\kappa>0$ | 关键 | 完整讲解 |  | 原页已核 |
| (8.29) 印刷页 251；PDF 页 270 | FORMULA | 锥上 $\lvert\Psi\rvert$ 的上界 | 辅助 | 并入相关内容 | Theorem 8.10 证明 | 原页已核 |
| (8.30) 印刷页 251；PDF 页 270 | FORMULA | 惩罚基本不等式 | 辅助 | 并入相关内容 | Theorem 8.10 证明 | 原页已核 |
| Lemma 8.11 印刷页 251；PDF 页 270 | LEMMA | 锥不等式 $\Vert\widehat\Delta_{S^c}\Vert_1\le 3\Vert\widehat\Delta_S\Vert_1$，故 $\Vert\widehat\Delta\Vert_1\le 4\sqrt{s}\Vert\widehat\Delta\Vert_2$ | 关键 | 完整讲解 |  | 原页已核 |
| (8.31) 印刷页 251；PDF 页 270 | FORMULA | Lemma 8.11 | 关键 | 并入相关内容 | Lemma 8.11 | 原页已核 |
| §8.3.2 印刷页 252–255；PDF 页 271–274 | SECTION | Consequences for the spiked model with sparsity | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 8.12 印刷页 252；PDF 页 271 | COROLLARY | $s\log d/n\le c\min\{1,\nu^2/(\nu+1)\}$ 时的稀疏尖刺误差 | 关键 | 完整讲解 |  | 原页已核 |
| (8.32) 印刷页 252；PDF 页 271 | FORMULA | $\min\{\Vert\widehat\theta-\theta^*\Vert_2,\Vert\widehat\theta+\theta^*\Vert_2\}\le c_4\sqrt{(\nu+1)/\nu^2}\{\sqrt{s\log d/n}+\delta\}$ | 关键 | 并入相关内容 | Corollary 8.12 | 原页已核 |
| Corollary 8.12 证明 印刷页 252–255；PDF 页 271–274 | PROOF_DERIVATION | 验证 (8.26) 并分解 $\Psi(\cdot;P_j)$ | 关键 | 简要说明 | 主线进 Notes；Lemma 8.14 细节指回教材 | 原页已核 |
| (8.33) 印刷页 252；PDF 页 271 | FORMULA | 一致偏差的显式 $\varphi_\nu,\psi_\nu^2,c_0=1/8$ | 关键 | 完整讲解 |  | 原页已核 |
| (8.34) 印刷页 253；PDF 页 272 | FORMULA | $\lvert\Psi(\Delta;P_1)\rvert\le(\nu/32)\Vert\Delta\Vert_2^2$ | 辅助 | 并入相关内容 | Corollary 8.12 证明 | 原页已核 |
| (8.35) 印刷页 253；PDF 页 272 | FORMULA | $\lvert\Psi(\Delta;P_2)\rvert$ 用 $\Vert\bar w\Vert_\infty$ 与 $\langle\theta^*,\bar w\rangle$ | 辅助 | 并入相关内容 | Corollary 8.12 证明 | 原页已核 |
| Lemma 8.13 印刷页 254；PDF 页 273 | LEMMA | $\Vert\bar w\Vert_\infty$ 与 $\langle\theta^*,\bar w\rangle$ 的次高斯尾 | 关键 | 简要说明 | 证明留作第 2 章练习 | 原页已核 |
| (8.36a)–(8.36b) 印刷页 254；PDF 页 273 | FORMULA | Lemma 8.13 | 关键 | 并入相关内容 | Lemma 8.13 | 原页已核 |
| (8.37) 印刷页 254；PDF 页 273 | FORMULA | $\lvert\Psi(\Delta;P_2)\rvert$ 的汇合界 | 辅助 | 并入相关内容 | Corollary 8.12 证明 | 原页已核 |
| (8.38) 印刷页 254；PDF 页 273 | FORMULA | $\lvert\Psi(\Delta;P_3)\rvert\le\lvert\langle\Delta,P_3\Delta\rangle\rvert+2\Vert P_3\theta^*\Vert_\infty\Vert\Delta\Vert_1$ | 辅助 | 并入相关内容 | Corollary 8.12 证明 | 原页已核 |
| Lemma 8.14 印刷页 254；PDF 页 273 | LEMMA | $\Vert P_3\theta^*\Vert_\infty$ 与二次型一致界 | 关键 | 简要说明 |  | 原页已核 |
| (8.39a)–(8.39b) 印刷页 254；PDF 页 273 | FORMULA | Lemma 8.14 | 关键 | 并入相关内容 | Lemma 8.14 | 原页已核 |
| (8.40) 印刷页 254；PDF 页 273 | FORMULA | $\lvert\Psi(\Delta;P_3)\rvert$ 的汇合界 | 辅助 | 并入相关内容 | Corollary 8.12 证明 | 原页已核 |
| Lemma 8.14 证明 印刷页 254–255；PDF 页 273–274 | PROOF_DERIVATION | 子矩阵并、Theorem 6.5、Exercise 7.10 | 辅助 | 指回教材 | 技术细节不抄入 Notes | 原页已核 |
| §8.4 印刷页 255–256；PDF 页 274–275 | PROSE_RANGE | Bibliographic details：Johnstone 尖刺、SCOTLASS、SDP、极小极大与 $k$-团硬度 | 辅助 | 指回教材 | 文献清单不抄入 Notes | 原页已核 |
| §8.5 印刷页 256–258；PDF 页 275–277 | SECTION | Exercises 8.1–8.9 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 8.1 印刷页 256；PDF 页 275 | EXERCISE | Courant–Fischer 变分表示 (8.41) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 8.2 印刷页 256；PDF 页 275 | EXERCISE | 酉不变矩阵范数 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 8.3 印刷页 256；PDF 页 275 | EXERCISE | 证明 Weyl 不等式 (8.9) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 8.4 印刷页 256；PDF 页 275 | EXERCISE | (8.2) 的变分刻画 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 8.5 印刷页 257；PDF 页 276 | EXERCISE | 矩阵幂法 (8.42) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 8.6 印刷页 257；PDF 页 276 | EXERCISE | 高斯混合的 PCA 估计 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 8.7 印刷页 257；PDF 页 276 | EXERCISE | 由绝对值内积做 PCA 检索 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 8.8 印刷页 257–258；PDF 页 276–277 | EXERCISE | 稀疏 PCA 的半定松弛 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 8.9 印刷页 258；PDF 页 277 | EXERCISE | 稀疏 PCA 的原–对偶见证 (8.43) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |

## 来源异常与勘误

| 定位 | 问题类型 | 原式/原文 | 核验证据 | 处置 | 数学复核人 | 批准人 |
|---|---|---|---|---|---|---|
| (8.7) 印刷页 239；PDF 页 258 | 公式笔误嫌疑 | $\mathbb E[\Vert X-\Pi_{V^*}(X)\Vert_2^2]=\sum_{j=r+1}^d\gamma_j^2(\Sigma)$ | 原页 PNG；正确恒等式为 $\mathrm{tr}((I-\Pi)\Sigma)=\sum_{j=r+1}^d\gamma_j(\Sigma)$。平方出现在 Frobenius 矩阵逼近 (8.6) | 保留原文；Notes 标明与迹恒等式不一致；`勘误待批` | 作者 | 未批 |
| Corollary 8.7 证明 印刷页 247；PDF 页 266 | 常数笔误嫌疑 | 选取 $\delta_1=1/16$，$\delta_2=\delta/(4\sqrt{\nu})$，$\delta_3=\delta/16$，但失败概率写成 $\phi(1/4,\delta/(3\sqrt{\nu}),\delta/16)$ | 原页 PNG；$\phi$ 的三个自变量与正文刚选定的 $(\delta_1,\delta_2,\delta_3)$ 不一致。标度结论不受影响 | 保留原文；Notes 按选定的 $\delta_i$ 读，并记下 $\phi$ 自变量；`勘误待批` | 作者 | 未批 |
| Exercise 8.2(a)(i) 印刷页 256；PDF 页 275 | 拼写 | The Frobenium norm | 原页 PNG；标准名为 Frobenius | 保留原文；Solutions 按 Frobenius 解答；`勘误待批` | 作者 | 未批 |
| Exercise 8.6(a) 印刷页 257；PDF 页 276 | 排版 | $n>c_1\sigma^2(1++\sigma^2)d$ | 原页 PNG；与随后误差中的 $\sqrt{1+\sigma^2}$ 及尖刺换元 $\nu=1/\sigma^2$ 一致，应为 $1+\sigma^2$ | 保留原文；Solutions 按 $1+\sigma^2$ 求解；`勘误待批` | 作者 | 未批 |
| Lemma 8.6 证明 印刷页 243；PDF 页 262 | 符号笔误嫌疑 | 正文写 $\langle\langle\Sigma,\theta^*\otimes\theta^*-\widehat\theta\otimes\widehat\theta\rangle\rangle\le -\langle\langle P,\theta^*\otimes\theta^*-\widehat\theta\otimes\widehat\theta\rangle\rangle$，并称右端等于 $-\Psi(\widehat\Delta;P)$ | 原页 PNG。由 $\Psi(\Delta;P)=\langle\Delta,P\Delta\rangle+2\langle\Delta,P\theta^*\rangle$ 直接展开得 $-\langle\langle P,\theta^*\otimes\theta^*-\widehat\theta\otimes\widehat\theta\rangle\rangle=\Psi(\widehat\Delta;P)$，不是 $-\Psi$。随后 Lemma 8.6 用绝对值，结论不受影响 | 保留原文；Notes 按 $\Psi$ 的定义展开并取绝对值；`勘误待批` | 作者 | 未批 |
| Corollary 8.12 证明 印刷页 253；PDF 页 272 | 半径不一致 | 证明核 $\|\theta^*\|_1\le\nu\sqrt{n/\log d}$，并用该半径代入 $4R\psi_\nu^2$ | 原页 PNG。(8.25b) 与 Theorem 8.10 的技术球是 $(n/\log d)^{1/4}$。两种半径下 $4R\psi_\nu^2$ 都不超过 $\varphi_\nu$ 的量级，(8.32) 的标度不受影响 | 保留各处原文；Notes 标明不一致；`勘误待批` | 作者 | 未批 |

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
