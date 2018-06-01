# Linear Regression

- The equation for linear regression with a single variable is 

$$y=mx+c$$

- To measure the goodness of fit, we need a error function to minimize. Let's say for given values of $m$ and $c$ the prediction vector is $\hat{y}$

## Least Squares

- Error function used to measure the goodness of fit of a line.

$$\chi=\sum_{i=1}^{n}(y-\hat{y})^2$$

- To minimize this function, we can use the gradient of $\chi2$

$$\nabla \chi=\begin{bmatrix}\frac{\partial \chi}{\partial m}\\\frac{\partial \chi}{\partial c}\end{bmatrix}$$

- Solving this, we get
$$m=\frac{\sum_{i=1}^{n}(x_i-\bar{x})y_i}{\sum_{i=1}^n(x-\bar x)^2}$$
$$c=\bar{y}-m\bar{x}$$

