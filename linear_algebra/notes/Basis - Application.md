# Basis - Application

- $e_0 = \begin{bmatrix}1\\0\end{bmatrix}$ $e_1 = \begin{bmatrix}0\\1\end{bmatrix}$

## Basis
- Set of n vectors that
  - Are NOT linear combinations of each other(linearly independant)
  - Span the space they describe
    - The space is then n dimensional(important)

- They do NOT have to 
  - be unit vectors
  - be orthogonal
- BUT it'll be easier if they are

## Orthogonal Basis set

- All basis vectors that are orthogonal to each other and are unit vectors
- These will simplify the computation required.
- If they are not orthogonal, we CANNOT map a vector in one set of basis vectors(say $\hat{e}$) to another(say $\hat{b}$). WE WILL HAVE TO USE MATRICES

## Applications of changing basis

- Can be used to measure the fit of of a line in linear regression
- In neural networks
  - Derive set of basis vectors that can extract the most information rich features of the object(such as faces, cars, etc)
