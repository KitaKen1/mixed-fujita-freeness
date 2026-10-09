# Mixed Fujita Freeness and Linear Effective Base-Point Freeness

The mixed Fujita freeness conjecture asks for the following global generation statement.

> [!NOTE]
> **Conjecture (Mixed Fujita freeness).**
>
> Let $X$ be a smooth complex projective variety of dimension $n\ge 1$. For every collection of ample Cartier divisors $L_1,\ldots,L_s$ with $s\ge n+1$, and every nef Cartier divisor $N$, the adjoint divisor
>
> $$
> K_X+L_1+\cdots+L_s+N
> $$
>
> is globally generated.

The ample divisors may be chosen independently. For $N=0$, the statement gives the bound $\operatorname{Fu}(X)\le\dim X+1$ for the convex Fujita number.

The manuscript also proposes the following effective bound for klt pairs.

> [!NOTE]
> **Claim (Linear effective base-point freeness).**
>
> Let $(X,\Delta)$ be a complex projective klt pair with effective rational boundary, and let $D$ be nef Cartier. If $a\ge1$ is an integer and $aD-(K_X+\Delta)$ is nef and big, then $mD$ is globally generated for every integer
>
> $$
> m\ge a+\nu(D)+1.
> $$

Here $\nu(D)$ denotes the numerical dimension of $D$.

This repository presents proposed proofs of these statements for submission to **Formal Conjectures**. A proof sketch follows; the [PDF manuscript](PDF/mixed-fujita-freeness.pdf) contains the detailed proof.

## Proof sketch

### 1. Prove numerical freeness

For a projective klt pair $(V,B)$ with $B\ge0$, let $P$ be Cartier and $A=P-(K_V+B)$ ample $\mathbb Q$-Cartier. We prove that

$$
A^n>(n+1)^n,\qquad A^d\cdot W\ge(n+1)^d
$$

for every positive-dimensional proper integral subvariety $W$ implies that $P$ is globally generated. In the smooth case $P=K_X+A+N$, with $A$ ample Cartier and $N$ nef Cartier, the volume equality is also allowed.

### 2. Minimize and isolate a point

For an ample Cartier multiple $L$ of $A$, minimize

$$
\frac1{N_j}\sum_i\exp\!\left(\frac{\mathrm A_{V,B}(v)}t-\frac{v(s_i)}j\right)
$$

over bases of $H^0(V,jL)$ and valuations whose closed centers contain a fixed point. Uniform valuation bounds and closed threshold loci give attainment. Uniform growth of restriction images and tangential variation exclude positive-dimensional minimizing centers. Rational isolation and Kawamata–Viehweg vanishing then produce a section nonzero at the point. A separate blowup argument handles smooth volume equality.

### 3. Apply the criteria

For $A=\sum_iL_i$, mixed intersection numbers are positive integers, so $A^d\cdot W\ge s^d\ge(n+1)^d$. The smooth criterion proves mixed Fujita freeness.

For the second statement, two consecutive globally generated powers descend $D$ to an ample Cartier divisor $H$ on a base $Y$ of dimension $\nu(D)$. A small boundary perturbation and Ambro's descent give an effective klt boundary with $K_Y+B_Y\sim_{\mathbb Q}(a-\varepsilon)H$. The klt numerical criterion applies to $mH$ for every $m\ge a+\nu(D)+1$; pullback gives the result.

## Detailed manuscript

- [PDF manuscript](PDF/mixed-fujita-freeness.pdf)

Public draft 2, 9 October 2026.
