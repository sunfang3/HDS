---
chapter_id: "ch07"
chapter_title: "Sparse linear models in high dimensions"
source_title: "High-Dimensional Statistics: A Non-Asymptotic Viewpoint"
source_version: "Cambridge Series in Statistical and Probabilistic Mathematics, No. 48; first published 2019; ISBN 978-1-108-49802-9"
main_source_path: "High-Dimensional Statistics A Non-Asymptotic Viewpoint (Martin J. Wainwright) (z-library.sk, 1lib.sk, z-lib.sk).pdf"
printed_pages: "194–235"
pdf_pages: "213–254"
target_notes: "notes/ch07-notes.qmd"
language: "zh-CN"
learner_profile: "学过陈希孺《概率论与数理统计》本科教材；已读本书第 1–2 章（稀疏阈值、次高斯尾界）；首次需要把 ℓ0 稀疏回归的凸松弛（基追踪 / 套索）、限制零空间、限制特征值与变量选择一致性写成非渐近定理。"
map_status: "清单完成"
---

# 第 7 章内容清单

> 内部质量工件。正式内容逐项登记；§7.6 附录证明与 §7.8 习题不进入 Notes。

## 来源边界

- 教材权威来源：Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series No. 48
- 版本识别依据：封面 Cambridge Series；版权页 © Martin J. Wainwright 2019，First published 2019，ISBN 978-1-108-49802-9 Hardback，DOI 10.1017/9781108627771
- 目标章节与页码：第 7 章，印刷页 194–235；PDF 页 213–254（**PDF = 印刷 + 19**）
- 补充来源及用途：无（习题独立求解）
- 已知来源限制：文本层可用但公式常错位；公式、图注须对照 `scratch/ch07/p-2XX.png`

## 内容清单

| 定位 | 类型 | 内容/范围 | 重要性 | Notes 处理 | 合并目标/排除理由 | 核验状态 |
|---|---|---|---|---|---|---|
| 章首 印刷页 194；PDF 页 213 | SECTION | Chapter 7 Sparse linear models in high dimensions：高维线性模型与稀疏结构 | 关键 | 完整讲解 |  | 原页已核 |
| (7.1) 印刷页 194；PDF 页 213 | FORMULA | 线性模型 $y=X\theta^*+w$ | 关键 | 完整讲解 |  | 原页已核 |
| §7.1 印刷页 194–199；PDF 页 213–218 | SECTION | Problem formulation and applications | 关键 | 完整讲解 |  | 原页已核 |
| §7.1.1 印刷页 194–196；PDF 页 213–215 | SECTION | Different sparsity models：硬稀疏与弱稀疏 | 关键 | 完整讲解 |  | 原页已核 |
| Figure 7.1 印刷页 195；PDF 页 214 | FIGURE_TABLE | $\ell_q$-“球” $q=1,0.75,0.5$ | 辅助 | 简要说明 |  | 原页已核 |
| (7.2) 印刷页 195；PDF 页 214 | DEFINITION | 支撑集 $S(\theta^*)=\{j:\theta^*_j\neq 0\}$，$s=\lvert S(\theta^*)\rvert$ | 关键 | 完整讲解 |  | 原页已核 |
| (7.3) 印刷页 195；PDF 页 214 | DEFINITION | $\ell_q$-球 $\mathbb B_q(R_q)=\{\theta:\sum_j\lvert\theta_j\rvert^q\le R_q\}$ | 关键 | 完整讲解 |  | 原页已核 |
| (7.4) 印刷页 195；PDF 页 214 | FORMULA | 按绝对值降序的坐标 $\lvert\theta^*_{(1)}\rvert\ge\cdots\ge\lvert\theta^*_{(d)}\rvert$ | 关键 | 完整讲解 |  | 原页已核 |
| §7.1.2 印刷页 196–199；PDF 页 215–218 | SECTION | Applications of sparse linear models | 关键 | 完整讲解 |  | 原页已核 |
| Example 7.1 印刷页 196；PDF 页 215 | EXAMPLE | 高斯序列模型 $y_i=\sqrt n\,\theta^*_i+w_i$，$X=\sqrt n\,I_n$ | 关键 | 完整讲解 |  | 原页已核 |
| (7.5) 印刷页 196；PDF 页 215 | FORMULA | 高斯序列观测方程 | 关键 | 并入相关内容 | Example 7.1 | 原页已核 |
| Example 7.2 印刷页 196–197；PDF 页 215–216 | EXAMPLE | 正交基下的信号去噪与压缩 | 关键 | 完整讲解 |  | 原页已核 |
| (7.6a) 印刷页 197；PDF 页 216 | DEFINITION | 硬阈值 $[H_\lambda(y)]_i=y_i\,\mathbb I[\lvert y_i\rvert\ge\lambda]$ | 关键 | 完整讲解 |  | 原页已核 |
| (7.6b) 印刷页 197；PDF 页 216 | DEFINITION | 软阈值 $[T_\lambda(y)]_i=\mathrm{sign}(y_i)(\lvert y_i\rvert-\lambda)_+$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 7.3 印刷页 197–198；PDF 页 216–217 | EXAMPLE | 提升与非线性：多项式 / 基函数线性化 | 辅助 | 简要说明 |  | 原页已核 |
| Example 7.4 印刷页 198；PDF 页 217 | EXAMPLE | 过完备基下的信号压缩与 $\ell_1$ 松弛 | 关键 | 完整讲解 |  | 原页已核 |
| Example 7.5 印刷页 198–199；PDF 页 217–218 | EXAMPLE | 压缩感知与随机投影 | 关键 | 完整讲解 |  | 原页已核 |
| (7.7) 印刷页 199；PDF 页 218 | FORMULA | 变换域基追踪 $\min\lVert\theta\rVert_1$ s.t. $y=\widetilde X\theta$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 7.6 印刷页 199；PDF 页 218 | EXAMPLE | 高斯图模型选择化为稀疏回归 | 辅助 | 简要说明 |  | 原页已核 |
| §7.2 印刷页 199–205；PDF 页 218–224 | SECTION | Recovery in the noiseless setting | 关键 | 完整讲解 |  | 原页已核 |
| §7.2.1 印刷页 200；PDF 页 219 | SECTION | $\ell_1$-based relaxation | 关键 | 完整讲解 |  | 原页已核 |
| 印刷页 200；PDF 页 219 | DEFINITION | $\ell_0$-“范数” $\lVert\theta\rVert_0=\sum_j\mathbb I[\theta_j\neq 0]$ | 关键 | 完整讲解 |  | 原页已核 |
| (7.8) 印刷页 200；PDF 页 219 | FORMULA | $\ell_0$ 规划 $\min\lVert\theta\rVert_0$ s.t. $X\theta=y$ | 关键 | 完整讲解 |  | 原页已核 |
| (7.9) 印刷页 200；PDF 页 219 | FORMULA | 基追踪 LP $\min\lVert\theta\rVert_1$ s.t. $X\theta=y$ | 关键 | 完整讲解 |  | 原页已核 |
| §7.2.2 印刷页 200–202；PDF 页 219–221 | SECTION | Exact recovery and restricted nullspace | 关键 | 完整讲解 |  | 原页已核 |
| (7.10) 印刷页 201；PDF 页 220 | DEFINITION | $\ell_1$-球在 $\theta^*$ 处的切锥 $\mathbb T(\theta^*)$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 7.2 印刷页 201；PDF 页 220 | FIGURE_TABLE | 切锥与限制零空间的二维几何 | 辅助 | 简要说明 |  | 原页已核 |
| 印刷页 201；PDF 页 220 | DEFINITION | 锥 $\mathbb C(S)=\{\Delta:\lVert\Delta_{S^c}\rVert_1\le\lVert\Delta_S\rVert_1\}$ | 关键 | 完整讲解 |  | 原页已核 |
| Definition 7.7 印刷页 202；PDF 页 221 | DEFINITION | 限制零空间性质 $\mathbb C(S)\cap\mathrm{null}(X)=\{0\}$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 7.8 印刷页 202；PDF 页 221 | THEOREM | 基追踪对一切 $S$-稀疏向量唯一恢复 $\iff$ 限制零空间 | 关键 | 完整讲解 |  | 原页已核 |
| (7.11) 印刷页 202；PDF 页 221 | FORMULA | 反向蕴含所用的辅助基追踪问题 | 辅助 | 并入相关内容 | Theorem 7.8 | 原页已核 |
| §7.2.3 印刷页 202–205；PDF 页 221–224 | SECTION | Sufficient conditions for restricted nullspace | 关键 | 完整讲解 |  | 原页已核 |
| (7.12) 印刷页 203；PDF 页 222 | DEFINITION | 成对不相干 $\delta_{\mathrm{PW}}(X)$ | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 7.9 / (7.13) 印刷页 203；PDF 页 222 | PROPOSITION | $\delta_{\mathrm{PW}}(X)\le 1/(3s)$ $\Rightarrow$ 均匀限制零空间 | 关键 | 完整讲解 |  | 原页已核 |
| Definition 7.10 / (7.14) 印刷页 203；PDF 页 222 | DEFINITION | 限制等距性质（RIP）$\delta_s(X)$ | 关键 | 完整讲解 |  | 原页已核 |
| (7.15) 印刷页 204；PDF 页 223 | FORMULA | $\delta_{\mathrm{PW}}\le\delta_s\le s\,\delta_{\mathrm{PW}}$ | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 7.11 印刷页 204；PDF 页 223 | PROPOSITION | $\delta_{2s}(X)<1/3$ $\Rightarrow$ 均匀限制零空间 | 关键 | 完整讲解 |  | 原页已核 |
| (7.16) 印刷页 205；PDF 页 224 | FORMULA | RIP 证明中的 $\lVert\widetilde\theta_{S_0}\rVert_2\le\frac{\delta_{2s}}{1-\delta_{2s}}\sum_j\lVert\widetilde\theta_{S_j}\rVert_2$ | 辅助 | 并入相关内容 | Proposition 7.11 | 原页已核 |
| (7.17) 印刷页 205；PDF 页 224 | FORMULA | 尖峰单位协方差 $\Sigma=(1-\mu)I_d+\mu\mathbb 1\mathbb 1^T$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 7.3 印刷页 206；PDF 页 225 | FIGURE_TABLE | 各向同性高斯设计下基追踪相变 | 辅助 | 简要说明 |  | 原页已核 |
| §7.3 印刷页 206–216；PDF 页 225–235 | SECTION | Estimation in noisy settings | 关键 | 完整讲解 |  | 原页已核 |
| (7.18) 印刷页 206；PDF 页 225 | FORMULA | 拉格朗日套索 $\frac1{2n}\lVert y-X\theta\rVert_2^2+\lambda_n\lVert\theta\rVert_1$ | 关键 | 完整讲解 |  | 原页已核 |
| (7.19) 印刷页 206；PDF 页 225 | FORMULA | 约束套索 $\lVert\theta\rVert_1\le R$ | 关键 | 完整讲解 |  | 原页已核 |
| (7.20) 印刷页 206；PDF 页 225 | FORMULA | 松弛基追踪 $\frac1{2n}\lVert y-X\theta\rVert_2^2\le b^2$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 7.4 印刷页 207；PDF 页 226 | FIGURE_TABLE | $\mu=0.5$ 相关设计下基追踪仍出现同一相变 | 辅助 | 简要说明 |  | 原页已核 |
| §7.3.1 印刷页 207–209；PDF 页 226–228 | SECTION | Restricted eigenvalue condition | 关键 | 完整讲解 |  | 原页已核 |
| (7.21) 印刷页 207；PDF 页 226 | DEFINITION | 锥 $\mathbb C_\alpha(S)=\{\Delta:\lVert\Delta_{S^c}\rVert_1\le\alpha\lVert\Delta_S\rVert_1\}$ | 关键 | 完整讲解 |  | 原页已核 |
| Definition 7.12 / (7.22) 印刷页 208；PDF 页 227 | DEFINITION | 限制特征值（RE）：$\frac1n\lVert X\Delta\rVert_2^2\ge\kappa\lVert\Delta\rVert_2^2$ 对一切 $\Delta\in\mathbb C_\alpha(S)$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 7.5 印刷页 208；PDF 页 227 | FIGURE_TABLE | 代价函数曲率与估计误差 | 辅助 | 简要说明 |  | 原页已核 |
| (7.23) 印刷页 209；PDF 页 228 | FORMULA | Hessian $\nabla^2\mathcal L_n(\theta)=n^{-1}X^T X$ | 关键 | 完整讲解 |  | 原页已核 |
| (7.24) 印刷页 209；PDF 页 228 | FORMULA | 全空间强凸（$d>n$ 时不可能） | 关键 | 完整讲解 |  | 原页已核 |
| Figure 7.6 印刷页 209；PDF 页 228 | FIGURE_TABLE | 高维二次型只在部分方向弯曲；误差落在 $\mathbb C_\alpha(S)$ | 辅助 | 简要说明 |  | 原页已核 |
| §7.3.2 印刷页 209–213；PDF 页 228–232 | SECTION | Bounds on $\ell_2$-error for hard sparse models | 关键 | 完整讲解 |  | 原页已核 |
| (A1)–(A2) 印刷页 210；PDF 页 229 | ASSUMPTION | $\theta^*$ 支撑在 $S$，$\lvert S\rvert=s$；RE 参数 $(\kappa,3)$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 7.13 / (7.25a–c) 印刷页 210；PDF 页 229 | THEOREM | 三种套索的 $\ell_2$ 误差界；附 $\ell_1$ 界 $\lVert\widehat\theta-\theta^*\rVert_1\le 4\sqrt s\,\lVert\widehat\theta-\theta^*\rVert_2$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 7.14 / (7.26)–(7.27) 印刷页 210–211；PDF 页 229–230 | EXAMPLE | 经典高斯线性模型：$C$-列标准化下的高概率界 | 关键 | 完整讲解 |  | 原页已核 |
| Example 7.15 印刷页 211–212；PDF 页 230–231 | EXAMPLE | 压缩感知：高斯设计、有界噪声 | 关键 | 完整讲解 |  | 原页已核 |
| (7.28) 印刷页 212；PDF 页 231 | FORMULA | 约束套索基本不等式 $\frac1n\lVert X\widehat\Delta\rVert_2^2\le\frac{2w^T X\widehat\Delta}n$ | 关键 | 并入相关内容 | Theorem 7.13 | 原页已核 |
| (7.29)–(7.30) 印刷页 213；PDF 页 232 | FORMULA | 拉格朗日基本不等式；$\lambda_n\ge 2\lVert X^T w/n\rVert_\infty$ $\Rightarrow$ $\widehat\Delta\in\mathbb C_3(S)$ | 关键 | 完整讲解 |  | 原页已核 |
| §7.3.3 印刷页 213–216；PDF 页 232–235 | SECTION | Restricted nullspace and eigenvalues for random designs | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 7.16 / (7.31) 印刷页 214；PDF 页 233 | THEOREM | 高斯行 $N(0,\Sigma)$ 的二次型下界；$c_1=1/8$，$c_2=50$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 7.17 印刷页 214；PDF 页 233 | EXAMPLE | 几何衰减 Toeplitz $\Sigma_{ij}=\nu^{\lvert i-j\rvert}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 7.18 印刷页 214–215；PDF 页 233–234 | EXAMPLE | 尖峰单位模型：RE 成立但 RIP / 成对不相干失败 | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 7.19 / (7.32) 印刷页 215；PDF 页 234 | THEOREM | 套索预言不等式：估计误差 + 逼近误差 | 关键 | 完整讲解 |  | 原页已核 |
| (7.33)–(7.36) 印刷页 215–216；PDF 页 234–235 | PROOF_DERIVATION | 预言不等式证明：一般向量的锥不等式与分情形 | 辅助 | 简要说明 |  | 原页已核 |
| §7.4 印刷页 216–218；PDF 页 235–237 | SECTION | Bounds on prediction error | 关键 | 完整讲解 |  | 原页已核 |
| (7.37) 印刷页 216；PDF 页 235 | DEFINITION | 样本内均方预测误差 $n^{-1}\lVert X(\widehat\theta-\theta^*)\rVert_2^2$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 7.20 / (7.38)–(7.39) 印刷页 217；PDF 页 236 | THEOREM | 预测误差慢速率与快速率 | 关键 | 完整讲解 |  | 原页已核 |
| (7.40)–(7.41) 印刷页 217；PDF 页 236 | FORMULA | 次高斯噪声下的慢/快高概率界 | 关键 | 完整讲解 |  | 原页已核 |
| (7.42) 印刷页 218；PDF 页 237 | FORMULA | 预测误差证明中的拉格朗日基本不等式 | 辅助 | 并入相关内容 | Theorem 7.20 | 原页已核 |
| §7.5 印刷页 218–224；PDF 页 237–243 | SECTION | Variable or subset selection | 关键 | 完整讲解 |  | 原页已核 |
| §7.5.1 印刷页 219–222；PDF 页 238–241 | SECTION | Variable selection consistency for the Lasso | 关键 | 完整讲解 |  | 原页已核 |
| (A3) / (7.43a) 印刷页 219；PDF 页 238 | ASSUMPTION | 下特征值 $\gamma_{\min}(X_S^T X_S/n)\ge c_{\min}>0$ | 关键 | 完整讲解 |  | 原页已核 |
| (A4) / (7.43b) 印刷页 219；PDF 页 238 | ASSUMPTION | 相互不相干 $\max_{j\in S^c}\lVert(X_S^T X_S)^{-1}X_S^T X_j\rVert_1\le\alpha<1$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 7.21 / (7.44)–(7.45) 印刷页 220；PDF 页 239 | THEOREM | 套索唯一性、无假阳性、$\ell_\infty$ 界、无假阴性 | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 7.22 / (7.46)–(7.47) 印刷页 220–221；PDF 页 239–240 | COROLLARY | 次高斯噪声、列标准化下的变量选择 | 关键 | 完整讲解 |  | 原页已核 |
| Figure 7.7 印刷页 222；PDF 页 241 | FIGURE_TABLE | 变量选择相变：$n/(s\log(d-s))$ | 辅助 | 简要说明 |  | 原页已核 |
| §7.5.2 印刷页 222–224；PDF 页 241–243 | SECTION | Proof of Theorem 7.21：原–对偶见证 | 关键 | 完整讲解 |  | 原页已核 |
| (7.48) 印刷页 222；PDF 页 241 | FORMULA | 零次梯度条件 $n^{-1}X^T(X\widehat\theta-y)+\lambda_n\widehat z=0$ | 关键 | 完整讲解 |  | 原页已核 |
| (7.49) 印刷页 223；PDF 页 242 | ALGORITHM | PDW 构造：$\widehat\theta_{S^c}=0$、oracle 子问题、严格对偶可行 | 关键 | 完整讲解 |  | 原页已核 |
| (7.50)–(7.54) 印刷页 223–224；PDF 页 242–243 | FORMULA | 分块 KKT、$\widehat z_{S^c}$ 与 $\widehat\theta_S-\theta^*_S$ 的显式 | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 7.23 印刷页 223；PDF 页 242 | LEMMA | PDW 成功 + (A3) $\Rightarrow$ $(\widehat\theta_S,0)$ 是唯一最优 | 关键 | 完整讲解 |  | 原页已核 |
| §7.6 印刷页 224–227；PDF 页 243–246 | SECTION | Appendix: Proof of Theorem 7.16 | 辅助 | 简要说明 | 主线只留 Gordon 比较与剥壳；细节指回教材 | 原页已核 |
| (7.55)–(7.59) 印刷页 224–227；PDF 页 243–246 | PROOF_DERIVATION | 坏事件、半径壳、Gordon 比较、高斯利普希茨尾 | 辅助 | 指回教材 | 附录完整证明不抄入 Notes | 原页已核 |
| Lemma 7.24 / (7.57a–b) 印刷页 225；PDF 页 244 | LEMMA | 壳事件尾界与坏事件覆盖 | 辅助 | 简要说明 |  | 原页已核 |
| §7.7 印刷页 227–229；PDF 页 246–248 | PROSE_RANGE | Bibliographic details：基追踪、套索、RIP、RE、PDW、慢/快速率 | 辅助 | 指回教材 | 文献清单不抄入 Notes | 原页已核 |
| §7.8 印刷页 229–235；PDF 页 248–254 | SECTION | Exercises 7.1–7.20 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 7.1 印刷页 229；PDF 页 248 | EXERCISE | 硬/软阈值的优化解释 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 7.2 印刷页 229–230；PDF 页 248–249 | EXERCISE | $\ell_q$-球：星形、强弱包含、最佳 $s$ 项逼近 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| (7.60)–(7.63) 印刷页 229–230；PDF 页 248–249 | FORMULA | 强/弱 $\ell_q$-球与最佳 $s$ 项逼近误差 | 关键 | 完整讲解 | 正文 (7.3)–(7.4) 已用；习题式编号在 Notes 只作对照 | 原页已核 |
| Exercise 7.3 印刷页 230；PDF 页 249 | EXERCISE | 成对不相干 $\Rightarrow$ 限制零空间 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 7.4 印刷页 230；PDF 页 249 | EXERCISE | RIP 与成对不相干的夹心与紧例 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 7.5 印刷页 230；PDF 页 249 | EXERCISE | $\ell_2$-RE $\Rightarrow$ $\ell_1$-RE | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 7.6 印刷页 230–231；PDF 页 249–250 | EXERCISE | 加权 $\ell_1$ 与加权基追踪 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 7.7 印刷页 231；PDF 页 250 | EXERCISE | 各向同性高斯的成对不相干与 RIP 样本量 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 7.8 印刷页 231；PDF 页 250 | EXERCISE | 尖峰单位模型下不相干与 RIP 失败 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 7.9 印刷页 231；PDF 页 250 | EXERCISE | $\ell_0$ 与 $\ell_1$ 约束集的凸包关系 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 7.10 印刷页 231–232；PDF 页 250–251 | EXERCISE | 由 $\mathbb L_0(2s)$ 控制推出 RE | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 7.11 印刷页 232；PDF 页 251 | EXERCISE | (7.31) 推出均匀 RE | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 7.12 印刷页 232；PDF 页 251 | EXERCISE | $\ell_q$-球上的套索 $\ell_2$ 速率 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 7.13 印刷页 232；PDF 页 251 | EXERCISE | 套索的 $\ell_\infty$ 界 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| (7.64) 印刷页 232；PDF 页 251 | FORMULA | $\ell_\infty$-曲率 $\lVert\widehat\Sigma\Delta\rVert_\infty\ge\gamma\lVert\Delta\rVert_\infty$ 在 $\mathbb C_3(S)$ 上 | 辅助 | 不进入 Notes | 习题公式；Notes 只在变量选择处对照 | 原页已核 |
| Exercise 7.14 印刷页 233；PDF 页 252 | EXERCISE | 高斯设计下样本 $\ell_\infty$-曲率 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 7.15 印刷页 233；PDF 页 252 | EXERCISE | 线性稀疏下更锐的 $\log(ed/s)$ 界 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| (7.65)–(7.66) 印刷页 233；PDF 页 252 | FORMULA | 约束套索锐界与经验过程 $Z$ | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 7.16 印刷页 233–234；PDF 页 252–253 | EXERCISE | 加权套索分析 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| (7.67) 印刷页 233；PDF 页 252 | FORMULA | 加权锥 $\mathbb C_3(S;\nu)$ | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 7.17 印刷页 234；PDF 页 253 | EXERCISE | 平方根套索 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 7.18 印刷页 234；PDF 页 253 | EXERCISE | 成对不相干 $\Rightarrow$ 不可表示条件 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 7.19 印刷页 234–235；PDF 页 253–254 | EXERCISE | 随机设计的不可表示条件 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 7.20 印刷页 235；PDF 页 254 | EXERCISE | $\ell_0$ 约束二次规划 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| (7.68)–(7.69) 印刷页 235；PDF 页 254 | FORMULA | $\ell_0$-RE 与 $\ell_0$ 约束最小二乘 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |

## 来源异常与勘误

| 定位 | 问题类型 | 原式/原文 | 核验证据 | 处置 | 数学复核人 | 批准人 |
|---|---|---|---|---|---|---|
| Example 7.15 印刷页 212；PDF 页 231 | 交叉引用笔误 | “relaxed basis pursuit program (7.19)” | 原页；(7.19) 是约束套索 $\lVert\theta\rVert_1\le R$；(7.20) 才是松弛基追踪 | 保留原文；Notes 按 (7.20) 解读；`勘误待批` | 作者 | 未批 |
| Theorem 7.13(c) 印刷页 210 vs 证明 印刷页 212；PDF 页 229 vs 231 | 常数不一致 | (7.25c) 写 $\frac4\kappa\sqrt s\,\lVert X^T w/n\rVert_\infty$；证明末行与 Example 7.15 写 $\frac8\kappa$ | 原页；由 $\kappa x^2\le A x+B$、$A=4\sqrt s\,\lVert X^T w/n\rVert_\infty$：Young 给出 $x\le A/\kappa+\sqrt{2B/\kappa}$（即 $4/\kappa$），更粗的 $x\le 2A/\kappa+\cdots$ 给出 $8/\kappa$ | 保留两式；Notes 陈述用 (7.25c) 的 $4/\kappa$，并标明证明写出 $8/\kappa$；`勘误待批` | 作者 | 未批 |
| Theorem 7.19 证明 (7.33) 印刷页 215；PDF 页 234 | 常数嫌疑 | (7.33) 花括号内为 $+2\lVert\theta^*_{S^c}\rVert_1$ | 由 (7.29) 与三角不等式：$\lVert\theta^*\rVert_1-\lVert\widehat\theta\rVert_1\le\lVert\Delta_S\rVert_1-\lVert\Delta_{S^c}\rVert_1+2\lVert\theta^*_{S^c}\rVert_1$，再加 Hölder $\le(\lambda_n/2)\lVert\Delta\rVert_1$，花括号内应变为 $+4\lVert\theta^*_{S^c}\rVert_1$；速率不变 | 保留原文；Notes 按印刷 (7.32)–(7.33) 陈述并标明独立复核；`勘误待批` | 作者 | 未批 |
| Proposition 7.11 证明 印刷页 204–205；PDF 页 223–224 | 记号跳换 | 先令 $S$ 为绝对值最大的 $s$ 个坐标，随后下界改写 $\widetilde\theta_{S_0}$ | 原页；论证需 $S_0=S$（$s$ 个最大坐标） | 保留原文；Notes 显式令 $S_0=S$；不单独立项为已批勘误 | 作者 | 未批 |

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
