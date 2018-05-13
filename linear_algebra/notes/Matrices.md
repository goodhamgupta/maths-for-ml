# Matrices

## Linear algebra

- Maths system for manipulating systems/vectors
- Mostly used to transform vectors using matrices
- Used to solve the problem of simultaneous matrix


## How matrices transform space

- Applying one matrix transformation after another is called `composition`
- $\boldsymbol{A}\text{ } r =\hat{r}$
- $\boldsymbol{A}\text{ }(nr) =n\hat{r}$
- $\boldsymbol{A}\text{ }(r+s) =\boldsymbol{A}\hat{r} + \boldsymbol{A}\hat{s}$

$$\boldsymbol{A}(\hat{n\hat{e_1}}+\hat{m\hat{e_2}})$$
$$= A{n\hat{e_1}} + A{m\hat{e_2}}$$
$$= ne_1^\prime + ne_2^\prime$$

- All vector sums will work
- Check the example in [this](https://www.coursera.org/learn/linear-algebra-machine-learning/lecture/IhJAZ/how-matrices-transform-space) video to verify all operations work


## Types of matrix transformation

- $\boldsymbol{I}$ => This type of matrix does not perform any transformation i.e leaves the matrix the same. It is called `identity` matrix.
- $e_0 = \begin{bmatrix}3&0\\0&2\end{bmatrix}$  => This will scale the x axis by a factor of 3 and the y axis by a factor of 2
- $e_0 = \begin{bmatrix}-1&0\\0&-1\end{bmatrix}$ => Inverts both coordinates. This is called an `inversion`.
- $e_0 = \begin{bmatrix}0&1\\1&0\end{bmatrix}$ => Makes x axis as y axis and vice version. It's like putting a mirror at $45\degree$ which passes through the origin
- `Shear` => Change only one of the coordinates
- Rotation matrix: $\begin{bmatrix}cos\theta&sin\theta\\sin\theta&cos\theta\end{bmatrix}$ 
- If same rotation with `z` axis, preserve the z axis
$$\begin{bmatrix}cos\theta&sin\theta&0\\sin\theta&cos\theta&0\\0&0&1\end{bmatrix}$$

## Combination of matrix transforms

- Any combo of matrix transformations can be applied to a vector
- The order of the transforms applied DOES NOT matter.

