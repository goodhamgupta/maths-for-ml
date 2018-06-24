# Variance and Covariance

- Describing the concentration of points around the mean is called _variance_
- It is used to characterize the spread of data points in a dataset
$$\text{for } X=[x_1,x_2...x_n]$$
$$Var[X]=\sum_{i=1}^{n}\frac{x_i-\bar{x}}{n}$$

## Variance for high dimensional spaces

- Use covariance to describe the relation between two variablex $X$ and $Y$

$$cov[X,Y]=E[(x-\mu_x)(y-\mu_y)]$$
$$\mu_x=E[X]$$
$$\mu_y=E[Y]$$

- We get the terms
$$cov[X, Y]$$
$$var[X]$$
$$cov[Y, X]$$
$$var[Y]$$

- Hence, the covariance matrix is expressed as

$$\begin{bmatrix}var[X]&cov[X,Y]\\cov[Y,X]&var[Y]\end{bmatrix}$$

- For $D$ dimensional dataset, we can compute variance as

$$D = {x_1,x_2..x_n}, X\epsilon {\rm I\!R}$$

$$var[D]=\frac{1}{N}(x_i-\mu)(x_i-\mu)^T$$

- This is called the _covariance_ of a dataset. It will be a $DxD$ matrix



