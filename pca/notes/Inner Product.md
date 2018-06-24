# Inner Product

- Generalization of dot product to compute angles, lengths and distances
- For vectors $X$ and $Y$ in $V$, a _inner product_ is defined as a symetric, positive definite, bilinear mapping 
- We take a mapping from these two vector

$$<.i.> : V x V -> \mathcal R$$
This function is symmetric, positive definite and bilinear

## Bilinearity

- Linearity in both arguments of the function
$$\text{For }x,y,z \epsilon V, \lambda \epsilon \mathcal R$$
$$<\lambda x+z, y> = \lambda<x,y>+<z,y>$$
$$<x, \lambda y + z> = \lambda<x,y>+<x,y>$$

## Positive Definite

$$<x,x> = 0, \text{ only if } x=\vec{0}$$

## Symmetric

- Order of the vector in the inner product does not matter

$$<x,y> = <y,x>$$

- To check for inner product properties, apply the following

  - _Symmetric_ :  Check if the off-diagonal elements are the same. If they are then it will be symmetric
  - _Bilinear_ :  Check if there are no quadratic or higher order items that are possible. For example, if x.T@A@y has no overlapping terms, then it will be bilinear.
  - _Positive Definite_ :
    1) Check if $b^2 - ac < 0$ (determinent) for every sub-matrix in the matrix. For example, for a 4x4 start with a[0,0], then a[0,0] to a[1,1], then a[0,0] to a[2,2] and so on.

    2) Check if a[0,0] > 0

