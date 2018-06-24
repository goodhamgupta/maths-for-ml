# Projections in Higher Dimensions

- If we have a vector $X \epsilon \mathbb{R}^3$ and a 2D subspace descriped by the basis vectors

$$u = [b_1, b_2]$$

- The orthogonal projection of $X$ on $u$ will be $\pi_u(X)$
  - $\pi_u(X)$ can be expressed as a linear combination of the basis vectors of $u$
  $$\pi_u(X) = \lambda_1b_1+\lambda_2b_2$$
  - Difference vector is orthogonal to $u$, which implies that it is orthogonal to all basis vectors of $u$
  $$<x-\pi_u(X), b_u> = 0$$
  
$$\lambda = (B^TB)^{-1}B^TX$$
$$\pi_u(X) = B\lambda=B(B^TB)^{-1}B^TX $$

- Hence we get

$$\lambda = \frac{b^Tx}{b^Tb}$$
$$\pi_u(x) = B\lambda = \frac{b^Tx}{b^Tb}b$$

