# Projection on 1D subspaces

- Orthogonal projections play a central role in dimensionality reduction
- $\pi_u(x)$ denotes the projection of vector $x$ on a subspace $u$
- Projection properties
  - $\pi_u(x) \epsilon U => \exists \text{  }\lambda \epsilon \text{ such that} \pi_u(x) = \lambda b$
  - $<b, \pi_u(x)-x> = 0$ i.e they are orthogonal to each other

- By solving the above two equations, we get

$$\lambda = \frac{<b,x>}{||b||^2}$$

- And $\pi_u(x)$(which represents projection of x on b) is expressed as

$$\pi_u(x)=\frac{x^Tb}{||b||^2}b$$ 
