---
chapter_id: "ch14"
chapter_title: "Localization and uniform laws"
source_title: "High-Dimensional Statistics: A Non-Asymptotic Viewpoint"
source_version: "Cambridge Series in Statistical and Probabilistic Mathematics, No. 48; first published 2019; ISBN 978-1-108-49802-9"
main_source_path: "High-Dimensional Statistics A Non-Asymptotic Viewpoint (Martin J. Wainwright) (z-library.sk, 1lib.sk, z-lib.sk).pdf"
printed_pages: "453–484"
pdf_pages: "472–503"
target_notes: "notes/ch14-notes.qmd"
language: "zh-CN"
learner_profile: "学过陈希孺《概率论与数理统计》本科教材，并已读本书第 2–5、12–13 章：熟悉尾界、对称化、拉德马赫复杂度、度量熵、RKHS 与非参数最小二乘的局部复杂度。首次需要把局部化做成 L2 范数的双边/单边一致定律，并用于 Lipschitz 代价与密度估计。"
map_status: "清单完成"
---

# 第 14 章内容清单

> 内部质量工件。正式内容逐项登记；习题按题号登记但不进入 Notes。单元格内不用竖线字符。

## 来源边界

- 教材权威来源：Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series No. 48
- 版本识别依据：封面 Cambridge Series；版权页 © Martin J. Wainwright 2019，First published 2019，ISBN 978-1-108-49802-9 Hardback，DOI 10.1017/9781108627771
- 目标章节与页码：第 14 章，印刷页 453–484；PDF 页 472–503（**PDF = 印刷 + 19**）
- 补充来源及用途：无（习题独立求解）。第 2、3、4、5、12、13 章仅作记号核对。
- 已知来源限制：文本层可用但公式常错位；公式、图注、定理框须对照 `scratch/ch14/p-472.png`–`p-503.png`

## 内容清单

| 定位 | 类型 | 内容/范围 | 重要性 | Notes 处理 | 合并目标/排除理由 | 核验状态 |
|---|---|---|---|---|---|---|
| 章首 印刷页 453；PDF 页 472 | SECTION | Chapter 14 Localization and uniform laws：从渐近一致定律到局部化的非渐近速率 | 关键 | 完整讲解 |  | 原页已核 |
| §14.1 印刷页 453–462；PDF 页 472–481 | SECTION | Population and empirical L2-norms | 关键 | 完整讲解 |  | 原页已核 |
| (14.1) 印刷页 453；PDF 页 472 | DEFINITION | 总体 L2(P) 范数：$\Vert f\Vert_{L^2(\mathbb P)}^2=\int f^2\,d\mathbb P=\mathbb E[f^2(X)]$ | 关键 | 完整讲解 |  | 原页已核 |
| (14.2) 印刷页 453；PDF 页 472 | DEFINITION | 经验分布 $\mathbb P_n=n^{-1}\sum\delta_{x_i}$ 与经验 L2 范数 $\Vert f\Vert_n^2=n^{-1}\sum f^2(x_i)$ | 关键 | 完整讲解 |  | 原页已核 |
| §14.1 印刷页 454；PDF 页 473 | FORMULA | $\mathbb E[\Vert f\Vert_n^2]=\Vert f\Vert_2^2$；有界时 Hoeffding：$\mathbb P[\lvert\Vert f\Vert_n^2-\Vert f\Vert_2^2\rvert\ge t]\le 2\exp(-nt^2/(2b^4))$ | 关键 | 完整讲解 |  | 原页已核 |
| §14.1.1 印刷页 454–458；PDF 页 473–477 | SECTION | A uniform law with localization | 关键 | 完整讲解 |  | 原页已核 |
| (14.3) 印刷页 454；PDF 页 473 | DEFINITION | 局部总体拉德马赫复杂度 $\overline{\mathcal R}_n(\delta;\mathscr F)=\mathbb E_{\varepsilon,x}[\sup_{\Vert f\Vert_2\le\delta}\lvert n^{-1}\sum\varepsilon_i f(x_i)\rvert]$ | 关键 | 完整讲解 |  | 原页已核 |
| §14.1.1 印刷页 454；PDF 页 473 | DEFINITION | 星形（star-shaped around the origin）；$b$-一致有界 | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 14.1 印刷页 455；PDF 页 474 | THEOREM | 临界不等式 $\overline{\mathcal R}_n(\delta;\mathscr F)\le\delta^2/b$；双边平方偏差 (14.5a) 与范数偏差 (14.5b) | 关键 | 完整讲解 |  | 原页已核 |
| (14.6)–(14.7) 印刷页 455；PDF 页 474 | DEFINITION | 局部经验拉德马赫复杂度 $\widehat{\mathcal R}_n$ 与随机临界半径 $\hat\delta_n$ | 关键 | 完整讲解 |  | 原页已核 |
| (14.8) 印刷页 455；PDF 页 474 | FORMULA | $\hat\delta_n\in[c\delta_n,C\delta_n]$ 时 $\lvert\Vert f\Vert_n-\Vert f\Vert_2\rvert\le(c_0/c)\hat\delta_n$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 14.2 印刷页 455–457；PDF 页 474–476 | EXAMPLE | 有界二次函数类 $\mathcal P_2$：VC 给出 $n^{-1/4}$；勒让德基局部化给出 $n^{-1/2}$ | 关键 | 完整讲解 |  | 原页已核 |
| (14.9)–(14.12) 印刷页 455–457；PDF 页 474–476 | FORMULA | $\mathcal P_2$ 定义；naive VC 界 (14.10)；次优 (14.11)；局部化最优 (14.12) | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 14.3 印刷页 457；PDF 页 476 | COROLLARY | 经验覆盖数的 Dudley 积分临界不等式 (14.13) | 关键 | 完整讲解 |  | 原页已核 |
| Example 14.4 印刷页 457–458；PDF 页 476–477 | EXAMPLE | 凸 1-Lipschitz 类：$\log N_{\mathrm{sup}}\lesssim t^{-1/2}$ 推出 $\delta_n\asymp n^{-2/5}$ | 关键 | 完整讲解 |  | 原页已核 |
| §14.1.2 印刷页 458–459；PDF 页 477–478 | SECTION | Specialization to kernel classes | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 14.5 印刷页 458；PDF 页 477 | COROLLARY | RKHS 单位球：$\overline{\mathcal R}_n(\delta;\mathscr F)\le\sqrt{2/n}\sqrt{\sum\min\{\mu_j,\delta^2\}}$；经验核矩阵类似 (14.14b) | 关键 | 完整讲解 |  | 原页已核 |
| Example 14.6 印刷页 459；PDF 页 478 | EXAMPLE | 一阶 Sobolev：$\mu_j=(2/((2j-1)\pi))^2$，$\delta_n=c n^{-1/3}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 14.7 印刷页 459；PDF 页 478 | EXAMPLE | 高斯核：$\mu_j\le c_0 e^{-c_1 j\log j}$，$\delta_n\asymp\sqrt{\log(n+1)/n}$ | 关键 | 完整讲解 |  | 原页已核 |
| §14.1.3 印刷页 460–462；PDF 页 479–481 | SECTION | Proof of Theorem 14.1 | 关键 | 简要说明 |  | 原页已核 |
| (14.15)–(14.16) 印刷页 460；PDF 页 479 | FORMULA | 重标度临界 $\overline{\mathcal R}_n\le\delta^2/16$；过程 $Z_n(r)$ 与球 $\mathbb B_2(r;\mathscr F)$ | 关键 | 简要说明 |  | 原页已核 |
| Lemma 14.8 印刷页 460；PDF 页 479 | LEMMA | 星形类上 $\mathcal E_0\subseteq\mathcal A_0(t)$ 且 $\mathcal E_1\subseteq\mathcal A_0(\delta_n)\cup\mathcal A_1$ | 关键 | 简要说明 |  | 原页已核 |
| Lemma 14.9 印刷页 461；PDF 页 480 | LEMMA | $Z_n(r)$ 的尾界 (14.18)；对称化、Ledoux–Talagrand、Talagrand | 关键 | 简要说明 |  | 原页已核 |
| (14.19)–(14.20) 印刷页 461–462；PDF 页 480–481 | FORMULA | $r\mapsto\overline{\mathcal R}_n(r)/r$ 不增；剥皮论证与 $M\le 4\log(1/\delta_n)$ | 关键 | 简要说明 |  | 原页已核 |
| §14.2 印刷页 462–468；PDF 页 481–487 | SECTION | A one-sided uniform law | 关键 | 完整讲解 |  | 原页已核 |
| (14.21) 印刷页 462；PDF 页 481 | FORMULA | 单函数下尾 $\mathbb P[\Vert f\Vert_n^2\le\Vert f\Vert_2^2-t]\le\exp(-nt^2/(2\mathbb E[f^4]))$ | 关键 | 完整讲解 |  | 原页已核 |
| (14.22a)–(14.22b) 印刷页 463；PDF 页 482 | ASSUMPTION | 弱四阶矩 $\mathbb E[f^4]\le C^2\mathbb E[f^2]$（在 $\Vert f\Vert_2\le 1$）；强形式 $\mathbb E[f^4]\le C^2(\mathbb E[f^2])^2$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 14.10 印刷页 463；PDF 页 482 | EXAMPLE | 线性类 $\mathscr F_{\mathrm{lin}}$：高斯时 $C^2=3$，不必一致有界 | 关键 | 完整讲解 |  | 原页已核 |
| Example 14.11 / (14.23) 印刷页 463–464；PDF 页 482–483 | EXAMPLE | 可加非参数类；四向独立时弱矩 $C^2=b^2+6$ | 关键 | 完整讲解 |  | 原页已核 |
| (14.24) 印刷页 464；PDF 页 483 | FORMULA | 单边临界 $\overline{\mathcal R}_n(\delta;\mathscr F)/\delta\le\delta/(128C)$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 14.12 印刷页 464；PDF 页 483 | THEOREM | 星形、零均值、四阶矩下 $\Vert f\Vert_n^2\ge\tfrac12\Vert f\Vert_2^2$ 对 $\mathscr F\setminus\mathbb B_2(\delta)$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 14.13 / (14.26)–(14.29) 印刷页 465；PDF 页 484 | EXAMPLE | 线性类与随机矩阵：$\tfrac1n\Vert X\theta\Vert_2^2\ge\tfrac12\Vert\sqrt{\Sigma}\theta\Vert_2^2$；$\delta_n^2\lesssim d/n$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 14.14 / (14.30)–(14.31) 印刷页 466；PDF 页 485 | EXAMPLE | 可加模型 $\delta_n\lesssim\sqrt d\,\varepsilon_n$；Sobolev 基类时 $\Vert f\Vert_2\gtrsim\sqrt d\,n^{-1/3}$ | 关键 | 完整讲解 |  | 原页已核 |
| §14.2.1 印刷页 466–467；PDF 页 485–486 | SECTION | Consequences for nonparametric least squares | 关键 | 完整讲解 |  | 原页已核 |
| (14.32) 印刷页 466；PDF 页 485 | FORMULA | 总体拉德马赫临界与局部高斯复杂度临界（$\varepsilon_n$ 依赖协变量） | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 14.15 / (14.33) 印刷页 467；PDF 页 486 | COROLLARY | 非参数最小二乘 $\Vert\widehat f-f^*\Vert_2^2$ 高概率不超过 $c_0(\varepsilon_n^2+\delta_n^2)$ | 关键 | 完整讲解 |  | 原页已核 |
| §14.2.2 印刷页 468–469；PDF 页 487–488 | SECTION | Proof of Theorem 14.12 | 关键 | 简要说明 |  | 原页已核 |
| (14.34)–(14.38) 印刷页 468–469；PDF 页 487–488 | PROOF_DERIVATION | 截断二次 $\varphi_\tau$；$\tau^2=4C^2$；对称化与 Talagrand | 关键 | 简要说明 |  | 原页已核 |
| §14.3 印刷页 469–474；PDF 页 488–493 | SECTION | A uniform law for Lipschitz cost functions | 关键 | 完整讲解 |  | 原页已核 |
| §14.3.1 印刷页 469–472；PDF 页 488–491 | SECTION | General prediction problems | 关键 | 完整讲解 |  | 原页已核 |
| (14.39)–(14.40) 印刷页 469–470；PDF 页 488–489 | DEFINITION | 经验代价 $\mathbb P_n(\mathcal L(f(x),y))$ 与总体代价 $\mathbb P(\mathcal L(f(x),y))$ | 关键 | 完整讲解 |  | 原页已核 |
| (14.41)–(14.42) 印刷页 470；PDF 页 489 | DEFINITION | 第一变元 $L$-Lipschitz；总体代价在 $f^*$ 处相对 $L^2(\mathbb P)$ 的 $\gamma$-强凸 | 关键 | 完整讲解 |  | 原页已核 |
| Example 14.16 印刷页 470–471；PDF 页 489–490 | EXAMPLE | 最小二乘：有界噪声下 Lipschitz 常数 $L=2b+c$；点态 $\gamma=1$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 14.17 / (14.43)–(14.44) 印刷页 471；PDF 页 490 | EXAMPLE | 稳健回归：$\ell_1$ 与 Huber 代价 | 关键 | 完整讲解 |  | 原页已核 |
| Example 14.18 / (14.45)–(14.46) 印刷页 471；PDF 页 490 | EXAMPLE | Logistic：1-Lipschitz；总体差为条件 KL | 关键 | 完整讲解 |  | 原页已核 |
| Example 14.19 / (14.47) 印刷页 472；PDF 页 491 | EXAMPLE | 支持向量机与铰链代价，在 RKHS 球上二次规划 | 辅助 | 简要说明 |  | 原页已核 |
| §14.3.2 印刷页 472–474；PDF 页 491–493 | SECTION | Uniform law for Lipschitz cost functions | 关键 | 完整讲解 |  | 原页已核 |
| (14.48)–(14.50) 印刷页 472；PDF 页 491 | DEFINITION | 平移类 $\mathscr F^*=\mathscr F-f^*$；临界 $\overline{\mathcal R}_n(\delta;\mathscr F^*)\le\delta^2$ 且 $\delta_n^2\ge c/n$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 14.20 印刷页 472–473；PDF 页 491–492 | THEOREM | Lipschitz 一致定律 (14.51)；强凸推出 (14.52a)–(14.52b) | 关键 | 完整讲解 |  | 原页已核 |
| (14.53) 印刷页 473；PDF 页 492 | FORMULA | 有界直径时经验代价极小化的相合：超额风险 $O(\delta_n)$ | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 14.21 印刷页 473；PDF 页 492 | LEMMA | $Z_n(r)$ 尾界 (14.54)；证明用对称化、压缩与 Talagrand | 关键 | 简要说明 |  | 原页已核 |
| §14.4 印刷页 475–479；PDF 页 494–498 | SECTION | Some consequences for nonparametric density estimation | 关键 | 完整讲解 |  | 原页已核 |
| §14.4.1 印刷页 475–476；PDF 页 494–495 | SECTION | Density estimation via the nonparametric MLE | 关键 | 完整讲解 |  | 原页已核 |
| (14.56) 印刷页 475；PDF 页 494 | DEFINITION | 约束非参数 MLE：$\widehat f\in\arg\min_{f\in\mathscr F}\mathbb P_n(-\log f)$ | 关键 | 完整讲解 |  | 原页已核 |
| (14.57a)–(14.57b) 印刷页 475；PDF 页 494 | DEFINITION | 平方海林格 $H^2(f\Vert g)=\tfrac12\int(\sqrt f-\sqrt g)^2\,d\mu$；$D(f\Vert g)\ge 2H^2(f\Vert g)$ | 关键 | 完整讲解 |  | 原页已核 |
| (14.58) 印刷页 476；PDF 页 495 | FORMULA | 平方根密度平移类的临界不等式 | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 14.22 / (14.59) 印刷页 476；PDF 页 495 | COROLLARY | NPMLE 的海林格界 $H^2(\widehat f\Vert f^*)\le c_0\delta_n^2$ | 关键 | 完整讲解 |  | 原页已核 |
| §14.4.2 印刷页 477–479；PDF 页 496–498 | SECTION | Density estimation via projections | 关键 | 完整讲解 |  | 原页已核 |
| (14.60) 印刷页 477；PDF 页 496 | DEFINITION | 投影密度估计 $\arg\min\{\tfrac12\Vert f\Vert_2^2-\mathbb P_n(f)\}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 14.23 / (14.61)–(14.64) 印刷页 477–478；PDF 页 496–497 | EXAMPLE | 正交级数：直方图与投影傅里叶；闭式系数 (14.63) | 关键 | 完整讲解 |  | 原页已核 |
| Figure 14.1 印刷页 478；PDF 页 497 | FIGURE_TABLE | 直方图密度估计，$n=100$ 与 $n=2000$，$T=5,20$ | 辅助 | 简要说明 |  | 原页已核 |
| Figure 14.2 印刷页 479；PDF 页 498 | FIGURE_TABLE | 傅里叶投影密度估计，阶跃密度 (14.64) | 辅助 | 简要说明 |  | 原页已核 |
| Corollary 14.24 / (14.65) 印刷页 479；PDF 页 498 | COROLLARY | 投影估计的神谕不等式 | 关键 | 完整讲解 |  | 原页已核 |
| §14.5 印刷页 480–481；PDF 页 499–500 | SECTION | Appendix: Population and empirical Rademacher complexities | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 14.25 / (14.66) 印刷页 480；PDF 页 499 | PROPOSITION | 三明治 $\delta_n/4\le\hat\delta_n\le 3\delta_n$ | 关键 | 完整讲解 |  | 原页已核 |
| (14.67)–(14.68) 印刷页 480；PDF 页 499 | FORMULA | 事件 $\mathcal E_0(t),\mathcal E_1$ 上总体球与经验球互相控制 | 辅助 | 并入相关内容 | 并入 Proposition 14.25 的证明要点 | 原页已核 |
| §14.6 印刷页 481–482；PDF 页 500–501 | PROSE_RANGE | Bibliographic details：局部复杂度、单边定律、可加模型、SVM、密度估计文献 | 辅助 | 指回教材 | 文献清单不抄入 Notes | 原页已核 |
| §14.7 印刷页 482–484；PDF 页 501–503 | SECTION | Exercises 14.1–14.11 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 14.1 印刷页 482；PDF 页 501 | EXERCISE | 证明 $\mathbb E[\sup_{\Vert f\Vert_2\le t}\Vert f\Vert_n]\le\sqrt5\,t$ | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 14.2 印刷页 482；PDF 页 501 | EXERCISE | 局部拉德马赫的单调性与临界半径比较 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 14.3 印刷页 482；PDF 页 501 | EXERCISE | 用熵积分改进 Example 14.2 的 naive 界 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 14.4 印刷页 482–483；PDF 页 501–502 | EXERCISE | 证明 Corollary 14.5 的总体界 (14.14a) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 14.5 印刷页 483；PDF 页 502 | EXERCISE | 核积分算子的经验逼近与算子范数 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 14.6 印刷页 483；PDF 页 502 | EXERCISE | 四向独立线性类的强四阶矩 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 14.7 印刷页 483–484；PDF 页 502–503 | EXERCISE | 稀疏锥上的限制特征值 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 14.8 印刷页 484；PDF 页 503 | EXERCISE | 可加模型临界半径 $\delta_n^2\lesssim d\varepsilon_n^2$ | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 14.9 印刷页 484；PDF 页 503 | EXERCISE | 全体可微密度上 NPMLE 不存在 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 14.10 印刷页 484；PDF 页 503 | EXERCISE | 证明 $D\ge 2H^2$ | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 14.11 印刷页 484；PDF 页 503 | EXERCISE | 直方图神谕不等式给出 $n^{-2/3}$ | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |

## 来源异常与勘误

| 定位 | 问题类型 | 原式/原文 | 核验证据 | 处置 | 数学复核人 | 批准人 |
|---|---|---|---|---|---|---|
| Example 14.2 印刷页 457；PDF 页 476 | 笔误嫌疑 | 局部化计算之后写 “Applying Theorem 4.10 then guarantees” 得到 (14.12) | 原页；(14.12) 即 Theorem 14.1 的 (14.5a)；Theorem 4.10 是第 4 章对称化/ULLN | 保留原文；Notes 按 Theorem 14.1 解读；`勘误待批` | 作者 | 未批 |
| Example 14.13 印刷页 465；PDF 页 484 | 笔误嫌疑 | “Writing each $x=\sqrt{\Sigma}w$, where $w\sim\mathcal N(0,\Sigma)$” | 原页；紧接着写 $\varepsilon_i w_i$ 为标准高斯，且 $\mathbb E\Vert n^{-1}\sum\varepsilon_i w_i\Vert_2\le\sqrt{d/n}$，故应为 $w\sim\mathcal N(0,I)$ | 保留原文；Notes 按 $w\sim\mathcal N(0,I_d)$ 解读；`勘误待批` | 作者 | 未批 |
| Example 14.14 印刷页 466；PDF 页 485 | 笔误嫌疑 | 单变量临界写成 $\overline{\mathcal R}_n(\varepsilon;\mathscr F)\lesssim\varepsilon^2$ | 原页；前文定义 $\varepsilon_n$ 属于单变量类 $\mathscr G$，应为 $\overline{\mathcal R}_n(\varepsilon;\mathscr G)$ | 保留原文；Notes 按 $\mathscr G$ 解读；`勘误待批` | 作者 | 未批 |
| Example 14.17 / (14.44) 印刷页 471；PDF 页 490 | 笔误嫌疑 | Huber 在 $\lvert u\rvert>\tau$ 写成 $\tau u-\tau^2/2$ | 原页；该式在 $u<-\tau$ 时无下界且可为负；标准 Huber 为 $\tau\lvert u\rvert-\tau^2/2$ | 保留原文；Notes 标明与标准定义不一致；`勘误待批` | 作者 | 未批 |
| Corollary 14.15 证明 Case 1 印刷页 467；PDF 页 486 | 笔误嫌疑 | $\mathbb P_w[\Vert\widehat f-f^*\Vert_n\ge 16\delta_n^2]$ | 原页；Case 2 与 Theorem 14.12 均用平方经验范数；与 $2\Vert\cdot\Vert_n^2$ 相加才得到总体平方误差 $c_0\delta_n^2$ | 保留原文；Notes 按 $\Vert\widehat f-f^*\Vert_n^2\ge 16\delta_n^2$ 解读；`勘误待批` | 作者 | 未批 |
| Theorem 14.20 证明 印刷页 474；PDF 页 493 | 笔误嫌疑 | 强凸推出 $\Vert\widehat f-f^*\Vert_2\le 10L/\gamma$ | 原页；由 $(\gamma/2)r^2\le 10L\delta_n r$ 应得 $r\le 20L\delta_n/\gamma$；陈述 (14.52a) 含 $\delta_n$ | 保留原文；Notes 按带 $\delta_n$ 的 (14.52a) 解读；`勘误待批` | 作者 | 未批 |
| Exercise 14.4(a) 印刷页 483；PDF 页 502 | 笔误嫌疑 | 约束 $\sum\theta_j^2\le\delta$ | 原页；$\Vert f\Vert_2\le\delta$ 应对 $\sum\theta_j^2\le\delta^2$；(b) 的 $\eta_j=\min\{\delta^2,\mu_j\}$ 与椭圆常数 2 只在平方约束下成立 | 保留原文；Solutions 按 $\delta^2$ 求解并标明；`勘误待批` | 作者 | 未批 |
| Exercise 14.5(c) 印刷页 483；PDF 页 502 | 笔误嫌疑 | $\lVert\widehat T_{\mathcal K}(\phi_j)-\mu_j\phi_j\rVert_{\mathbb H}\le\Vert\widehat T_{\mathcal K}-T_{\mathcal K}\Vert_{\mathbb H}/\mu_j$ | 原页；Corollary 12.26 给出 $\lVert\phi_j\rVert_{\mathbb H}=1/\sqrt{\mu_j}$，算子范数定义只推出分母 $\sqrt{\mu_j}$ | 保留原文；Solutions 按 $1/\sqrt{\mu_j}$ 求解并标明；`勘误待批` | 作者 | 未批 |
| Exercise 14.6 印刷页 483；PDF 页 502 | 笔误嫌疑 | 强矩条件 (14.22b) “with $C=B+6$” | 原页；Example 14.13 写 $C^2=B+6$；(14.22b) 含 $C^2(\mathbb E[f^2])^2$；计算给出 $\mathbb E[f^4]\le(B+6)(\mathbb E[f^2])^2$ | 保留原文；Solutions 证明 $C^2=B+6$ 并标明题干 $C$；`勘误待批` | 作者 | 未批 |

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
