# Changing Eigenbasis

- Combining eigenvectors with changing basis concept
  - Helps in performing efficient matrix operations called _diagonalisation_

## Diagonal matrix
- All terms are 0 expect the terms on the leading diagonal 
- Make things easier when computing powers of matrices($\boldsymbol{T}, \boldsymbol{T}^2, \boldsymbol{T}^n, etc$)
  - Only the terms on the diagonal will be affected by the power
  - Example
$$\boldsymbol{T} = \begin{bmatrix}3&0\\0&3\end{bmatrix}$$
$$\boldsymbol{T}^2 = \begin{bmatrix}9&0\\0&9\end{bmatrix}$$
$$\boldsymbol{T}^5 = \begin{bmatrix}243&0\\0&243\end{bmatrix}$$

- What if $\boldsymbol{T}$ is not a diagonal matrix?
  - Use eigen-analysis
  - Change to a basis where $\boldsymbol{T}$ becomes a diagonal matrix
  - This basis is called _eigen-basis_
  - Apply _n_ to the diagonalized form
  - Transform back to our basis to get the result

$$\boldsymbol{T}^n = \boldsymbol{C}^{-1}D^n\boldsymbol{C}$$
