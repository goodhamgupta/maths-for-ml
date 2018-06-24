# Dot Product

- _Inner product_ allows us to talk about geometric products in the vector space such as distances, angles, lengths of the vectors, etc.
- The dot product of two vectors $X$ and $Y$ is defined as

$$X.Y=X^TY=\sum_{i=1}^Nx_iy_i \text{ where } X, Y \in \mathcal{R}^N$$

- The length of $X$ is defined as the square root of the dot product of X with ITSELF

$$||X||=\sqrt{X^TX}=\sqrt{\sum_{i=1}^N{x_i^2}}$$

- _Distance_ between two vectors $X$ and $Y$ is computed by the length of the DIFFERENCE VECTOR i.e

$$d(X,Y) = ||(X-Y)||=\sqrt{(X-Y)^T(X-Y)}$$

- _Angle between two vectors_
  - From course 1, we know using the cosine rule

  $$X.Y=||X||||Y||cos\theta$$
  
  $$cos\theta=\frac{X.Y}{||X|||*|Y||}$$
  $$cos\theta=\frac{X^TY}{||X||*||Y||}$$