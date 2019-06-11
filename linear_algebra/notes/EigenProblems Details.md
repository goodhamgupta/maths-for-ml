# EigenProblems Details

## Special eigen-cases

- Uniform scaling
  - Any vector in this will be an eigenvector
- Rotation
  - Small rotation has no eigenvectors
  - BUT, rotation of $180\degree$ has _infinite_ eigenvectors as after rotation the vector will just be in the opposite direction(i.e they will still lie on the same span). The eigenvalues for them will be $-1$ as the direction has changed
- Horizontal shear + vertical scaling
  - This will have TWO eigenvectors
    - The horizontal vector will be an eigenvector with value one. 
    - The vector between the pink and the orange vectors.(see from minute 1:30 [here](https://www.coursera.org/learn/linear-algebra-machine-learning/lecture/urLNy/special-eigen-cases))
- For 3D rotation, two of the three vectors will change but there will be one eigenvector. If we find the eigenvector, it implies that we have found the axis of rotation

## Calculating Eigenvectors

- For our transformation matrix $\boldsymbol{A}$ and our eigenvector(say $x$), we can calculate our eigenvector as

$$\boldsymbol{A}x = \lambda{}x$$
- $\lambda{}$ is just some number. We will find the values of x for which both sides are equal.
- A must be an $nxn$ matrix
- Solving this we get
$$= (\boldsymbol{A}-\lambda{})x=0$$
$$= (\boldsymbol{A}-\boldsymbol{I}\lambda{})x=0$$

- $\boldsymbol{I}$ is necessary because $\lambda$ is a scalar. Scalars cannot be subtracted from matrices. Hence, multiplying by $\boldsymbol{I}$ ensures that we get the scalar in the matrix format without changing the meaning.
- When we solve the above equation, if we get $x$ as 0, then the vector has no length or direction. This is called a _trivial solution_
- We can test if $(\boldsymbol{A}-\boldsymbol{I}\lambda{})$ gives 0 by calculating it's determinant
- The polynomail obtained when solving $det(\boldsymbol{A}-\boldsymbol{I}\lambda{})$ is called CHARACTERISTIC POLYNOMIAL
- Watch [video](https://www.coursera.org/learn/linear-algebra-machine-learning/lecture/We8G9/calculating-eigenvectors) for examples
