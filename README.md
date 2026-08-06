# The Missing Horizon in Random Reshuffling

## Abstract

Random reshuffling now has an upper bound that dominates stochastic gradient descent at every stable constant step size and every finite horizon. Its matching lower bound was left open. We solve this problem for the exact all-inner average used by the upper bound. The answer is not the published horizon-independent stochastic envelope. If $\alpha=\eta nL\leq 1$, the fixed-step minimax stochastic error is

$$\Theta\\!\left(\eta^2 n L\sigma_\star^2\\,\left[K^{-1}+\min\\{(\alpha K)^2,\\,1\\}\right]\right).$$

It decreases, increases, and then plateaus across three horizon regimes. Its minimum occurs at $K\asymp\alpha^{-2/3}$, before the usual mixing scale $\alpha^{-1}$. For $\alpha\geq 1$, the law is $\Theta(\eta\sigma_\star^2)$.

The upper bound follows from an exact finite-population bridge identity and a dimension-free control of all state memory as a Lipschitz remainder. The lower bound combines a centered common-Hessian bridge with a rectifying piecewise quadratic in two dimensions. An exact telescoping identity explains why common-Hessian quadratics alone miss the eventual floor. Together with the deterministic term, this gives a complete minimax characterization for all horizons and all stable constant steps. Optimizing the step recovers the best known tuned rate, while the fixed-step landscape is genuinely richer than the tuned rate suggests.

## Main results

**Theorem (All steps and all horizons).** There are universal constants $c,C>0$ such that for every $n\geq 8$, $K\geq 1$, $L>0$, $D,\sigma\geq 0$, and $0<\eta\leq 1/(6L)$,

$$c\left[\min\\!\left\\{LD^2,\\,\frac{D^2}{\eta nK}\right\\}+\mathcal S_{n,K}\right] \leq \mathcal R_{n,K}(\eta,L,D,\sigma) \leq C\left[\min\\!\left\\{LD^2,\\,\frac{D^2}{\eta nK}\right\\}+\mathcal S_{n,K}\right].$$

The lower bound is attained in dimension at most two. For even $n$ it uses balanced signs. For odd $n$ the same construction uses one zero sign. The stochastic term $\mathcal S_{n,K}$ carries the three-phase horizon dependence of the abstract.

**Corollary (Tuned constant step).** Minimizing the theorem over stable constant steps recovers, up to universal constants,

$$\frac{LD^2}{nK}+\min\\!\left\\{\frac{\sigma D}{\sqrt{nK}},\ \left(\frac{L\sigma^2 D^4}{nK^2}\right)^{1/3}\right\\}.$$

The transient dip in the fixed-step minimax law does not appear in the tuned envelope: tuning is free to move the trajectory to a different phase.

**Upper bound method.** A reset bridge identity plus a dimension-free Lipschitz remainder controls all state memory. The bridge yields the exact leading stochastic constant. The remainder is bounded independently of dimension by a single one-dimensional argument.

**Lower bound method.** A centered common-Hessian bridge captures the first two phases. A rectifying piecewise quadratic in two dimensions produces the plateau. A telescoping identity for common-Hessian quadratics shows why they cannot reach the floor alone. The construction uses balanced-sign labels in even $n$ and one zero-sign label in odd $n$.

## Keywords

random reshuffling, without-replacement SGD, stochastic gradient descent, minimax lower bound, horizon dependence, finite-population bridge, common-Hessian quadratic, constant step size

## Files

- `main.pdf`
- `main.tex`
- `references.bib`
- `iclr2027_conference.sty`, `iclr2027_conference.bst`, `natbib.sty`, `fancyhdr.sty`
- `supplement.zip` bundled auxiliary material
- `main.pdf.ots`, `README.md.ots`, `supplement.zip.ots` OpenTimestamps priority proofs
