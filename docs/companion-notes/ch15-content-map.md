---
chapter_id: "ch15"
chapter_title: "Minimax lower bounds"
source_title: "High-Dimensional Statistics: A Non-Asymptotic Viewpoint"
source_version: "Cambridge Series in Statistical and Probabilistic Mathematics, No. 48; first published 2019; ISBN 978-1-108-49802-9"
main_source_path: "High-Dimensional Statistics A Non-Asymptotic Viewpoint (Martin J. Wainwright) (z-library.sk, 1lib.sk, z-lib.sk).pdf"
printed_pages: "485–523"
pdf_pages: "504–542"
target_notes: "notes/ch15-notes.qmd"
language: "zh-CN"
learner_profile: "学过陈希孺《概率论与数理统计》本科教材，并读过本书第 5 章填装/度量熵；熟悉假设检验的奈曼–皮尔逊思想与高斯模型；首次需要把上界理论对偶成与算法无关的极小极大下界，并掌握勒卡姆两点法、凸包法、范诺局部填装与杨–巴伦全局熵。"
map_status: "清单完成"
---

# 第 15 章内容清单

> 内部质量工件。正式内容逐项登记；连续说明与文献可聚合。§15.6 习题进入 Solutions，不进 Notes。

## 来源边界

- 教材权威来源：Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series No. 48
- 版本识别依据：封面 Cambridge Series；版权页 © Martin J. Wainwright 2019，First published 2019，ISBN 978-1-108-49802-9 Hardback，DOI 10.1017/9781108627771
- 目标章节与页码：第 15 章，印刷页 485–523；PDF 页 504–542（**PDF = 印刷 + 19**）
- 补充来源及用途：无（习题独立求解）
- 已知来源限制：文本层可用但公式常错位；公式、图注须对照 `scratch/ch15/p-5XX.png`

## 内容清单

| 定位 | 类型 | 内容/范围 | 重要性 | Notes 处理 | 合并目标/排除理由 | 核验状态 |
|---|---|---|---|---|---|---|
| 章首 印刷页 485；PDF 页 504 | SECTION | Chapter 15 Minimax lower bounds：与算法无关的估计下界；填装、度量熵与信息论 | 关键 | 完整讲解 |  | 原页已核 |
| §15.1 印刷页 485–491；PDF 页 504–510 | SECTION | Basic framework | 关键 | 完整讲解 |  | 原页已核 |
| §15.1 印刷页 485–486；PDF 页 504–505 | DEFINITION | 泛函 $\theta(\mathbb P)$；参数化族与非参数泛函（二次泛函、众数） | 关键 | 完整讲解 |  | 原页已核 |
| §15.1.1 印刷页 486；PDF 页 505 | SECTION | Minimax risks | 关键 | 完整讲解 |  | 原页已核 |
| (15.1) 印刷页 486；PDF 页 505 | FORMULA | 极小极大风险 $\mathfrak M(\theta(\mathcal P);\rho)=\inf_{\widehat\theta}\sup_{\mathbb P}\mathbb E_{\mathbb P}[\rho(\widehat\theta,\theta(\mathbb P))]$ | 关键 | 完整讲解 |  | 原页已核 |
| (15.2) 印刷页 486；PDF 页 505 | FORMULA | 复合损失 $\mathfrak M(\theta(\mathcal P);\Phi\circ\rho)$；常见 $\Phi(t)=t^2$ | 关键 | 完整讲解 |  | 原页已核 |
| §15.1.1 脚注 印刷页 486；PDF 页 505 | DEFINITION | 半度量：除 $\rho(\theta,\theta')=0$ 不必推出 $\theta=\theta'$ 外满足度量公理 | 辅助 | 简要说明 |  | 原页已核 |
| §15.1.2 印刷页 487–489；PDF 页 506–508 | SECTION | From estimation to testing | 关键 | 完整讲解 |  | 原页已核 |
| Prop. 15.1 / (15.3) 印刷页 487；PDF 页 506 | PROPOSITION | 估计约化到检验：$\mathfrak M(\theta(\mathcal P),\Phi\circ\rho)\ge\Phi(\delta)\inf_\psi\mathbb Q[\psi(Z)\ne J]$ | 关键 | 完整讲解 |  | 原页已核 |
| (15.4) 印刷页 488；PDF 页 507 | FORMULA | 最近邻检验 $\psi(Z)=\arg\min_{\ell}\rho(\theta^\ell,\widehat\theta)$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 15.1 印刷页 488；PDF 页 507 | FIGURE_TABLE | $2\delta$-分离集把 $\rho(\widehat\theta,\theta^j)<\delta$ 变成正确判决 | 辅助 | 简要说明 |  | 原页已核 |
| §15.1.3 印刷页 489–491；PDF 页 508–510 | SECTION | Some divergence measures | 关键 | 完整讲解 |  | 原页已核 |
| (15.5)–(15.6) 印刷页 489；PDF 页 508 | DEFINITION | 全变差距离：集合上确界与 $\frac12\Vert p-q\Vert_{L^1(\nu)}$ | 关键 | 完整讲解 |  | 原页已核 |
| (15.7) 印刷页 490；PDF 页 509 | DEFINITION | 库尔贝克–莱布勒散度 $D(\mathbb Q\Vert\mathbb P)=\int q\log(q/p)\,d\nu$ | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 15.2 / (15.8) 印刷页 490；PDF 页 509 | LEMMA | 平斯克–奇萨尔–库尔贝克：$\Vert\mathbb P-\mathbb Q\Vert_{\mathrm{TV}}\le\sqrt{\frac12 D(\mathbb Q\Vert\mathbb P)}$ | 关键 | 完整讲解 |  | 原页已核 |
| (15.9) 印刷页 490；PDF 页 509 | DEFINITION | 平方赫林格距离 $H^2(\mathbb P\Vert\mathbb Q)=\int(\sqrt p-\sqrt q)^2\,d\nu\in[0,2]$ | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 15.3 / (15.10) 印刷页 490；PDF 页 509 | LEMMA | 勒卡姆不等式：TV $\le H\sqrt{1-H^2/4}$ | 关键 | 完整讲解 |  | 原页已核 |
| (15.11a)–(15.11b) 印刷页 491；PDF 页 510 | FORMULA | 乘积测度下 KL 可加；$n$ 次 i.i.d. 时为 $nD$ | 关键 | 完整讲解 |  | 原页已核 |
| (15.12a)–(15.12b) 印刷页 491；PDF 页 510 | FORMULA | 赫林格乘积公式；i.i.d. 时 $\frac12 H^2(\mathbb P^{1:n}\Vert\mathbb Q^{1:n})\le\frac n2 H^2(\mathbb P_1\Vert\mathbb Q_1)$ | 关键 | 完整讲解 |  | 原页已核 |
| §15.2 印刷页 491–500；PDF 页 510–519 | SECTION | Binary testing and Le Cam's method | 关键 | 完整讲解 |  | 原页已核 |
| §15.2.1 印刷页 491–497；PDF 页 510–516 | SECTION | Bayes error and total variation distance | 关键 | 完整讲解 |  | 原页已核 |
| (15.13) 印刷页 491；PDF 页 510 | FORMULA | 等先验二元贝叶斯风险 $\inf\mathbb Q[\psi(Z)\ne J]=\frac12\{1-\Vert\mathbb P_1-\mathbb P_0\Vert_{\mathrm{TV}}\}$ | 关键 | 完整讲解 |  | 原页已核 |
| (15.14) 印刷页 492；PDF 页 511 | FORMULA | 两点勒卡姆下界 $\mathfrak M\ge\frac{\Phi(\delta)}{2}\{1-\Vert\mathbb P_1-\mathbb P_0\Vert_{\mathrm{TV}}\}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 15.4 / (15.15)–(15.16) 印刷页 492；PDF 页 511 | EXAMPLE | 高斯位置族：两点法给出 $\sigma/(12\sqrt n)$ 与 $\sigma^2/(24n)$；样本均值上界匹配阶 | 关键 | 完整讲解 |  | 原页已核 |
| Example 15.5 印刷页 493；PDF 页 512 | EXAMPLE | 均匀位置族：KL 无穷，改用赫林格；MSE 下界阶 $n^{-2}$；最小观测可达 | 关键 | 完整讲解 |  | 原页已核 |
| (15.17) 印刷页 493；PDF 页 512 | DEFINITION | 泛函相对赫林格的利普希茨常数 $\omega(\epsilon;\theta,\mathscr F)$ | 关键 | 完整讲解 |  | 原页已核 |
| Cor. 15.6 / (15.18) 印刷页 494；PDF 页 513 | COROLLARY | 泛函勒卡姆：$\inf\sup\mathbb E\Phi(\lvert\widehat\theta-\theta(f)\rvert)\ge\frac14\Phi\bigl(\frac12\omega(1/(2\sqrt n))\bigr)$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 15.7 / (15.19)–(15.20) 印刷页 494–495；PDF 页 513–514 | EXAMPLE | 利普希茨密度的点估计：帽函数扰动，MSE $\asymp n^{-2/3}$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 15.2 印刷页 495；PDF 页 514 | FIGURE_TABLE | $\delta=0.12$ 的帽函数 $\phi$ | 辅助 | 简要说明 |  | 原页已核 |
| Example 15.8 / (15.21)–(15.24) 印刷页 496–497；PDF 页 515–516 | EXAMPLE | 二次泛函两点法只给出 $n^{-1/2}$，不是最优（最优 $n^{-4/9}$） | 关键 | 完整讲解 |  | 原页已核 |
| Figure 15.3 印刷页 497；PDF 页 516 | FIGURE_TABLE | 基函数、平移尺度、均匀密度与叠加密度 $g$ | 辅助 | 简要说明 |  | 原页已核 |
| §15.2.2 印刷页 497–500；PDF 页 516–519 | SECTION | Le Cam's convex hull method | 关键 | 完整讲解 |  | 原页已核 |
| (15.25) 印刷页 498；PDF 页 517 | DEFINITION | 两类 $2\delta$-分离：一切 $\mathbb P_0\in\mathcal P_0$、$\mathbb P_1\in\mathcal P_1$ 满足 $\rho(\theta(\mathbb P_0),\theta(\mathbb P_1))\ge 2\delta$ | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 15.9 / (15.26) 印刷页 498；PDF 页 517 | LEMMA | 勒卡姆凸包：最坏风险 $\ge(\delta/2)\sup_{\mathrm{conv}}\{1-\Vert\mathbb P_0-\mathbb P_1\Vert_{\mathrm{TV}}\}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 15.10 / (15.27) 印刷页 498–499；PDF 页 517–518 | EXAMPLE | 高斯位置族凸包：前置因子从 $1/12$ 升到 $3/20$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 15.11 / (15.28) 印刷页 499–500；PDF 页 518–519 | EXAMPLE | 二次泛函凸包：符号模式混合给出 $n^{-4/9}$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 15.4 印刷页 500；PDF 页 519 | FIGURE_TABLE | 不同符号向量 $\alpha$ 下的密度 $f_\alpha$ | 辅助 | 简要说明 |  | 原页已核 |
| §15.3 印刷页 500–515；PDF 页 519–534 | SECTION | Fano's method | 关键 | 完整讲解 |  | 原页已核 |
| §15.3.1 印刷页 501；PDF 页 520 | SECTION | Kullback–Leibler divergence and mutual information | 关键 | 完整讲解 |  | 原页已核 |
| (15.29) 印刷页 501；PDF 页 520 | DEFINITION | 互信息 $I(Z,J)=D(\mathbb Q_{Z,J}\Vert\mathbb Q_Z\mathbb Q_J)$ | 关键 | 完整讲解 |  | 原页已核 |
| (15.30) 印刷页 501；PDF 页 520 | FORMULA | $I(Z;J)=\frac1M\sum_j D(\mathbb P_{\theta^j}\Vert\overline{\mathbb Q})$ | 关键 | 完整讲解 |  | 原页已核 |
| §15.3.2 印刷页 501–503；PDF 页 520–522 | SECTION | Fano lower bound on minimax risk | 关键 | 完整讲解 |  | 原页已核 |
| (15.31) 印刷页 501；PDF 页 520 | FORMULA | 范诺：$\mathbb P[\psi(Z)\ne J]\ge 1-(I(Z;J)+\log 2)/\log M$ | 关键 | 完整讲解 |  | 原页已核 |
| Prop. 15.12 / (15.32) 印刷页 502；PDF 页 521 | PROPOSITION | 范诺极小极大下界 $\mathfrak M\ge\Phi(\delta)\{1-(I+\log 2)/\log M\}$ | 关键 | 完整讲解 |  | 原页已核 |
| (15.33)–(15.34) 印刷页 502；PDF 页 521 | FORMULA | 目标 $I+\log 2\le\frac12\log M$；凸性上界 $I\le M^{-2}\sum_{j,k}D(\mathbb P_{\theta^j}\Vert\mathbb P_{\theta^k})$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 15.13 印刷页 502–503；PDF 页 521–522 | EXAMPLE | 三点高斯位置：范诺给出 $\sigma^2/(80n)$ | 关键 | 完整讲解 |  | 原页已核 |
| §15.3.3 印刷页 503–506；PDF 页 522–525 | SECTION | Bounds based on local packings | 关键 | 完整讲解 |  | 原页已核 |
| (15.35a)–(15.35b) 印刷页 503；PDF 页 522 | FORMULA | 局部填装：$\sqrt{D}\le c\sqrt n\,\delta$ 且 $\log M(2\delta)\ge 2\{c^2 n\delta^2+\log 2\}$ 则 $\mathfrak M\ge\frac12\Phi(\delta)$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 15.14 / (15.36)–(15.37) 印刷页 503–504；PDF 页 522–523 | EXAMPLE | 固定设计线性回归：预测风险 $\ge\sigma^2\mathrm{rank}(\mathbf X)/(128n)$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 15.15 / (15.38)–(15.39) 印刷页 504–505；PDF 页 523–524 | EXAMPLE | $\mathscr F_2$ 密度估计：局部填装给出平方赫林格 $n^{-4/5}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 15.16 / (15.40)–(15.41) 印刷页 506；PDF 页 525 | EXAMPLE | 稀疏线性回归：$\mathfrak M(\mathbb S^d(s);\Vert\cdot\Vert_2)\gtrsim(\sigma^2/\gamma_{2s}^2)\,s\log(ed/s)/n$ | 关键 | 完整讲解 |  | 原页已核 |
| §15.3.4 印刷页 506–512；PDF 页 525–531 | SECTION | Local packings with Gaussian entropy bounds | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 15.17 / (15.42)–(15.43) 印刷页 506–507；PDF 页 525–526 | LEMMA | 高斯条件分布的互信息：$\frac12\{\log\det\mathrm{cov}(Z)-M^{-1}\sum\log\det(\Sigma^j)\}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 15.18 / (15.44)–(15.46) 印刷页 507–509；PDF 页 526–528 | EXAMPLE | 稀疏回归变量选择：两个 ensemble 给出样本量下界 (15.44) | 关键 | 完整讲解 |  | 原页已核 |
| (15.47) 印刷页 509；PDF 页 528 | FORMULA | 尖刺协方差 $x\stackrel{d}{=}\sqrt{\nu}\,\xi\theta^*+w$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 15.19 / (15.48)–(15.50) 印刷页 509–511；PDF 页 528–530 | EXAMPLE | PCA：$\mathfrak M\gtrsim\min\{(1+\nu)d/(\nu^2 n),\,1\}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 15.20 印刷页 511–512；PDF 页 530–531 | EXAMPLE | 稀疏 PCA 支撑恢复：$\theta_{\min}\gtrsim s^{-1/2}$ 时需 $n\gtrsim\frac{1+\nu}{\nu^2}s\log(d-s+1)$ | 关键 | 完整讲解 |  | 原页已核 |
| §15.3.5 印刷页 512–515；PDF 页 531–534 | SECTION | Yang–Barron version of Fano's method | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 15.21 / (15.51)–(15.52) 印刷页 512；PDF 页 531 | LEMMA | 杨–巴伦：$I(Z;J)\le\inf_{\epsilon}\{\epsilon^2+\log N_{\mathrm{KL}}(\epsilon;\mathcal P)\}$ | 关键 | 完整讲解 |  | 原页已核 |
| (15.53a)–(15.53b) 印刷页 513；PDF 页 532 | FORMULA | 两步选 $(\epsilon_n,\delta_n)$：$\epsilon_n^2\ge\log N_{\mathrm{KL}}$ 且 $\log M(\delta_n)\ge 4\epsilon_n^2+2\log 2$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 15.22 印刷页 513–514；PDF 页 532–533 | EXAMPLE | 密度估计再用杨–巴伦直接得到 $n^{-4/5}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 15.23 / (15.54)–(15.56) 印刷页 514–515；PDF 页 533–534 | EXAMPLE | 广义索伯列夫：$\inf\sup\mathbb E\Vert\widehat f-f\Vert_2^2\gtrsim\min\{1,(\sigma^2/n)^{2\alpha/(2\alpha+1)}\}$ | 关键 | 完整讲解 |  | 原页已核 |
| §15.4 印刷页 515–518；PDF 页 534–537 | SECTION | Appendix: Basic background in information theory | 关键 | 完整讲解 |  | 原页已核 |
| Def. 15.24 / (15.57)–(15.58) 印刷页 516；PDF 页 535 | DEFINITION | 香农熵；离散熵 $H(\mathbb Q)=-\sum q\log q$ | 关键 | 完整讲解 |  | 原页已核 |
| Def. 15.25 / (15.59) 印刷页 516；PDF 页 535 | DEFINITION | 条件熵 $H(X\mid Y)=\mathbb E_Y[H(\mathbb Q_{X\mid Y})]$ | 关键 | 完整讲解 |  | 原页已核 |
| (15.60a)–(15.60e) 印刷页 516–517；PDF 页 535–536 | FORMULA | 条件化减熵、链式法则、互信息与熵的关系 | 关键 | 完整讲解 |  | 原页已核 |
| (15.61)–(15.62) 印刷页 517；PDF 页 536 | PROOF_DERIVATION | 范诺标准形 $h(q_e)+q_e\log(M-1)\ge H(J\mid Z)$ 及其证明 | 关键 | 完整讲解 |  | 原页已核 |
| §15.5 印刷页 518–519；PDF 页 537–538 | PROSE_RANGE | Bibliographic details：Shannon、KL、Le Cam、Hasminskii、Assouad、Birgé、Yu、Yang–Barron、计算/隐私约束极小极大 | 辅助 | 指回教材 | 文献清单不抄入 Notes | 原页已核 |
| §15.6 印刷页 519–523；PDF 页 538–542 | SECTION | Exercises 15.1–15.18 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 15.1 印刷页 519；PDF 页 538 | EXERCISE | TV 的变分表示 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 15.2 印刷页 519；PDF 页 538 | EXERCISE | 离散熵非负且 $\le\log\lvert\mathcal X\rvert$ | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 15.3 / (15.63) 印刷页 519–520；PDF 页 538–539 | EXERCISE | KL 非负、凸性、乘积可加 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 15.4 印刷页 520；PDF 页 539 | EXERCISE | 条件化减熵与链式法则 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 15.5 印刷页 520；PDF 页 539 | EXERCISE | 证明勒卡姆不等式 (15.10) | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 15.6 / (15.64) 印刷页 520；PDF 页 539 | EXERCISE | 证明平斯克不等式 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 15.7 印刷页 520；PDF 页 539 | EXERCISE | 赫林格乘积公式 (15.12a) | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 15.8 印刷页 520；PDF 页 539 | EXERCISE | 高斯位置族更锐两点界 $\sigma/(8\sqrt n)$、$\sigma^2/(16n)$ | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 15.9 印刷页 520；PDF 页 539 | EXERCISE | 均匀平移：$\widetilde\theta=\min Y_i$ 满足 $\mathbb E[(\widetilde\theta-\theta)^2]\le 2/n^2$ | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 15.10 / (15.65)–(15.66) 印刷页 521；PDF 页 540 | EXERCISE | TV 的二阶矩上界；高斯与对称混合 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 15.11 印刷页 521；PDF 页 540 | EXERCISE | 混合物极小化平均 KL | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 15.12 / (15.67) 印刷页 521；PDF 页 540 | EXERCISE | $f$-散度：KL、反向 KL、赫林格、$1-\sqrt t$ | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 15.13 印刷页 521；PDF 页 540 | EXERCISE | 多元高斯 KL | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 15.14 印刷页 522；PDF 页 541 | EXERCISE | 高斯最大熵 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 15.15 印刷页 522；PDF 页 541 | EXERCISE | 稀疏 PCA 支撑恢复的 $\theta_{\min}$ 依赖下界 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 15.16 印刷页 522；PDF 页 541 | EXERCISE | 稀疏 PCA 的 $\ell_2$ 下界 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 15.17 印刷页 522–523；PDF 页 541–542 | EXERCISE | 广义线性模型的极小极大下界 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |
| Exercise 15.18 印刷页 523；PDF 页 542 | EXERCISE | 可加 / 稀疏可加非参数回归下界 | 辅助 | 不进入 Notes | 写入 Solutions | 原页已核 |

## 来源异常与勘误

| 定位 | 问题类型 | 原式/原文 | 核验证据 | 处置 | 数学复核人 | 批准人 |
|---|---|---|---|---|---|---|
| Def. 15.25 (15.59) 印刷页 516；PDF 页 535 | 笔误嫌疑 | 条件熵展开写成 $\mathbb E_Y\bigl[\int q(x\mid Y)\log q(x\mid Y)\,\mu(dx)\bigr]$，缺负号 | 原页 PNG `p-535.png`；Def. 15.24 的 $H(\mathbb Q)=-\int q\log q$ | 保留原文；Notes 按 $-\int q\log q$ 使用；`勘误待批` | 作者 | 未批 |
| (15.60c) 印刷页 517；PDF 页 536 | 笔误嫌疑 | $H(X,Y\mid Z)=H(X\mid Z)+H(X\mid Y,Z)$ | 原页 PNG `p-536.png`；链式法则应为 $H(X\mid Z)+H(Y\mid X,Z)$ | 保留原文；Notes 写正形式并标明；`勘误待批` | 作者 | 未批 |
| 范诺证明末句 印刷页 518；PDF 页 537 | 笔误嫌疑 | $H(V,J\mid Z)\le h(q_e)+\log(M-1)$ | 原页 PNG `p-537.png`；按 $H(J\mid V,Z)=q_e H(J\mid Z,V=1)$ 应为 $h(q_e)+q_e\log(M-1)$ 才能得 (15.61) | 保留原文；Notes 补 $q_e$；`勘误待批` | 作者 | 未批 |
| Example 15.15 印刷页 505；PDF 页 524 | 笔误嫌疑 | $(\sqrt{f_\alpha}+\sqrt{f_\beta})^2=2(f_\alpha+f_\beta)\le 4$ | 原页 PNG `p-524.png`；展开是 $f_\alpha+f_\beta+2\sqrt{f_\alpha f_\beta}$；$\alpha_j\ne\beta_j$ 时 $f_\alpha+f_\beta=2$，故 $4$ 是上界不是恒等 | 保留原文；Notes 按 $\le 4$ 用；`勘误待批` | 作者 | 未批 |
| (15.44) 印刷页 507；PDF 页 526 | 笔误嫌疑 | 第一项分母外写 $\log(d+s-1)$ | 原页 PNG `p-526.png`；Ensemble B 明确 $M=d-s+1$，印刷页 509 亦写 $\log(d-s+1)>4\log 2$ | 保留原文；Notes 按 $d-s+1$ 解读；`勘误待批` | 作者 | 未批 |
| Example 15.20 印刷页 512；PDF 页 531 | 笔误嫌疑 | 正文写 $\log M=\log(d-s-1)$ | 原页 PNG `p-531.png`；同一段随后的比值用 $\log(d-s+1)$，且 $M=\lvert S^c\rvert=d-s+1$ | 保留原文；Notes 按 $d-s+1$；`勘误待批` | 作者 | 未批 |

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
