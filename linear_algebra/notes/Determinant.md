# Determinant

- Used to define the factor by which the  current space has expanded. For example
$$\begin{bmatrix}a&0\\0&d\end{bmatrix}$$

- Above matrix implies that x axis has been expanded by `a` and y axis by `d`. The area of the rectangle formed `ad` is called the determinant
- For a matrix below
$$\begin{bmatrix}a&b\\c&d\end{bmatrix}$$
- Determinant will be 
```
ad - bc
```

## Singular Matrix

- Matrices that do not have an inverse are called singular matrices
  - If there are any zeros left on the leading diagonal that CANNOT be removed, it causes the matrix to be singular
  - When one row can be expressed as a direct linear combination of the other rows, it will cause the matrix to be singular
  - Determinant = 0 => Basis vectors are NOT linearly independant => Inverse does not exist => Matrix is singular
