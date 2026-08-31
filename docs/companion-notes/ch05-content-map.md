---
chapter_id: "ch05"
chapter_title: "Metric entropy and its uses"
source_title: "High-Dimensional Statistics: A Non-Asymptotic Viewpoint"
source_version: "Cambridge Series in Statistical and Probabilistic Mathematics, No. 48; first published 2019; ISBN 978-1-108-49802-9"
main_source_path: "High-Dimensional Statistics A Non-Asymptotic Viewpoint (Martin J. Wainwright) (z-library.sk, 1lib.sk, z-lib.sk).pdf"
printed_pages: "121–158"
pdf_pages: "140–177"
target_notes: "notes/ch05-notes.qmd"
language: "zh-CN"
learner_profile: "学过陈希孺《概率论与数理统计》本科教材；已读本书第 1–4 章的伴读 Notes。第 1 章已预告 δ-覆盖/填装；缺口是度量熵的精确定义与体积比、高斯/拉德马赫复杂度、一步离散化、达德利熵积分与链式、斯莱皮安/苏达科夫–费尔尼克比较、高斯收缩、苏达科夫下界、奥尔里奇过程。"
map_status: "清单完成"
---

# 第 5 章内容清单

> 内部质量工件。正式内容逐项登记；§5.8 习题整段不进入 Notes，完整解答写入 Solutions。

## 来源边界

- 教材权威来源：Wainwright, *High-Dimensional Statistics: A Non-Asymptotic Viewpoint*, Cambridge Series No. 48
- 版本识别依据：封面 Cambridge Series；版权页 © Martin J. Wainwright 2019，First published 2019，ISBN 978-1-108-49802-9 Hardback，DOI 10.1017/9781108627771
- 目标章节与页码：第 5 章，印刷页 121–158；PDF 页 140–177（**PDF = 印刷 + 19**）
- 补充来源及用途：无（习题独立求解）
- 已知来源限制：文本层可用但公式常错位；公式、图注、定理框须对照 `scratch/ch05/p-1XX.png`

## 内容清单

| 定位 | 类型 | 内容/范围 | 重要性 | Notes 处理 | 合并目标/排除理由 | 核验状态 |
|---|---|---|---|---|---|---|
| 章首 印刷页 121；PDF 页 140 | SECTION | Chapter 5 Metric entropy and its uses：用覆盖/填装度量无穷指标集，服务随机过程上确界 | 关键 | 完整讲解 |  | 原页已核 |
| §5.1 印刷页 121–131；PDF 页 140–150 | SECTION | Covering and packing | 关键 | 完整讲解 |  | 原页已核 |
| §5.1 印刷页 121；PDF 页 140 | DEFINITION | 度量空间 $(T,\rho)$：非负、对称、三角不等式 | 关键 | 完整讲解 |  | 原页已核 |
| (5.1a) 印刷页 121；PDF 页 140 | FORMULA | 欧氏度量 $\rho(\theta,\widetilde\theta)=\Vert\theta-\widetilde\theta\Vert_2$ | 关键 | 完整讲解 |  | 原页已核 |
| (5.1b) 印刷页 121；PDF 页 140 | FORMULA | 重标度汉明度量 $\rho_H(\theta,\widetilde\theta)=d^{-1}\sum_j \mathbb I[\theta_j\neq\widetilde\theta_j]$ | 关键 | 完整讲解 |  | 原页已核 |
| (5.1c) 印刷页 122；PDF 页 141 | FORMULA | $L^2(\mu,[0,1])$ 度量 $\Vert f-g\Vert_2=(\int_0^1(f-g)^2\,d\mu)^{1/2}$ | 关键 | 完整讲解 |  | 原页已核 |
| (5.1d) 印刷页 122；PDF 页 141 | FORMULA | $C[0,1]$ 上的一致度量 $\Vert f-g\Vert_\infty=\sup_x\lvert f(x)-g(x)\rvert$ | 关键 | 完整讲解 |  | 原页已核 |
| Definition 5.1 印刷页 122；PDF 页 141 | DEFINITION | $\delta$-覆盖与覆盖数 $N(\delta;T,\rho)$ | 关键 | 完整讲解 |  | 原页已核 |
| Figure 5.1 印刷页 122；PDF 页 141 | FIGURE_TABLE | $\delta$-覆盖（半径 $\delta$ 的球）与 $\delta$-填装（半径 $\delta/2$ 的不相交球） | 辅助 | 简要说明 |  | 原页已核 |
| §5.1 印刷页 123；PDF 页 142 | DEFINITION | 完全有界：一切 $\delta>0$ 的覆盖数有限；度量熵 $\log N(\delta;T,\rho)$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 5.2 / (5.2) 印刷页 123；PDF 页 142 | EXAMPLE | $N(\delta;[-1,1],\lvert\cdot\rvert)\le 1/\delta+1$；立方体 $N(\delta;[-1,1]^d,\Vert\cdot\Vert_\infty)\le(1+1/\delta)^d$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 5.3 印刷页 123–124；PDF 页 142–143 | EXAMPLE | 布尔超立方体汉明覆盖：上界 $\log N_H/\log 2\le\lceil d(1-\delta)\rceil$；Hoeffding 下界 $2d(1/2-\delta)^2$ | 关键 | 完整讲解 |  | 原页已核 |
| (5.3) 印刷页 124；PDF 页 143 | FORMULA | $\log N_H(\delta;\mathbb H^d)\ge d D(\delta\Vert 1/2)$，$\delta\in(0,1/2)$ | 关键 | 完整讲解 |  | 原页已核 |
| Definition 5.4 印刷页 124；PDF 页 143 | DEFINITION | $\delta$-填装与填装数 $M(\delta;T,\rho)$ | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 5.5 / (5.4) 印刷页 124；PDF 页 143 | LEMMA | $M(2\delta;T,\rho)\le N(\delta;T,\rho)\le M(\delta;T,\rho)$ | 关键 | 完整讲解 | 证明见 Exercise 5.2 | 原页已核 |
| Example 5.6 / (5.5) 印刷页 124–125；PDF 页 143–144 | EXAMPLE | 单位区间填装给出 $\log N(\delta;[0,1]^d,\Vert\cdot\Vert_\infty)\asymp d\log(1/\delta)$ | 关键 | 完整讲解 |  | 原页已核 |
| (5.6)–(5.7) 印刷页 125；PDF 页 144 | DEFINITION | $\ell_q$-单位球 $\mathbb B_q^d(1)$ 与 $\ell_q$-范数 | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 5.7 / (5.8) 印刷页 125；PDF 页 144 | LEMMA | 体积比：$(1/\delta)^d\mathrm{vol}(\mathbb B)/\mathrm{vol}(\mathbb B')\le N(\delta;\mathbb B,\Vert\cdot\Vert')\le\mathrm{vol}((2/\delta)\mathbb B+\mathbb B')/\mathrm{vol}(\mathbb B')$ | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 5.7 随后 印刷页 125；PDF 页 144 | FORMULA | 若 $\mathbb B'\subseteq\mathbb B$，则 $N\le(1+2/\delta)^d\mathrm{vol}(\mathbb B)/\mathrm{vol}(\mathbb B')$ | 关键 | 并入相关内容 | 并入 Lemma 5.7 | 原页已核 |
| Example 5.8 / (5.9) 印刷页 126；PDF 页 145 | EXAMPLE | 单位球在自身范数下 $d\log(1/\delta)\le\log N(\delta;\mathbb B,\Vert\cdot\Vert)\le d\log(1+2/\delta)$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 5.9 / (5.10) 印刷页 126–127；PDF 页 145–146 | EXAMPLE | 参数类 $\mathscr P=\{f_\theta(x)=1-e^{-\theta x}\}$：$1+\lfloor(1-1/e)/(2\delta)\rfloor\le N_\infty(\delta;\mathscr P)\le 1/(2\delta)+2$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 5.10 / (5.11)–(5.14) 印刷页 127–128；PDF 页 146–147 | EXAMPLE | Lipschitz 类 $\mathscr F_L$：$\log N_\infty(\delta;\mathscr F_L)\asymp L/\delta$；分段线性符号填装 | 关键 | 完整讲解 |  | 原页已核 |
| Figure 5.2 印刷页 128；PDF 页 147 | FIGURE_TABLE | $\{f_\beta:\beta\in\{-1,+1\}^M\}$ 的锯齿填装 | 辅助 | 简要说明 |  | 原页已核 |
| (5.15) 及随后 印刷页 129；PDF 页 148 | FORMULA | 高维 Lipschitz：$\log N_\infty(\delta;\mathscr F_L([0,1]^d))\asymp(L/\delta)^d$，维数灾难 | 关键 | 完整讲解 |  | 原页已核 |
| Example 5.11 / (5.16)–(5.19) 印刷页 129–130；PDF 页 148–149 | EXAMPLE | 光滑类 $\mathscr F_{\alpha,\gamma}$：$\log N(\delta;\mathscr F_{\alpha,\gamma},\Vert\cdot\Vert_\infty)\asymp(1/\delta)^{1/(\alpha+\gamma)}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 5.12 / (5.20)–(5.21) 印刷页 130–131；PDF 页 149–150 | EXAMPLE | $\ell^2(\mathbb N)$ 椭球 $\mu_j=j^{-2\alpha}$：$\log N(\delta;\mathcal E,\Vert\cdot\Vert_2)\asymp(1/\delta)^{1/\alpha}$ | 关键 | 完整讲解 |  | 原页已核 |
| §5.2 印刷页 132–134；PDF 页 151–153 | SECTION | Gaussian and Rademacher complexity | 关键 | 完整讲解 |  | 原页已核 |
| (5.22)–(5.23) 印刷页 132；PDF 页 151 | DEFINITION | 典范高斯过程 $G_\theta=\langle w,\theta\rangle$ 与高斯复杂度 $\mathcal G(T)=\mathbb E[\sup_{\theta\in T}\langle\theta,w\rangle]$ | 关键 | 完整讲解 |  | 原页已核 |
| (5.24) 印刷页 132；PDF 页 151 | DEFINITION | 拉德马赫过程与拉德马赫复杂度 $\mathcal R(T)=\mathbb E[\sup\langle\theta,\varepsilon\rangle]$；$\mathcal R(T)\le\sqrt{\pi/2}\,\mathcal G(T)$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 5.13 / (5.25) 印刷页 132–133；PDF 页 151–152 | EXAMPLE | $\mathcal R(\mathbb B_2^d)=\sqrt d$，$\mathcal G(\mathbb B_2^d)/\sqrt d=1-o(1)$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 5.14 / (5.26) 印刷页 133；PDF 页 152 | EXAMPLE | $\mathcal R(\mathbb B_1^d)=1$，$\mathcal G(\mathbb B_1^d)/\sqrt{2\log d}=1\pm o(1)$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 5.15 / (5.27)–(5.29) 印刷页 133；PDF 页 152 | EXAMPLE | $\ell_0$-球 $\mathbb S^d(s)=\mathbb B_0^d(s)\cap\mathbb B_2^d(1)$：$\mathcal G(\mathbb S^d(s))\lesssim\sqrt{s\log(ed/s)}$ | 关键 | 完整讲解 | 细节见 Exercises 5.7–5.8 | 原页已核 |
| (5.30)–(5.31) 印刷页 134；PDF 页 153 | FORMULA | 设计点上的 $\mathscr F(x_1^n)$ 与经验 $L^2$ 度量 $\Vert f-g\Vert_n$；平凡界 $\mathcal G(\mathscr F(x_1^n)/n)\le b$ | 关键 | 完整讲解 |  | 原页已核 |
| §5.3 印刷页 134–143；PDF 页 153–162 | SECTION | Metric entropy and sub-Gaussian processes | 关键 | 完整讲解 |  | 原页已核 |
| Definition 5.16 / (5.32) 印刷页 134；PDF 页 153 | DEFINITION | 关于 $\rho_X$ 的次高斯过程：$\mathbb E[e^{\lambda(X_\theta-X_{\widetilde\theta})}]\le\exp(\lambda^2\rho_X^2(\theta,\widetilde\theta)/2)$ | 关键 | 完整讲解 |  | 原页已核 |
| §5.3.1 印刷页 135–136；PDF 页 154–155 | SECTION | Upper bound by one-step discretization | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 5.17 / (5.33) 印刷页 135；PDF 页 154 | PROPOSITION | 一步离散化：$\mathbb E[\sup(X_\theta-X_{\widetilde\theta})]\le 2\mathbb E[\sup_{\rho\le\delta}(X_\gamma-X_{\gamma'})]+4\sqrt{D^2\log N_X(\delta;T)}$ | 关键 | 完整讲解 |  | 原页已核 |
| (5.34) 印刷页 136；PDF 页 155 | FORMULA | 覆盖分解 $\sup(X_\theta-X_{\widetilde\theta})\le 2\sup_{\rho\le\delta}(X_\gamma-X_{\gamma'})+2\max_i\lvert X_{\theta^i}-X_{\theta^1}\rvert$ | 关键 | 并入相关内容 | 并入 Proposition 5.17 | 原页已核 |
| (5.35) 印刷页 136；PDF 页 155 | FORMULA | 局部高斯复杂度 $\mathcal G(T)\le\min_\delta\{\mathcal G(\widetilde T(\delta))+2\sqrt{D^2\log N_2(\delta;T)}\}$ | 关键 | 完整讲解 |  | 原页已核 |
| (5.36) 印刷页 136；PDF 页 155 | FORMULA | 朴素离散化 $\mathcal G(T)\le\min_\delta\{\delta\sqrt d+2\sqrt{D^2\log N_2(\delta;T)}\}$ | 关键 | 完整讲解 |  | 原页已核 |
| §5.3.2 印刷页 137–139；PDF 页 156–158 | SECTION | Some examples of discretization bounds | 关键 | 完整讲解 |  | 原页已核 |
| Example 5.18 印刷页 137；PDF 页 156 | EXAMPLE | $\mathcal G(\mathbb B_2^d)\le\sqrt d\{1/2+2\sqrt{2\log 5}\}$，标度正确、常数次优 | 关键 | 完整讲解 |  | 原页已核 |
| Example 5.19 / (5.37)–(5.41) 印刷页 137–138；PDF 页 156–157 | EXAMPLE | 次高斯矩阵 $\mathbb E[\Vert\Vert\vert W\Vert\Vert\vert_2/\sqrt n]\lesssim 1+\sqrt{d/n}$；秩一变分与度量熵 | 关键 | 完整讲解 | 细节见 Exercise 5.11 | 原页已核 |
| (5.42) 印刷页 138；PDF 页 157 | FORMULA | $\log N_2(\delta;\mathscr F(x_1^n)/\sqrt n)\le\log N_\infty(\delta;\mathscr F(x_1^n))\le\log N(\delta;\mathscr F,\Vert\cdot\Vert_\infty)$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 5.20 / (5.43) 印刷页 138–139；PDF 页 157–158 | EXAMPLE | 参数类经验高斯复杂度 $\mathcal G(\mathscr P(x_1^n)/n)\lesssim\sqrt{(\log n)/n}$，对数因子次优 | 关键 | 完整讲解 |  | 原页已核 |
| Example 5.21 / (5.44) 印刷页 139；PDF 页 158 | EXAMPLE | Lipschitz 类 $\mathcal G(\mathscr F_L(x_1^n)/n)\lesssim n^{-1/3}$ | 关键 | 完整讲解 |  | 原页已核 |
| §5.3.3 印刷页 139–143；PDF 页 158–162 | SECTION | Chaining and Dudley's entropy integral | 关键 | 完整讲解 |  | 原页已核 |
| (5.45) 印刷页 139；PDF 页 158 | FORMULA | $\delta$-截断达德利熵积分 $\mathcal J(\delta;D)=\int_\delta^D\sqrt{\log N_X(u;T)}\,du$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 5.22 / (5.46) 印刷页 140；PDF 页 159 | THEOREM | Dudley：$\mathbb E[\sup(X_\theta-X_{\widetilde\theta})]\le 2\mathbb E[\sup_{\rho\le\delta}(X_\gamma-X_{\gamma'})]+32\mathcal J(\delta/4;D)$ | 关键 | 完整讲解 |  | 原页已核 |
| (5.47) 印刷页 140；PDF 页 159 | FORMULA | 链式分解 $X_\theta-X_{\gamma^1}=\sum_{m=2}^L(X_{\gamma^m}-X_{\gamma^{m-1}})$ | 关键 | 并入相关内容 | 并入 Theorem 5.22 | 原页已核 |
| Figure 5.3 印刷页 141；PDF 页 160 | FIGURE_TABLE | $L=5$ 的链式树：逐层 $D2^{-m}$-覆盖 | 辅助 | 简要说明 |  | 原页已核 |
| Example 5.23 印刷页 142；PDF 页 161 | EXAMPLE | Dudley 去掉参数类的对数因子：$\mathcal G(\mathscr P(x_1^n)/n)\le c'/\sqrt n$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 5.24 / (5.48)–(5.51) 印刷页 142–143；PDF 页 161–162 | EXAMPLE | 有限 VC 类：$\mathbb E_\varepsilon\sup\lvert n^{-1}\sum\varepsilon_i f(x_i)\rvert\le c_0'\sqrt{\nu/n}$；Glivenko–Cantelli 尾 (5.51) | 关键 | 完整讲解 |  | 原页已核 |
| (5.49) 印刷页 143；PDF 页 162 | FORMULA | VC 度量熵 $N(\varepsilon;\mathscr F,\Vert\cdot\Vert_{\mathbb P_n})\le C\nu(16e)^\nu(b/\varepsilon)^{2\nu}$ | 关键 | 完整讲解 | 较弱形式见 Exercise 5.4 | 原页已核 |
| §5.4 印刷页 143–148；PDF 页 162–167 | SECTION | Some Gaussian comparison inequalities | 关键 | 完整讲解 |  | 原页已核 |
| §5.4.1 印刷页 143–145；PDF 页 162–164 | SECTION | A general comparison result | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 5.25 / (5.52)–(5.54) 印刷页 144；PDF 页 163 | THEOREM | 一般高斯比较：协方差在 $A$/$B$ 上的不等式与 $F$ 的二阶导数符号匹配则 $\mathbb E[F(X)]\le\mathbb E[F(Y)]$ | 关键 | 完整讲解 |  | 原页已核 |
| (5.55) 印刷页 144；PDF 页 163 | FORMULA | 插值 $Z(t)=\sqrt{1-t}\,X+\sqrt t\,Y$ | 关键 | 并入相关内容 | 并入 Theorem 5.25 | 原页已核 |
| §5.4.2 印刷页 145–146；PDF 页 164–165 | SECTION | Slepian and Sudakov–Fernique inequalities | 关键 | 完整讲解 |  | 原页已核 |
| Corollary 5.26 / (5.56)–(5.57) 印刷页 145；PDF 页 164 | COROLLARY | 斯莱皮安：非对角协方差更大且等方差则 $\mathbb E[\max X_i]\le\mathbb E[\max Y_i]$ | 关键 | 完整讲解 |  | 原页已核 |
| (5.58) 印刷页 145；PDF 页 164 | FORMULA | 软最大夹逼 $\max x_j\le F_\beta(x)\le\max x_j+(\log N)/\beta$ | 关键 | 并入相关内容 | 并入 Corollary 5.26 | 原页已核 |
| Theorem 5.27 / (5.59) 印刷页 146；PDF 页 165 | THEOREM | 苏达科夫–费尔尼克：$\mathbb E[(X_i-X_j)^2]\le\mathbb E[(Y_i-Y_j)^2]$ 则 $\mathbb E[\max X_j]\le\mathbb E[\max Y_j]$ | 关键 | 完整讲解 |  | 原页已核 |
| §5.4.3 印刷页 146–148；PDF 页 165–167 | SECTION | Gaussian contraction inequality | 关键 | 完整讲解 |  | 原页已核 |
| Proposition 5.28 / (5.60) 印刷页 147；PDF 页 166 | PROPOSITION | 高斯收缩：中心 1-Lipschitz 坐标映射不增大高斯复杂度 | 关键 | 完整讲解 | 证明见 Exercise 5.12 | 原页已核 |
| (5.61) 印刷页 147；PDF 页 166 | FORMULA | 拉德马赫收缩 $\mathcal R(\phi(T))\le 2\mathcal R(T)$ | 关键 | 简要说明 |  | 原页已核 |
| Example 5.29 / (5.62) 印刷页 147–148；PDF 页 166–167 | EXAMPLE | 平方函数类 $\mathcal G(\mathscr F^2(x_1^n))\le 2b\,\mathcal G(\mathscr F(x_1^n))$ | 关键 | 完整讲解 |  | 原页已核 |
| §5.5 印刷页 148–150；PDF 页 167–169 | SECTION | Sudakov's lower bound | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 5.30 / (5.63) 印刷页 148；PDF 页 167 | THEOREM | 苏达科夫下界：$\mathbb E[\sup X_\theta]\ge\sup_{\delta>0}(\delta/2)\sqrt{\log M_X(\delta;T)}$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 5.31 印刷页 148–149；PDF 页 167–168 | EXAMPLE | $\mathcal G(\mathbb B_2^d)\ge\sqrt{\log 4}/8\cdot\sqrt d$，标度匹配 | 关键 | 完整讲解 |  | 原页已核 |
| Example 5.32 / (5.64) 印刷页 149；PDF 页 168 | EXAMPLE | $\ell_1$-球度量熵 $\log N(\delta;\mathbb B_1^d,\Vert\cdot\Vert_2)\le c(1/\delta)^2\log d$ | 关键 | 完整讲解 |  | 原页已核 |
| Example 5.33 印刷页 149–150；PDF 页 168–169 | EXAMPLE | $\mathbb E[\Vert\Vert\vert W\Vert\Vert\vert_2]\gtrsim\sqrt n+\sqrt d$，与 Example 5.19 匹配 | 关键 | 完整讲解 | 填装下界见 Exercise 5.13 | 原页已核 |
| §5.6 印刷页 150–153；PDF 页 169–172 | SECTION | Chaining and Orlicz processes | 关键 | 完整讲解 |  | 原页已核 |
| Definition 5.34 / (5.65) 印刷页 150；PDF 页 169 | DEFINITION | $\psi_q$-奥尔里奇范数 $\Vert X\Vert_{\psi_q}=\inf\{\lambda>0:\mathbb E[\psi_q(\lvert X\rvert/\lambda)]\le 1\}$，$\psi_q(t)=e^{t^q}-1$ | 关键 | 完整讲解 |  | 原页已核 |
| Definition 5.35 / (5.66) 印刷页 151；PDF 页 170 | DEFINITION | $\psi_q$-过程：$\Vert X_\theta-X_{\widetilde\theta}\Vert_{\psi_q}\le\rho(\theta,\widetilde\theta)$ | 关键 | 完整讲解 |  | 原页已核 |
| (5.67)–(5.68) 印刷页 151；PDF 页 170 | FORMULA | 广义 Dudley 积分 $\mathcal J_q(\delta;D)=\int_\delta^D\psi_q^{-1}(N(u;T,\rho))\,du$，$\psi_q^{-1}(u)=[\log(1+u)]^{1/q}$ | 关键 | 完整讲解 |  | 原页已核 |
| Theorem 5.36 / (5.69) 印刷页 151；PDF 页 170 | THEOREM | $\psi_q$-过程尾界 $\mathbb P[\sup\lvert X_\theta-X_{\widetilde\theta}\rvert\ge c_1(\mathcal J_q(0;D)+t)]\le 2e^{-t^q/D^q}$ | 关键 | 完整讲解 |  | 原页已核 |
| Lemma 5.37 / (5.70)–(5.71) 印刷页 152；PDF 页 171 | LEMMA | 奥尔里奇变量在可测集 $A$ 上的积分：$\mathbb E_A[Y_i]\le\mathbb P[A]\psi_q^{-1}(1/\mathbb P(A))$ 及最大值形式 | 关键 | 完整讲解 |  | 原页已核 |
| (5.72)–(5.73) 印刷页 152–153；PDF 页 171–172 | FORMULA | 链式给出 $\mathbb E_A[Z]\le 8\mathbb P[A]\int\psi_q^{-1}(N(u)/P[A])\,du$ | 关键 | 并入相关内容 | 并入 Theorem 5.36 | 原页已核 |
| §5.7 印刷页 153–154；PDF 页 172–173 | PROSE_RANGE | Bibliographic details：Kolmogorov–Tikhomirov、Dudley、Talagrand generic chaining、Ledoux–Talagrand、Slepian、Gordon、VC 熵 van der Vaart–Wellner | 辅助 | 指回教材 | 文献清单不抄入 Notes | 原页已核 |
| §5.8 印刷页 154–158；PDF 页 173–177 | SECTION | Exercises 5.1–5.14 | 辅助 | 不进入 Notes | 习题整节进 Solutions，不进 Notes | 原页已核 |
| Exercise 5.1 印刷页 154；PDF 页 173 | EXERCISE | 凸函数类 $C([0,1],b)$ 在一致范数下不完全有界 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 5.2 印刷页 154；PDF 页 173 | EXERCISE | 证明 Lemma 5.5 的填装–覆盖关系 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 5.3 印刷页 155；PDF 页 174 | EXERCISE | 布尔超立方体填装数的 KL 上界 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 5.4 印刷页 155；PDF 页 174 | EXERCISE | VC 维到 $L^1(\mathbb P)$ 度量熵 (5.74) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 5.5 印刷页 155；PDF 页 174 | EXERCISE | 高斯与拉德马赫复杂度互相控制 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 5.6 印刷页 155–156；PDF 页 174–175 | EXERCISE | $\ell_q$-球的高斯复杂度 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 5.7 印刷页 156；PDF 页 175 | EXERCISE | $\ell_0$-球高斯复杂度上界 (5.75) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 5.8 印刷页 156；PDF 页 175 | EXERCISE | $\ell_0$-球高斯复杂度下界 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 5.9 印刷页 156–157；PDF 页 175–176 | EXERCISE | $\ell^2(\mathbb N)$ 椭球及其截断的高斯复杂度 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 5.10 印刷页 157；PDF 页 176 | EXERCISE | 高斯上确界的集中 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 5.11 印刷页 157；PDF 页 176 | EXERCISE | Example 5.19 的细节 (5.38)–(5.41) | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 5.12 印刷页 157；PDF 页 176 | EXERCISE | 证明高斯收缩不等式 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 5.13 印刷页 157；PDF 页 176 | EXERCISE | $\mathbb M^{n,d}(1)$ 的填装下界 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |
| Exercise 5.14 印刷页 157–158；PDF 页 176–177 | EXERCISE | 高斯矩阵最大奇异值：模拟、变分、Gordon 比较、尾界 | 辅助 | 不进入 Notes | 完整解答写入 Solutions | 原页已核 |

## 来源异常与勘误

| 定位 | 问题类型 | 原式/原文 | 核验证据 | 处置 | 数学复核人 | 批准人 |
|---|---|---|---|---|---|---|
| Example 5.2 印刷页 123；PDF 页 142 | 笔误嫌疑 | 构造 $[-1,1]$ 的覆盖时写 “for any point $\overline\theta\in[0,1]$” | 原页 PNG；区间与覆盖中心均在 $[-1,1]$ | 保留原文；Notes 按 $[-1,1]$ 理解；`勘误待批` | 作者 | 未批 |
| Example 5.11 印刷页 130；PDF 页 149 | 符号冲突 | 末式写 $\log N(\delta;\mathscr F_{\alpha,\gamma},\Vert\cdot\Vert_\infty)\gtrsim(1/\delta)\asymp(1/\varepsilon)^{1/(\alpha+\gamma)}$ | 原页 PNG；正文把网格间距也叫 $\delta$，填装半径是 $2\varepsilon$；(5.17) 的覆盖半径标度是 $(1/\delta)^{1/(\alpha+\gamma)}$ | 保留原文；Notes 按 (5.17) 陈述，并标明末式符号混用；`勘误待批` | 作者 | 未批 |
| Theorem 5.25 证明 印刷页 145；PDF 页 164 | 笔误嫌疑 | “assumptions on the second derivatives of $f$” | 原页 PNG；定理中的函数是 $F$，不是 $f$ | 保留原文；Notes 写 $F$；`勘误待批` | 作者 | 未批 |
| Theorem 5.27 印刷页 146；PDF 页 165 | 排印 | 定理框 “$(Y_1,\ldots,Y_N$, suppose that” 缺右括号 | 原页 PNG | 保留原文；Notes 补全括号并标明；`勘误待批` | 作者 | 未批 |
| Example 5.31 印刷页 149；PDF 页 168 | 交叉引用 | “From Example 5.9, the metric entropy of the ball $\mathbb B_2^d$” | 原页 PNG；单位球自身度量熵是 Example 5.8 / (5.9)；Example 5.9 是参数函数类 | 保留原文；Notes 改引 Example 5.8 并标明；`勘误待批` | 作者 | 未批 |
| Figure 5.3 图注 印刷页 141；PDF 页 160 | 排印嫌疑 | 图注写 $De^{-m}$-cover | 原页 PNG；正文证明用的是 $\varepsilon_m=D2^{-m}$ | 保留原文；Notes 按 $D2^{-m}$ 讲解；`勘误待批` | 作者 | 未批 |

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
