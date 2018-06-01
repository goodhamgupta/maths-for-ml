# Lagrange Multipliers

## Constrianed optimization

- This is used to find the minina/maxima subject to some constraint. These contraints are called lagrange multipliers
- For eg,

$$\text{maximize} f(x,y)=x^2y$$
$$\text{constraint} g(x,y)=x^2+y^2=a^2$$

- The above equation requires us the find the maximum value of the gradient in the circle specified by $g(x)$
$$\nabla f=\lambda \nabla g$$
- $\lambda$ is the lagrange multiplier
$$\nabla f=\begin{bmatrix}2xy\\x^2\end{bmatrix}$$
$$\lambda \nabla g=\lambda \begin{bmatrix}2x\\2y\end{bmatrix}$$
- Solving these equations, we get

$$2xy=\lambda 2x $$
$$=> y=\lambda$$
- Similarly
$$x^2=\lambda 2y $$
$$x^2=2y^2$$
$$x=\sqrt{2}y$$
- Further,

$$x^2+y^2=a^2$$
$$2y^2+y^2=a^2$$
$$y=\pm\frac{a}{\sqrt{3}}$$

- Hence, we have the following solutions for $y=1$
$$\frac{a}{\sqrt{}3}\begin{bmatrix}\sqrt{2}\\1\end{bmatrix},\frac{a}{\sqrt{}3}\begin{bmatrix}\sqrt{2}\\-1\end{bmatrix},
\frac{a}{\sqrt{}3}\begin{bmatrix}-\sqrt{2}\\1\end{bmatrix},
\frac{a}{\sqrt{}3}\begin{bmatrix}-\sqrt{2}\\-1\end{bmatrix}$$

- Hence, the value of $f(x,y)$ will be

$$$$
