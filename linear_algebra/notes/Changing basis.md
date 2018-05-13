# Changing basis

- The coordinate system is represented by unit vectors
- Any vector can be represented as a linear combination of these unit vectors
- The unit vectors/vectors that are used to define the vector space are called `basis vectors`


## Finding components with different basis vectors

- We can compute the coordinates for the new basis vectors using `dot` products.
- `dot` product is computationally faster and easier to compute when the basis vectors are orthogonal to each other.

### Steps

- Given a vector `r` whose coordinates are mapped using basis vectors $\hat{e_1}$ and $\hat{e_2}$ and we have two new vectors called $\hat{b_1}$ and $\hat{b_2}$
- $r_e$ => e as basis vector
- $r_b$ => b as basis vector
- Find projection of r on $\hat{b_1}$
- Find projection of r on $\hat{b_2}$
- Check if the vectors $\hat{b_1}$ and $\hat{b_2}$ are orthogonal by taking their `dot` product.

$$\cos{\theta} = \frac{b_1.b_2}{|b_1||b_2|}$$

- $cos\theta$ will be ZERO if the vectors are orthogonal
- Hence, to calcuate coordinates of $r_b$, apply the following

$$\frac{r_e.b1}{|b1|^2}$$
$$\frac{r_e.b2}{|b2|^2}$$

- General formula
$$\frac{r_e.bn}{|bn|^2}$$

