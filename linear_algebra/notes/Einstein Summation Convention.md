# Einstein Summation Convention


$$ab_{ik} = \sum_{j}a_{ij} * b_{jk} \text{for all possible values of j}$$

$$= a_ibi\text{ (notation without the sigma symbol)}$$

- If we have a matrix A of size `n x m` and B of size `o x p` we can multiply them only if `m = o`
- When we do dot product of two vectors say `u` and `v`, they can be expressed as a matrix product
$$\vec{u}.\vec{v}$$
$$= \begin{bmatrix}u1&u2&u3&un\\\end{bmatrix}\begin{bmatrix}v1\\v2\\v3\\vn\\\end{bmatrix}$$

- Matrix multiplication => projection of a vector onto the vectors which represent the matrix i.e the vectors representing the columns of the matrix(minute 8:30 onwards [here](https://www.coursera.org/learn/linear-algebra-machine-learning/lecture/kI0DB/introduction-einstein-summation-convention-and-the-symmetry-of-the-dot-product))
