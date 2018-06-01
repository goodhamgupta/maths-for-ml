# Non-linear regression

- For a function $y$ with parameters $a_k$

$$y(x_i, a_k)=(x-a_1)^2+a_2$$
$$\text{for $x_i$ and $y_i$}$$
- We have an associated uncertanity for each $y_i$ denoted by $\sigma_i$ i.e more uncertain we are about the data point, the greater the value of $\sigma_i$ will be
- Hence, the error function $\chi^2$ will be

$$\chi^2=\frac{\sum_{i=1}^{n}[y_i-y(x_i, a_k)]^2}{\sigma^2}$$

- Here, we are penalizaing uncertain data points by a factor of $\sigma^2$ so that these points have a low weight in the sum(and so that they don't affect the fit too much).
- Minimum of $\chi^2$ will be when

$$\nabla \chi^2=0$$
$$a_{next}=a_{cur}-constant*\nabla \chi^2$$

- Here, the constant specifies how fast/slow we want to go down the hill(aka learning rate)

$$\frac{\partial \chi^2}{\partial a_k}=\text{calculate this}$$

- We can use the Jacobian to perform steepest gradient descent effectively
- 