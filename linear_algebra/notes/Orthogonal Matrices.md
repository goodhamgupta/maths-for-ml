# Orthogonal Matrices

## Transpose

- Rows of the matrix become it's columns and vice-versa
- Flip elements that are NOT on the leading diagonal
$$(A_{ij})^{T} = A_{ji} $$

- Consider a matrix of size `n x n` which contains the basis vectors as column vectors
- Let $\hat{a}$ represent these vectors
- Each of the above vectors are unit length(hence the $\hat{a}$. This is a property of orthogonal matrices)
- Each of the vectors are orthogonal to each other 
$$a_i.a_j = 0 \text{ for }i!=j$$
$$a_i.a_j = 1 \text{ for }i=j$$
- When we _transpose_ the matrix, the column vectors will become row vectors.
- Therefore, multiplying $\boldsymbol{A^T}$ with $\boldsymbol{A}$ we get the identity matrix
$$\boldsymbol{A^T} . \boldsymbol{A} = \boldsymbol{I}$$
- We also know 
$$\boldsymbol{A^{-1}} . \boldsymbol{A} = \boldsymbol{I}$$
$$=> \boldsymbol{A^T} = \boldsymbol{A^{-1}}$$

- Hence, for orthonormal basis vectors, the transpose of the matrix WILL BE EQUAL TO the inverse of the matrix.
- Since all the vectors of a orthogonal matrix are unit vectors, it MUST SCALE SPACE by a factor of ONE. Therefore
$$|A| = \pm1$$
- `-1` arises if the unit vectors are inverted => they point in the opposite direction
- 
