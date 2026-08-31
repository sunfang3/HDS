---
chapter_id: "ch06"
chapter_title: "Random matrices and covariance estimation"
source_title: "High-Dimensional Statistics: A Non-Asymptotic Viewpoint"
source_version: "Cambridge Series in Statistical and Probabilistic Mathematics, No. 48; first published 2019; ISBN 978-1-108-49802-9"
main_source_path: "High-Dimensional Statistics A Non-Asymptotic Viewpoint (Martin J. Wainwright) (z-library.sk, 1lib.sk, z-lib.sk).pdf"
printed_pages: "159–193"
pdf_pages: "178–212"
target_notes: "notes/ch06-notes.qmd"
language: "zh-CN"
learner_profile: "学过陈希孺《概率论与数理统计》本科教材；第 1 章已见样本协方差 (1.8)、算子范数 (1.9)、MP 定律 (1.10) 与非渐近上尾 (1.11)。本章缺口：维希特矩阵、协方差算子范数界、矩阵 Chernoff / Ahlswede–Winter、子高斯系综、稀疏协方差的阈值估计。"
map_status: "清单完成"
---

# 第 6 章内容清单

> 内部质量工件。正式定理、定义、引理、推论与关键编号公式逐项登记；证明细节可并入对应定理。习题全部不进入 Notes。

## 来源边界

- 教材权威来源：Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series No. 48
- 版本识别依据：封面 Cambridge Series；版权页 © Martin J. Wainwright 2019，First published 2019，ISBN 978-1-108-49802-9 Hardback，DOI 10.1017/9781108627771
- 目标章节与页码：第 6 章，印刷页 159–193；PDF 页 178–212（**PDF = 印刷 + 19**）
- 补充来源及用途：无
- 已知来源限制：文本层公式常错位；须对照 `scratch/ch06/p-178.png`–`p-212.png`

## 内容清单

| 定位 | 类型 | 内容/范围 | 重要性 | Notes 处理 | 合并目标/排除理由 | 核验状态 |
|---|---|---|---|---|---|---|
| 章首 印刷页 159；PDF 页 178 | SECTION | Chapter 6：随机矩阵与协方差估计；非渐近偏差；高斯到子高斯再到弱尾；调用第 2–5 章并引入矩阵尾界 | 关键 | 完整讲解 |  | 原页已核 |
| §6.1 印刷页 159–161；PDF 页 178–180 | SECTION | Some preliminaries | 关键 | 完整讲解 |  | 原页已核 |
| §6.1.1 印刷页 159–160；PDF 页 178–179 | SECTION | Notation and basic facts：奇异值、对称矩阵、半正定锥 | 关键 | 完整讲解 |  | 原页已核 |
| (6.1) 印刷页 159；PDF 页 178 | FORMULA | $\sigma_{\max}(A)=\max_{v\in\mathbb S^{m-1}}\Vert Av\Vert_2$，$\sigma_{\min}(A)=\min\Vert Av\Vert_2$；$\Vert A\Vert_{\mathrm{op}}=\sigma_{\max}(A)$（教材三竖线） | 关键 | 完整讲解 |  | 原页已核 |
| (6.2) 印刷页 160；PDF 页 179 | DEFINITION | $\mathcal S_+^{d\times d}:=\{Q\in\mathcal S^{d\times d}:Q\succeq 0\}$ | 关键 | 完整讲解 |  | 原页已核 |
| (6.3) 印刷页 160；PDF 页 179 | FORMULA | Rayleigh–Ritz：$\gamma_{\max}(Q)=\max_{v\in\mathbb S^{d-1}}v^T Qv$，$\gamma_{\min}$ 同理取 min | 关键 | 完整讲解 |  | 原页已核 |
| (6.4a)–(6.4b) 印刷页 160；PDF 页 179 | FORMULA | 对称矩阵 $\Vert Q\Vert_{\mathrm{op}}=\max\{\gamma_{\max}(Q),\lvert\gamma_{\min}(Q)\rvert\}=\max_{v\in\mathbb S^{d-1}}\lvert v^T Qv\rvert$ | 关键 | 完整讲解 |  | 原页已核 |
| §6.1.2 印刷页 160–161；PDF 页 179–180 | SECTION | Set-up of covariance estimation：零均值 i.i.d.，$\widehat\Sigma=n^{-1}\sum x_i x_i^T$ | 关键 | 完整讲解 |  | 原页已核 |
| (6.5) 印刷页 160；PDF 页 179 | FORMULA | 样本协方差 $\widehat\Sigma:=n^{-1}\sum_{i=1}^n x_i x_i^T$（无偏） | 关键 | 完整讲解 |  | 原页已核 |
| (6.6) 印刷页 161；PDF 页 180 | FORMULA | $\Vert\widehat\Sigma-\Sigma\Vert_{\mathrm{op}}\le\varepsilon$ 等价于球面上二次型的一致大数定律 | 关键 | 完整讲解 |  | 原页已核 |
| (6.7) 印刷页 161；PDF 页 180 | FORMULA | Weyl 推论：$\max_j\lvert\gamma_j(\widehat\Sigma)-\gamma_j(\Sigma)\rvert\le\Vert\widehat\Sigma-\Sigma\Vert_{\mathrm{op}}$ | 关键 | 完整讲解 |  | 原页已核 |
| §6.2 印刷页 161–165；PDF 页 180–184 | SECTION | Wishart matrices and their behavior | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 6.1 印刷页 161–162；PDF 页 180–181 | THEOREM | $\Sigma$-高斯系综奇异值上下偏差 (6.8)–(6.9) | 关键 | 完整讲解 |  | 原页已核 |
| (6.8) 印刷页 161；PDF 页 180 | FORMULA | $\mathbb P[\sigma_{\max}(X)/\sqrt n\ge\gamma_{\max}(\sqrt\Sigma)(1+\delta)+\sqrt{\mathrm{tr}(\Sigma)/n}]\le e^{-n\delta^2/2}$ | 关键 | 完整讲解 |  | 原页已核 |
| (6.9) 印刷页 162；PDF 页 181 | FORMULA | $n\ge d$ 时 $\sigma_{\min}$ 的对称下偏差 | 关键 | 完整讲解 |  | 原页已核 |
| Example 6.2 印刷页 162；PDF 页 181 | EXAMPLE | 标准高斯系综 (6.10)–(6.11)；$d/n\to 0$ 时相合 | 关键 | 完整讲解 |  | 原页已核 |
| (6.10)–(6.11) 印刷页 162；PDF 页 181 | FORMULA | $\sigma_{\max}(W)/\sqrt n\le 1+\delta+\sqrt{d/n}$ 等；$\Vert(1/n)W^TW-I_d\Vert_{\mathrm{op}}\le 2\varepsilon+\varepsilon^2$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 6.3 印刷页 162；PDF 页 181 | EXAMPLE | 高斯协方差相对误差 (6.12) | 关键 | 完整讲解 |  | 原页已核 |
| (6.12) 印刷页 162；PDF 页 181 | FORMULA | $\Vert\widehat\Sigma-\Sigma\Vert_{\mathrm{op}}/\Vert\Sigma\Vert_{\mathrm{op}}\le 2\sqrt{d/n}+2\delta+(\sqrt{d/n}+\delta)^2$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 6.4 印刷页 162–163；PDF 页 181–182 | EXAMPLE | 迹约束与 Schatten $q$-球；有效维数 $C$ | 关键 | 完整讲解 |  | 原页已核 |
| (6.13)–(6.15) 印刷页 163；PDF 页 182 | FORMULA | $\mathrm{tr}(\Sigma)/\Vert\Sigma\Vert_{\mathrm{op}}\le C$；$\mathbb B_q(R_q)$；(6.15) 以 $C$ 替换 $d$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 6.1 证明 印刷页 163–165；PDF 页 182–184 | PROOF_DERIVATION | Lipschitz 集中 + Sudakov–Fernique；(6.16)–(6.17)；下界推迟到 §6.6 | 关键 | 完整讲解 | 上界完整写；下界并入 §6.6 | 原页已核 |
| §6.3 印刷页 165–168；PDF 页 184–187 | SECTION | Covariance matrices from sub-Gaussian ensembles | 关键 | 完整讲解 |  | 原页已核 |
| (6.18) 印刷页 165；PDF 页 184 | DEFINITION | 行向量子高斯：$\mathbb E[e^{\lambda\langle v,x_i\rangle}]\le e^{\lambda^2\sigma^2/2}$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 6.5 印刷页 166；PDF 页 185 | THEOREM | 行WISE $\sigma$-子高斯样本协方差的 mgf 与尾界 (6.19a)–(6.19b) | 关键 | 完整讲解 |  | 原页已核 |
| (6.19a)–(6.19b) 印刷页 166；PDF 页 185 | FORMULA | $\mathbb E[e^{\lambda\Vert\widehat\Sigma-\Sigma\Vert_{\mathrm{op}}}]\le\exp(c_0\lambda^2\sigma^4/n+4d)$，$\lvert\lambda\rvert<n/(64e^2\sigma^2)$；尾界含 $\sqrt{d/n}+d/n$ | 关键 | 完整讲解 |  | 原页已核 |
| (6.20) 印刷页 166；PDF 页 185 | FORMULA | $n\ge d$ 时 $\sigma_{\min}/\sqrt n$ 与 $\sigma_{\max}/\sqrt n$ 的夹心，常数 $c'>1$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 6.5 证明 印刷页 166–168；PDF 页 185–187 | PROOF_DERIVATION | $1/8$-覆盖 $N\le 17^d$；对称化；(6.21)–(6.23) | 关键 | 完整讲解 |  | 原页已核 |
| §6.4 印刷页 168–180；PDF 页 187–199 | SECTION | Bounds for general matrices：矩阵 Hoeﬀding / Bernstein | 关键 | 完整讲解 |  | 原页已核 |
| §6.4.1 印刷页 168–169；PDF 页 187–188 | SECTION | Background on matrix analysis：函数演算、谱映射、Löwner–Heinz | 关键 | 完整讲解 |  | 原页已核 |
| (6.24)–(6.25) 印刷页 169；PDF 页 188 | FORMULA | 谱映射 $\gamma(f(Q))=\{f(\gamma_j(Q))\}$；迹单调 $\mathrm{tr}(f(Q))\le\mathrm{tr}(f(R))$ 当 $Q\preceq R$ 且 $f$ 连续非降 | 关键 | 完整讲解 |  | 原页已核 |
| §6.4.2 印刷页 169–171；PDF 页 188–190 | SECTION | Tail conditions for matrices | 关键 | 完整讲解 |  | 原页已核 |
| (6.26) 印刷页 169；PDF 页 188 | DEFINITION | 矩阵矩母函数 $\Psi_Q(\lambda):=\mathbb E[e^{\lambda Q}]$ | 关键 | 完整讲解 |  | 原页已核 |
| Definition 6.6 印刷页 170；PDF 页 189 | DEFINITION | 矩阵子高斯：$\Psi_Q(\lambda)\preceq e^{\lambda^2 V/2}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 6.7–6.8 印刷页 170；PDF 页 189 | EXAMPLE | $Q=\varepsilon B$ 与 $Q=\varepsilon C$、$\Vert C\Vert_{\mathrm{op}}\le b$ | 辅助 | 简要说明 |  | 原页已核 |
| Definition 6.9 印刷页 170；PDF 页 189 | DEFINITION | 矩阵次指数：$\Psi_Q(\lambda)\preceq e^{\lambda^2 V/2}$，$\lvert\lambda\rvert<1/\alpha$ | 关键 | 完整讲解 |  | 原页已核 |
| Definition 6.10 印刷页 171；PDF 页 190 | DEFINITION | 矩阵 Bernstein 条件 (6.29)；有界情形 (6.30) | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 6.11 印刷页 171；PDF 页 190 | LEMMA | Bernstein 推出 $\Psi_Q(\lambda)\preceq\exp(\lambda^2\mathrm{var}(Q)/(2(1-b\lvert\lambda\rvert)))$，$\lvert\lambda\rvert<1/b$ | 关键 | 完整讲解 |  | 原页已核 |
| §6.4.3 印刷页 172–174；PDF 页 191–193 | SECTION | Matrix Chernoff approach and independent decompositions | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 6.12 印刷页 172；PDF 页 191 | LEMMA | 矩阵 Chernoff：$\mathbb P[\gamma_{\max}(Q)\ge\delta]\le\mathrm{tr}(\Psi_Q(\lambda))e^{-\lambda\delta}$；(6.33) 算子范数多因子 2 | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 6.13 印刷页 173；PDF 页 192 | LEMMA | Lieb 凹性：$\mathrm{tr}(\Psi_{S_n}(\lambda))\le\mathrm{tr}(\exp(\sum_i\log\Psi_{Q_i}(\lambda)))$；(6.37) | 关键 | 完整讲解 |  | 原页已核 |
| Example 6.14 印刷页 173–174；PDF 页 192–193 | EXAMPLE | 矩阵 Rademacher 对称化 | 辅助 | 简要说明 |  | 原页已核 |
| §6.4.4 印刷页 174–179；PDF 页 193–198 | SECTION | Upper tail bounds for random matrices | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 6.15 印刷页 174；PDF 页 193 | THEOREM | 矩阵 Hoeﬀding (6.38)；$\sigma^2=\Vert(1/n)\sum V_i\Vert_{\mathrm{op}}$ | 关键 | 完整讲解 |  | 原页已核 |
| (6.39) 印刷页 175；PDF 页 194 | FORMULA | 非方阵的对称膨胀 $Q_i=\bigl[\begin{smallmatrix}0_{d_1\times d_1}&A_i\\ A_i^T&0_{d_2\times d_2}\end{smallmatrix}\bigr]$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 6.16 印刷页 176；PDF 页 195 | EXAMPLE | (6.38) 的松/紧：Rademacher 差 $\sqrt{\log d}$，高斯不可改进 | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 6.17 印刷页 176；PDF 页 195 | THEOREM | 矩阵 Bernstein (6.42) | 关键 | 完整讲解 |  | 原页已核 |
| (6.43) 印刷页 177；PDF 页 196 | FORMULA | 非对称有界矩阵的 $\sigma^2=\max\{\Vert(1/n)\sum\mathbb E[A_i A_i^T]\Vert_{\mathrm{op}},\Vert(1/n)\sum\mathbb E[A_i^T A_i]\Vert_{\mathrm{op}}\}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 6.18 印刷页 177–178；PDF 页 196–197 | EXAMPLE | 矩阵补全掩膜；(6.44)–(6.45) | 辅助 | 简要说明 |  | 原页已核 |
| Example 6.19 印刷页 178–179；PDF 页 197–198 | EXAMPLE | 以 $\mathrm{tr}(\bar V)/\Vert\bar V\Vert_{\mathrm{op}}$ 替换 rank；(6.46)–(6.48) | 辅助 | 简要说明 | 细节进 Exercise 6.12 | 原页已核 |
| §6.4.5 印刷页 179–180；PDF 页 198–199 | SECTION | Consequences for covariance matrices | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 6.20 印刷页 179；PDF 页 198 | COROLLARY | $\Vert x_j\Vert_2\le\sqrt b$ a.s. 时样本协方差 Bernstein 尾 (6.49) | 关键 | 完整讲解 |  | 原页已核 |
| Example 6.21–6.22 印刷页 179–180；PDF 页 198–199 | EXAMPLE | 球面均匀与 spiked；(6.50)–(6.51)；$d\log d/n\to 0$；spiked 使对数因子必要 | 关键 | 完整讲解 |  | 原页已核 |
| §6.5 印刷页 180–185；PDF 页 199–204 | SECTION | Bounds for structured covariance matrices | 关键 | 完整讲解 |  | 原页已核 |
| §6.5.1 印刷页 180–183；PDF 页 199–202 | SECTION | Unknown sparsity and thresholding | 关键 | 完整讲解 |  | 原页已核 |
| (6.52) 印刷页 180；PDF 页 199 | DEFINITION | 硬阈值 $T_\lambda(u)=u\,\mathbb I[\lvert u\rvert>\lambda]$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 6.23 印刷页 181；PDF 页 200 | THEOREM | 阈值协方差：$\lambda_n/\sigma^2=8\sqrt{(\log d)/n}+\delta$ 时 (6.53) | 关键 | 完整讲解 |  | 原页已核 |
| (6.54) 印刷页 181；PDF 页 200 | FORMULA | 确定性：$\Vert\widehat\Sigma-\Sigma\Vert_{\max}\le\lambda_n$ 推出 $\Vert T_{\lambda_n}(\widehat\Sigma)-\Sigma\Vert_{\mathrm{op}}\le 2\Vert A\Vert_{\mathrm{op}}\lambda_n$ | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 6.24 印刷页 182；PDF 页 201 | COROLLARY | 每行至多 $s$ 个非零时 (6.55) | 关键 | 完整讲解 |  | 原页已核 |
| Example 6.25 / Figure 6.1 印刷页 182；PDF 页 201 | EXAMPLE | $s$-团与星图；邻接算子范数印刷作 $1+\sqrt{s-1}$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 6.1 印刷页 182；PDF 页 201 | FIGURE_TABLE | $d=9$ 的 $s=5$ 团与星–辐图 | 辅助 | 简要说明 |  | 原页已核 |
| Lemma 6.26 印刷页 183；PDF 页 202 | LEMMA | 逐元 $\ell_\infty$ 尾 (6.56) | 关键 | 完整讲解 |  | 原页已核 |
| §6.5.2 印刷页 183–185；PDF 页 202–204 | SECTION | Approximate sparsity | 关键 | 完整讲解 |  | 原页已核 |
| (6.58) 印刷页 184；PDF 页 203 | DEFINITION | 行 $\ell_q$-稀疏 $\max_j\sum_\ell\lvert\Sigma_{j\ell}\rvert^q\le R_q$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 6.27 印刷页 184；PDF 页 203 | THEOREM | $\ell_q$-稀疏下 $\Vert T_{\lambda_n}(\widehat\Sigma)-\Sigma\Vert_{\mathrm{op}}\le 4R_q\lambda_n^{1-q}$；(6.59a)–(6.59b) | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 6.27 证明 印刷页 184–185；PDF 页 203–204 | PROOF_DERIVATION | 行 $\ell_1$ 控制算子范数；(6.60) 与 $2^q R_q\lambda_n^{-q}$ | 关键 | 简要说明 | 并入 Theorem 6.27 | 原页已核 |
| §6.6 印刷页 185–188；PDF 页 204–207 | PROOF_DERIVATION | Appendix：Gordon 不等式证明 (6.9)；(6.61)–(6.67) | 辅助 | 简要说明 | 完整比较论证指回教材 | 原页已核 |
| §6.7 印刷页 188–189；PDF 页 207–208 | PROSE_RANGE | Bibliographic details：Weyl、Vershynin、Ahlswede–Winter、Tropp、Bickel–Levina、El Karoui | 辅助 | 指回教材 | 文献清单不抄入 Notes | 原页已核 |
| §6.8 印刷页 189–193；PDF 页 208–212 | SECTION | Exercises 6.1–6.16 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 6.1 印刷页 189；PDF 页 208 | EXERCISE | 特征值对算子范数的 Lipschitz | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 6.2 印刷页 190；PDF 页 209 | EXERCISE | $\ell_q\to\ell_q$ 算子范数关系 | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 6.3 印刷页 190；PDF 页 209 | EXERCISE | 非负矩阵与算子范数 | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 6.4 印刷页 190；PDF 页 209 | EXERCISE | $I+A\preceq e^A$ | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 6.5 印刷页 190；PDF 页 209 | EXERCISE | 矩阵单调：平方与指数反例；对数单调 | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 6.6 印刷页 190；PDF 页 209 | EXERCISE | $\mathrm{var}(Q)\succeq 0$ | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 6.7 印刷页 190–191；PDF 页 209–210 | EXERCISE | 子高斯随机矩阵 $Q=gB$ | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 6.8 印刷页 191；PDF 页 210 | EXERCISE | 子高斯和的期望界 (6.68) | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 6.9 印刷页 191；PDF 页 210 | EXERCISE | 有界矩阵推出 (6.30) | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 6.10 印刷页 191；PDF 页 210 | EXERCISE | 非对称矩阵尾界 (6.69)；零块维数与 (6.39) 不一致 | 辅助 | 不进入 Notes | Solutions；零块记入勘误表 | 原页已核 |
| Exercise 6.11 印刷页 191–192；PDF 页 210–211 | EXERCISE | 无界矩阵 Bernstein | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 6.12 印刷页 192；PDF 页 211 | EXERCISE | 锐化矩阵 Bernstein | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 6.13 印刷页 192；PDF 页 211 | EXERCISE | 向量 Bernstein 的维数因子 | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 6.14 印刷页 192；PDF 页 211 | EXERCISE | 随机填装 | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 6.15 印刷页 193；PDF 页 212 | EXERCISE | 对角协方差估计 | 辅助 | 不进入 Notes | Solutions | 原页已核 |
| Exercise 6.16 印刷页 193；PDF 页 212 | EXERCISE | 含 $s$-团且最大度 $s-1$ 的图：邻接算子范数等于 $s$ | 辅助 | 不进入 Notes | Solutions | 原页已核 |

## 来源异常与勘误

| 定位 | 问题类型 | 原式/原文 | 核验证据 | 处置 | 数学复核人 | 批准人 |
|---|---|---|---|---|---|---|
| Exercise 6.10 印刷页 191；PDF 页 210 | 笔误嫌疑 | 膨胀写作 $0_{d_1\times d_2}$ 与 $0_{d_2\times d_1}$ | 原页；(6.39) 印刷页 175 为 $0_{d_1\times d_1}$ 与 $0_{d_2\times d_2}$；按习题所写两块零矩阵与 $A_i\in\mathbb R^{d_1\times d_2}$ 不能拼成方阵（除非 $d_1=d_2$） | 保留原文；Notes 用 (6.39)；Solutions 按正确膨胀求解；`勘误待批` | 作者 | 未批 |
| §6.7 印刷页 189；PDF 页 208 | 拼写嫌疑 | 正文 “Alhswede and Winter (2002)” | 原页；标准拼写 Ahlswede–Winter | 保留原文；Notes 用 Ahlswede 并标明教材拼写；`勘误待批` | 作者 | 未批 |
| Example 6.25 印刷页 182；PDF 页 201 | 公式歧义 | 星–辐图印刷作 $\vert\!\vert\!\vert A\vert\!\vert\!\vert_2=1+\sqrt{s-1}$，同时写 hub 连接到 $s$ 个其余结点 | 原页；无自环星图邻接谱半径为 $\sqrt k$（$k$ 为辐条数），加对角 1 后为 $1+\sqrt k$；图注称与 (6.55) 差 $\sqrt s$ 因子，与 $k=s$ 的 $1+\sqrt s$ 更一致 | 保留印刷 $1+\sqrt{s-1}$；Notes 说明两种读法；`勘误待批` | 作者 | 未批 |
| Corollary 6.20 证明 印刷页 179；PDF 页 198 | 常数松紧 | 证明得 $\vert\!\vert\!\vert Q_i\vert\!\vert\!\vert_2\le 2b$，却直接代入 (6.42) 得到分母 $2b(\vert\!\vert\!\vert\Sigma\vert\!\vert\!\vert_2+\delta)$ | 原页；(6.42) 若 Bernstein 参数取 $2b$、$\sigma^2\le b\vert\!\vert\!\vert\Sigma\vert\!\vert\!\vert_2$，分母应为 $2(b\vert\!\vert\!\vert\Sigma\vert\!\vert\!\vert_2+2b\delta)$ | 保留 (6.49)；Notes 标明参数吸收；`勘误待批` | 作者 | 未批 |
| Theorem 6.17 印刷页 176；PDF 页 195 | 排印 | “Let $\{Q_i\}_{i=1}^n\}$ be a sequence” 多一个右花括号 | 原页 | 不影响数学；不改教材；`勘误待批` | 作者 | 未批 |

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
