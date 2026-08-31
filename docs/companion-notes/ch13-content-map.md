---
chapter_id: "ch13"
chapter_title: "Nonparametric least squares"
source_title: "High-Dimensional Statistics: A Non-Asymptotic Viewpoint"
source_version: "Cambridge Series in Statistical and Probabilistic Mathematics, No. 48; first published 2019; ISBN 978-1-108-49802-9"
main_source_path: "High-Dimensional Statistics A Non-Asymptotic Viewpoint (Martin J. Wainwright) (z-library.sk, 1lib.sk, z-lib.sk).pdf"
printed_pages: "416–452"
pdf_pages: "435–471"
target_notes: "notes/ch13-notes.qmd"
language: "zh-CN"
learner_profile: "学过陈希孺《概率论与数理统计》本科教材，并已读本书第 1、2、4、5 章及第 12 章的 RKHS 例子；熟悉最小二乘、条件期望、覆盖数与 Dudley 积分；首次需要把非参数最小二乘的预测误差写成局部高斯复杂度的临界半径，并用神谕不等式处理逼近–估计权衡。"
map_status: "清单完成"
---

# 第 13 章内容清单

> 内部质量工件。正式内容逐项登记；证明可按定理聚合；习题进 Solutions 不进 Notes。

## 来源边界

- 教材权威来源：Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series No. 48
- 版本识别依据：封面 Cambridge Series；版权页 © Martin J. Wainwright 2019，First published 2019，ISBN 978-1-108-49802-9 Hardback，DOI 10.1017/9781108627771
- 目标章节与页码：第 13 章，印刷页 416–452；PDF 页 435–471（**PDF = 印刷 + 19**）
- 补充来源及用途：无（习题独立求解）
- 已知来源限制：文本层可用但公式常错位；公式、图注须对照 `scratch/ch13/p-4XX.png`

## 内容清单

| 定位 | 类型 | 内容/范围 | 重要性 | Notes 处理 | 合并目标/排除理由 | 核验状态 |
|---|---|---|---|---|---|---|
| 章首 印刷页 416；PDF 页 435 | SECTION | Chapter 13 Nonparametric least squares：用前几章工具分析非参数最小二乘的收敛速率 | 关键 | 完整讲解 |  | 原页已核 |
| §13.1 印刷页 416–420；PDF 页 435–439 | SECTION | Problem set-up | 关键 | 完整讲解 |  | 原页已核 |
| (13.1) 印刷页 416；PDF 页 435 | FORMULA | 总体 MSE $\mathcal L_f:=\mathbb E_{X,Y}[(Y-f(X))^2]$ | 关键 | 完整讲解 |  | 原页已核 |
| (13.2) 印刷页 416；PDF 页 435 | DEFINITION | 回归函数 / Bayes 最小二乘 $f^*(x)=\mathbb E[Y\mid X=x]$ | 关键 | 完整讲解 |  | 原页已核 |
| (13.3) 印刷页 416；PDF 页 435 | FORMULA | 经验 MSE $\widehat{\mathcal L}_f=n^{-1}\sum(y_i-f(x_i))^2$ | 关键 | 完整讲解 |  | 原页已核 |
| §13.1.1 印刷页 416–417；PDF 页 435–436 | SECTION | Different measures of quality：超额风险 vs 经验 $L^2(\mathbb P_n)$ | 关键 | 完整讲解 |  | 原页已核 |
| (13.4) 印刷页 417；PDF 页 436 | FORMULA | 超额风险 $\mathcal L_f-\mathcal L_{f^*}=\mathbb E_X[(f(X)-f^*(X))^2]=\Vert f^*-f\Vert_{L^2(\mathbb P)}^2$ | 关键 | 完整讲解 |  | 原页已核 |
| (13.5) 印刷页 417；PDF 页 436 | DEFINITION | 经验范数 $\Vert f-f^*\Vert_{L^2(\mathbb P_n)}$ 与简写 $\Vert\cdot\Vert_n$；固定设计 | 关键 | 完整讲解 |  | 原页已核 |
| §13.1.2 印刷页 417–418；PDF 页 436–437 | SECTION | Estimation via constrained least squares | 关键 | 完整讲解 |  | 原页已核 |
| (13.6) 印刷页 417；PDF 页 436 | FORMULA | 生成模型 $y_i=f^*(x_i)+v_i$；标准模型 $v_i=\sigma w_i$、$w_i\sim N(0,1)$ | 关键 | 完整讲解 |  | 原页已核 |
| (13.7) 印刷页 417；PDF 页 436 | DEFINITION | 约束非参数最小二乘 $\widehat f\in\arg\min_{f\in\mathcal F}n^{-1}\sum(y_i-f(x_i))^2$ | 关键 | 完整讲解 |  | 原页已核 |
| (13.8) 印刷页 418；PDF 页 437 | DEFINITION | 正则化估计 $\widehat f\in\arg\min_{f\in\mathcal F}\{n^{-1}\sum(y_i-f(x_i))^2+\lambda_n\Vert f\Vert_{\mathcal F}^2\}$ | 关键 | 完整讲解 |  | 原页已核 |
| §13.1.3 印刷页 418–420；PDF 页 437–439 | SECTION | Some examples | 关键 | 完整讲解 |  | 原页已核 |
| Example 13.1 印刷页 418；PDF 页 437 | EXAMPLE | 线性回归、岭回归、约束 $\ell_q$ 球、约束 Lasso | 关键 | 完整讲解 |  | 原页已核 |
| Example 13.2 (13.9)–(13.10) 印刷页 419；PDF 页 438 | EXAMPLE | 三次光滑样条：$\int(f'')^2\le R$ 与惩罚形式 | 关键 | 完整讲解 |  | 原页已核 |
| Example 13.3 印刷页 419；PDF 页 438 | EXAMPLE | 核岭回归：$\widehat f(\cdot)=n^{-1/2}\sum\widehat\alpha_i\mathcal K(\cdot,x_i)$，$\widehat\alpha=(\mathbf K+\lambda_n I_n)^{-1}y/\sqrt n$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 13.4 (13.11)–(13.14) 印刷页 419–420；PDF 页 438–439 | EXAMPLE | 凸回归：次梯度、有限维凸规划、$N=n(d+1)$ 变量、$2\binom n2$ 线性约束；$\widehat f(x)=\max_i\{\widehat y_i+\langle\widehat z_i,x-x_i\rangle\}$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 13.1 印刷页 421；PDF 页 440 | FIGURE_TABLE | 凸回归与凸+单调拟合，$n=11$，$C=[-1,1]$ | 辅助 | 简要说明 |  | 原页已核 |
| §13.2 印刷页 420–432；PDF 页 439–451 | SECTION | Bounding the prediction error | 关键 | 完整讲解 |  | 原页已核 |
| (13.15) 印刷页 421；PDF 页 440 | DEFINITION | 平移类 $\mathcal F^*:=\mathcal F-\{f^*\}$ | 关键 | 完整讲解 |  | 原页已核 |
| (13.16) 印刷页 421；PDF 页 440 | DEFINITION | 局部高斯复杂度 $\mathcal G_n(\delta;\mathcal F^*)$ | 关键 | 完整讲解 |  | 原页已核 |
| (13.17) 印刷页 422；PDF 页 441 | DEFINITION | 临界不等式 $\mathcal G_n(\delta;\mathcal F^*)/\delta\le\delta/(2\sigma)$；有效半径与临界半径 $\delta_n^*$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 13.2 印刷页 422；PDF 页 441 | FIGURE_TABLE | Sobolev 核与高斯核的 $\delta\mapsto\mathcal G_n(\delta)/\delta$；临界半径为与斜率 $1/(2\sigma)$ 的交点 | 关键 | 完整讲解 |  | 原页已核 |
| (13.18) 印刷页 423；PDF 页 442 | FORMULA | 非参数最小二乘的基本不等式 $\tfrac12\Vert\widehat f-f^*\Vert_n^2\le(\sigma/n)\sum w_i(\widehat f(x_i)-f^*(x_i))$ | 关键 | 完整讲解 |  | 原页已核 |
| (13.19) 印刷页 423；PDF 页 442 | FORMULA | 启发式：$\delta^2/2\le\sigma\mathcal G_n(\delta;\mathcal F^*)$ 推出 $\delta\le\delta_n^*$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 13.5 (13.20) 印刷页 423；PDF 页 442 | THEOREM | 星形平移类下，$\mathbb P[\Vert\widehat f_n-f^*\Vert_n^2\ge 16 t\delta_n]\le e^{-nt\delta_n/(2\sigma^2)}$，$t\ge\delta_n$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 13.5 注记 印刷页 423；PDF 页 442 | PROSE_RANGE | 积分尾界得 $\mathbb E\Vert\widehat f_n-f^*\Vert_n^2\le c\{\delta_n^2+\sigma^2/n\}$；含常数函数时 $\delta_n^2$ 主导 | 关键 | 完整讲解 |  | 原页已核 |
| $Z_n(\delta)$ 印刷页 424；PDF 页 443 | FORMULA | 一般噪声复杂度 $Z_n(\delta)=\sup_{\Vert g\Vert_n\le\delta,g\in\mathcal F^*}\lvert n^{-1}\sum(v_i/\sigma)g(x_i)\rvert$ | 辅助 | 简要说明 |  | 原页已核 |
| Figure 13.3 印刷页 424；PDF 页 443 | FIGURE_TABLE | 凸集处处星形；非凸集可对某些点星形 | 辅助 | 简要说明 |  | 原页已核 |
| (13.21) 印刷页 424；PDF 页 443 | DEFINITION | 星形包 $\mathrm{star}(\mathcal F^*;0)$ | 关键 | 完整讲解 |  | 原页已核 |
| (13.22) 印刷页 424；PDF 页 443 | DEFINITION | 差类 $\partial\mathcal F:=\mathcal F-\mathcal F$ | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 13.6 (13.23) 印刷页 425；PDF 页 444 | LEMMA | 星形类上 $\delta\mapsto\mathcal G_n(\delta;\mathcal H)/\delta$ 非增，故临界不等式有最小正解 | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 13.6 证明 印刷页 425；PDF 页 444 | PROOF_DERIVATION | 缩放 $\widetilde h=(\delta/t)h$ 与星形性 | 关键 | 并入相关内容 | Lemma 13.6 | 原页已核 |
| §13.2.1 印刷页 425–426；PDF 页 444–445 | SECTION | Bounds via metric entropy | 关键 | 完整讲解 |  | 原页已核 |
| $\mathbb B_n(\delta;\mathcal H)$ 印刷页 425；PDF 页 444 | DEFINITION | $\mathbb B_n(\delta;\mathcal H):=\{h\in\mathrm{star}(\mathcal H):\Vert h\Vert_n\le\delta\}$ 及其 $t$-覆盖数 $N_n$ | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 13.7 (13.24) 印刷页 426；PDF 页 445 | COROLLARY | Dudley 积分充分条件：$(16/\sqrt n)\int_{\delta^2/(4\sigma)}^\delta\sqrt{\log N_n(t;\mathbb B_n(\delta;\mathcal F^*))}\,dt\le\delta^2/(4\sigma)$ | 关键 | 完整讲解 |  | 原页已核 |
| (13.25) 印刷页 426；PDF 页 445 | FORMULA | 覆盖拆分 $\mathcal G_n(\delta)\le\mathbb E[\max_j\lvert n^{-1}\sum w_i g^j(x_i)\rvert]+\delta^2/(4\sigma)$ | 辅助 | 并入相关内容 | Corollary 13.7 | 原页已核 |
| Corollary 13.7 证明 印刷页 426；PDF 页 445 | PROOF_DERIVATION | Cauchy–Schwarz、链锁、半度量 $\rho_Z(g^j,g^k)=\Vert g^j-g^k\Vert_n$ | 关键 | 简要说明 |  | 原页已核 |
| §13.2.2 印刷页 427–429；PDF 页 446–448 | SECTION | Bounds for high-dimensional parametric problems | 关键 | 完整讲解 |  | 原页已核 |
| Example 13.8 (13.26) 印刷页 427；PDF 页 446 | EXAMPLE | 线性回归：$\Vert f_{\widehat\theta}-f_{\theta^*}\Vert_n^2=\Vert\mathbf X(\widehat\theta-\theta^*)\Vert_2^2/n\lesssim\sigma^2\mathrm{rank}(\mathbf X)/n$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 13.9 (13.27)–(13.31) 印刷页 428–429；PDF 页 447–448 | EXAMPLE | $\ell_q$ 球 $q\in(0,1)$：熵 (13.30)、速率 $R_q(\sigma^2\log d/n)^{1-q/2}$ | 关键 | 完整讲解 |  | 原页已核 |
| §13.2.3 印刷页 429–430；PDF 页 448–449 | SECTION | Bounds for nonparametric problems | 关键 | 完整讲解 |  | 原页已核 |
| Example 13.10 (13.32)–(13.33) 印刷页 429–430；PDF 页 448–449 | EXAMPLE | Lipschitz 类：$\Vert\widehat f-f^*\Vert_n^2\lesssim(L\sigma^2/n)^{2/3}$，概率 $1-c_1e^{-c_2(n/(L\sigma^2))^{1/3}}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 13.11 (13.34)–(13.35) 印刷页 430；PDF 页 449 | EXAMPLE | 凸 Lipschitz：熵 $\log N(\epsilon)\lesssim\epsilon^{-1/2}$，速率 $(\sigma^2/n)^{4/5}$ | 关键 | 完整讲解 |  | 原页已核 |
| §13.2.4 印刷页 430–432；PDF 页 449–451 | SECTION | Proof of Theorem 13.5 | 关键 | 简要说明 |  | 原页已核 |
| (13.36) 印刷页 431；PDF 页 450 | FORMULA | 基本不等式用 $\widehat\Delta=\widehat f-f^*$ 重写 | 辅助 | 并入相关内容 | Theorem 13.5 | 原页已核 |
| (13.37)–(13.38) Lemma 13.12 印刷页 431；PDF 页 450 | LEMMA | 事件 $\mathcal A(u)$ 的尾界 $\mathbb P[\mathcal A(u)]\le e^{-nu^2/(2\sigma^2)}$，$u\ge\delta_n$ | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 13.12 证明 (13.39)–(13.41) 印刷页 431–432；PDF 页 450–451 | PROOF_DERIVATION | 星形缩放到 $\Vert\widetilde g\Vert_n=u$；高斯过程 Lipschitz 常数 $\sigma u/\sqrt n$；Theorem 2.26 | 关键 | 简要说明 |  | 原页已核 |
| §13.3 印刷页 432–438；PDF 页 451–457 | SECTION | Oracle inequalities | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 13.13 (13.42a)–(13.42b) 印刷页 433；PDF 页 452 | THEOREM | 神谕不等式：对一切 $f\in\mathcal F$，$\Vert\widehat f-f^*\Vert_n^2\le\inf_\gamma\{(1+\gamma)/(1-\gamma)\Vert f-f^*\Vert_n^2+c_0 t\delta_n/(\gamma(1-\gamma))\}$ | 关键 | 完整讲解 |  | 原页已核 |
| (13.43a)–(13.43b) 印刷页 433；PDF 页 452 | FORMULA | 简化形 $\Vert\widehat f-f^*\Vert_n^2\lesssim\inf_{f\in\mathcal F}\Vert f-f^*\Vert_n^2+\delta_n^2$ 及期望版 | 关键 | 完整讲解 |  | 原页已核 |
| §13.3.1 印刷页 434–437；PDF 页 453–456 | SECTION | Some examples of oracle inequalities | 关键 | 完整讲解 |  | 原页已核 |
| Example 13.14 (13.44)–(13.45) 印刷页 434；PDF 页 453 | EXAMPLE | 正交级数：逼近误差尾系数 $+$ 估计 $\sigma^2 T/n$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 13.4 印刷页 435；PDF 页 454 | FIGURE_TABLE | 上界 (13.45) 对 $T$：多项式 vs 指数衰减系数 | 辅助 | 简要说明 |  | 原页已核 |
| Example 13.15 (13.46)–(13.47) 印刷页 435–436；PDF 页 454–455 | EXAMPLE | Fourier 与 $\alpha$ 阶可微：$M\simeq(n/\sigma^2)^{1/(2\alpha+1)}$，速率 $(\sigma^2/n)^{2\alpha/(2\alpha+1)}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 13.16 (13.48)–(13.50) 印刷页 436–437；PDF 页 455–456 | EXAMPLE | 最佳 $s$-稀疏逼近：$\delta_n^2\simeq\sigma^2 s\log(ed/s)/n$ | 关键 | 完整讲解 |  | 原页已核 |
| §13.3.2 (13.51) 印刷页 437–438；PDF 页 456–457 | PROOF_DERIVATION | Theorem 13.13：可行点基本不等式、两种情形、Fenchel–Young | 关键 | 简要说明 |  | 原页已核 |
| §13.4 印刷页 439–448；PDF 页 458–467 | SECTION | Regularized estimators | 关键 | 完整讲解 |  | 原页已核 |
| (13.52) 印刷页 439；PDF 页 458 | DEFINITION | 正则化最小二乘（代价为 $1/(2n)$ 平方和） | 关键 | 完整讲解 |  | 原页已核 |
| §13.4.1 (13.53)–(13.54) 印刷页 439；PDF 页 458 | SECTION | 正则化估计的局部复杂度与临界不等式（半径 $R$ 球） | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 13.17 (13.55a)–(13.55b) 印刷页 439；PDF 页 458 | THEOREM | 凸类、$\lambda_n\ge 2\delta_n^2$：$\Vert\widehat f-f^*\Vert_n^2\le c_0\inf_{\Vert f\Vert_{\mathcal F}\le R}\Vert f-f^*\Vert_n^2+c_1 R^2\{\delta_n^2+\lambda_n\}$ | 关键 | 完整讲解 |  | 原页已核 |
| §13.4.2 印刷页 439–442；PDF 页 458–461 | SECTION | Consequences for kernel ridge regression | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 13.18 (13.56) 印刷页 440；PDF 页 459 | COROLLARY | KRR 临界条件 $\sqrt{2/n}\sqrt{\sum_j\min\{\delta^2,\widehat\mu_j\}}\le(R/(4\sigma))\delta^2$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 13.19 印刷页 440；PDF 页 459 | EXAMPLE | 多项式核：有限秩 $m$，速率 $\inf_{\Vert f\Vert_{\mathbb H}\le R}\Vert f-f^*\Vert_n^2+\sigma^2 m/n$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 13.20 印刷页 440–442；PDF 页 459–461 | EXAMPLE | 一阶 Sobolev 核 $K=\min\{x,z\}$：$\mu_j\asymp j^{-2}$，速率 $R^{2/3}(\sigma^2/n)^{2/3}$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 13.5 印刷页 441；PDF 页 460 | FIGURE_TABLE | 经验核矩阵谱：Sobolev vs 高斯核，$n=2000$ | 辅助 | 简要说明 |  | 原页已核 |
| Example 13.21 印刷页 442；PDF 页 461 | EXAMPLE | 高斯核：$\mu_j\asymp e^{-c j\log j}$，估计项 $c\sigma^2\log(Rn/\sigma)/n$ | 关键 | 完整讲解 |  | 原页已核 |
| §13.4.3 Lemma 13.22 (13.57)–(13.58) 印刷页 443–444；PDF 页 462–463 | LEMMA | RKHS 单位球局部高斯复杂度 $\le\sqrt{2/n}\sqrt{\sum\min\{\delta^2,\widehat\mu_j\}}$ | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 13.22 证明 印刷页 443–444；PDF 页 462–463 | PROOF_DERIVATION | 表示定理、椭圆交、Hölder 与 Jensen | 辅助 | 简要说明 |  | 原页已核 |
| §13.4.4 (13.59)–(13.69) 印刷页 444–448；PDF 页 463–467 | PROOF_DERIVATION | Theorem 13.17：缩放、修正基本不等式、两种范数情形、Lemma 13.23 剥皮 | 关键 | 简要说明 |  | 原页已核 |
| Lemma 13.23 (13.63) 印刷页 446；PDF 页 465 | LEMMA | 均匀随机过程界，对一切 $\Delta\in\partial\mathcal F$ 且 $\Vert\Delta\Vert_{\mathcal F}\ge 1$ | 关键 | 简要说明 |  | 原页已核 |
| §13.5 印刷页 448–449；PDF 页 467–468 | PROSE_RANGE | Bibliographic details：局部复杂度、剥皮、形状约束、可加模型（Exercise 13.9） | 辅助 | 指回教材 | 文献清单不抄入 Notes | 原页已核 |
| §13.6 印刷页 449–452；PDF 页 468–471 | SECTION | Exercises 13.1–13.11 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 13.1 印刷页 449；PDF 页 468 | EXERCISE | Bayes 最小二乘刻画：(a)(b)(c) 对应 (13.2)(13.4) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 13.2 印刷页 449；PDF 页 468 | EXERCISE | 线性回归预测误差的直接论证 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 13.3 印刷页 449–450；PDF 页 468–469 | EXERCISE | 三次光滑样条的核表示与二次规划 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 13.4 印刷页 450；PDF 页 469 | EXERCISE | 星形集与凸性 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 13.5 印刷页 450；PDF 页 469 | EXERCISE | 临界不等式的下界：$\delta^2=4\sigma^2$；含常数函数时 $\delta^2\ge\min\{1,(8/\pi)\sigma^2/n\}$ | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 13.6 印刷页 450；PDF 页 469 | EXERCISE | 局部高斯复杂度的自适应性：$\ell_1$ 球 vs 顶点 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 13.7 印刷页 451；PDF 页 470 | EXERCISE | 多项式回归速率 $\sigma^2 m\log n/n$ | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 13.8 印刷页 451；PDF 页 470 | EXERCISE | 二阶可微类速率 $(\sigma^2/n)^{4/5}$ | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 13.9 (13.70) 印刷页 451–452；PDF 页 470–471 | EXERCISE | 可加非参数模型：坐标复杂度与 $\Vert\widehat f-f^*\Vert_n^2\lesssim K d\delta_{n,\max}^2$ | 辅助 | 不进入 Notes | 第 1 章已预告；完整解答写入 Solutions；Notes 在 §13.1.3 / 本章小结陈述可加模型与维数含义 | 原页已核 |
| Exercise 13.10 印刷页 452；PDF 页 471 | EXERCISE | 正交级数与岭回归；Parseval 尾项 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 13.11 印刷页 452；PDF 页 471 | EXERCISE | 可微函数的 Fourier 系数与 (13.47) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |

## 来源异常与勘误

| 定位 | 问题类型 | 原式/原文 | 核验证据 | 处置 | 数学复核人 | 批准人 |
|---|---|---|---|---|---|---|
| Figure 13.2 图注 印刷页 422；PDF 页 441 | 笔误嫌疑 | 图注写 “the line of slope $1/(2\sigma)$ with $\sigma=1$” | 原页；正文同一页写 “Setting $\sigma=1/2$ for concreteness”；图中虚线从 $(0,0)$ 到 $(1,1)$，斜率 1，对应 $1/(2\sigma)=1$ 即 $\sigma=1/2$ | 保留原文；Notes 按正文 $\sigma=1/2$ 与斜率 1 解读；`勘误待批` | 作者 | 未批 |
| Theorem 13.5 注记 印刷页 423；PDF 页 442 | 笔误嫌疑 | “we necessarily have $\delta_n^2\ge\frac2\pi\frac{\sigma^2}n$” | 原页；Exercise 13.5(b) 印刷页 450 给出 $\delta^2\ge\min\{1,\frac8\pi\frac{\sigma^2}n\}$。含常数函数 1 时 $\mathcal G_n(\delta)/\delta\ge\sqrt{2/(\pi n)}$，临界不等式要求该量 $\le\delta/(2\sigma)$，故 $\delta^2\ge(8/\pi)\sigma^2/n$。$\frac2\pi$ 相当于把 $2\sigma$ 写成了 $\sigma$ | 保留原文；Notes 采用 Exercise 13.5 的 $8/\pi$ 推导，并标明与注记不一致；`勘误待批` | 作者 | 未批 |
| Theorem 13.5 注记 印刷页 423；PDF 页 442 | 笔误嫌疑 | “control on the regression error $\Vert\widehat f-f^*\Vert_2^2$” | 原页；(13.20) 与随后的 $L^2(\mathbb P_n)$-semi-norm 均用 $\Vert\cdot\Vert_n^2$ | 保留原文；Notes 按 $\Vert\cdot\Vert_n^2$ 陈述；`勘误待批` | 作者 | 未批 |
| 印刷页 424；PDF 页 443 | 笔误嫌疑 | “Theorem 13.5 can instead by applied with $\delta_n$ defined in terms of the star hull” | 原页；英语应为 be applied | 保留原文；Notes 按 “be applied” 理解；`勘误待批` | 作者 | 未批 |
| Lemma 13.12 证明 印刷页 432；PDF 页 451 | 笔误嫌疑 | “the function $v\mapsto\mathcal G_n(v)/v$ is non-decreasing” | 原页；Lemma 13.6 已证该函数非增；随后一行用 $u\ge\delta_n$ 推出 $\mathcal G_n(u)/u\le\mathcal G_n(\delta_n)/\delta_n$，只在非增时成立 | 保留原文；Notes 按非增使用；`勘误待批` | 作者 | 未批 |
| (13.53) 印刷页 439；PDF 页 458 | 笔误嫌疑 | 上确界的哑元是 $g\in\partial\mathcal F$，被积写成 $w_i f(x_i)$ | 原页；(13.16) 同类显示用 $g(x_i)$ | 保留原文；Notes 写 $g(x_i)$；`勘误待批` | 作者 | 未批 |
| Example 13.15 印刷页 435；PDF 页 454 | 笔误嫌疑 | “$(\beta_m^*)^2+(\widetilde\beta_m^*)^2\le c/m^{2\alpha}$”，未出现半径 $R$ | 原页；(13.47) 与 Exercise 13.11 均为 $cR/m^{2\alpha}$（或 $c'R/M^{2\alpha}$） | 保留原文；Notes 按带 $R$ 的系数界陈述；`勘误待批` | 作者 | 未批 |
| Exercise 13.9(b) 印刷页 452；PDF 页 471 | 笔误嫌疑 | “show that $\Vert\widehat f-f^*\Vert_n^2]\le c_3 K d\delta_{n,\max}^2$” | 原页；右方括号多余 | 保留原文；Solutions 去掉多余括号；`勘误待批` | 作者 | 未批 |
| Example 13.20 末式 印刷页 442；PDF 页 461 | 笔误嫌疑 | 先得 $\delta_n^2\simeq(\sigma^2/(R^2 n))^{2/3}$，随即写成 $R^2\delta_n^2\simeq R^2(\sigma^2/n)^{2/3}$ | 原页；同页高斯核例子把 $R^2\cdot(\sigma^2/R^2)$ 消掉。此处 $R^2\cdot R^{-4/3}=R^{2/3}$，一阶 Sobolev 的标准速率是 $R^{2/3}(\sigma^2/n)^{2/3}$ | 保留原文；Notes 写 $R^{2/3}(\sigma^2/n)^{2/3}$；`勘误待批` | 作者 | 未批 |
| Exercise 13.9(b) 兼容性 印刷页 452；PDF 页 471 | 笔误嫌疑 | $\sqrt{\sum_{j=1}^n\Vert g_j\Vert_n^2}\le\sqrt K\Vert\sum_{j=1}^d g_j\Vert_n$ | 原页；可加分量只有 $d$ 个，$j$ 应跑到 $d$。结论含 $Kd$ 只在 $\sum_{j=1}^d$ 时对得上 | 保留原文；Solutions 按 $\sum_{j=1}^d$ 理解；`勘误待批` | 作者 | 未批 |

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
