# Multivariate Chain Rule

- Total derivate of $f(x,y,z)$ where $x,y,z$ are function of a variable $t$ 

$$\frac{\partial f}{\partial t} = \frac{\partial f}{\partial x}*\frac{\partial x}{\partial t}+\frac{\partial f}{\partial y}*\frac{\partial y}{\partial t}+\frac{\partial f}{\partial z}*\frac{\partial z}{\partial t}$$

- We can represent $f(x_1,x_2,..,x_n)=f(\boldsymbol{x})$
- Therefore,

$$\frac{\partial f}{\partial \boldsymbol{x}} = \begin{bmatrix}\frac{\partial f}{\partial x_1}\\\frac{\partial f}{\partial x_2}\\.\\.\\\frac{\partial f}{\partial x_n}\end{bmatrix}$$
$$\frac{\partial \boldsymbol{x}}{\partial t}=\begin{bmatrix}\frac{\partial x_1}{\partial t}\\\frac{\partial x_2}{\partial t}\\.\\.\\\frac{\partial x_n}{\partial t}\end{bmatrix}$$
Hence, we get
$$\frac{\partial f}{\partial t} = \frac{\partial f}{\partial \boldsymbol{x}}.\frac{\partial \boldsymbol{x}}{\partial t}$$

- Here, $\frac{\partial f}{\partial \boldsymbol{x}}$ is the Jacobian vector by it is written as a column vector 
- Hence

$$\frac{\partial f}{\partial \boldsymbol{x}} = (\boldsymbol{J}_f)^T$$
- Dot product of two column vectors = Multiplying row vector with column vector
$$\frac{\partial f}{\partial t} = \boldsymbol{J}_f*\frac{\partial \boldsymbol{x}}{\partial t}$$

- Same chain rules works for multivariate function with variables which are vectors

$$\frac{\partial f}{\partial t} = \frac{\partial f}{dx}*\frac{\partial \boldsymbol{x}}{\partial \boldsymbol{u}}*\frac{\partial \boldsymbol{u}}{\partial t}$$
$$\frac{\partial f}{\partial t} = \bigg[\frac{\partial f}{\partial x_1},\frac{\partial f}{\partial x_2} \bigg]\begin{bmatrix}\frac{\partial x_1}{\partial u_1}&\frac{\partial x_2}{\partial u_2}\\\frac{\partial x_2}{\partial u_1}&\frac{\partial x_2}{\partial u_1}\end{bmatrix}\bigg[\frac{\partial \boldsymbol{u}}{\partial t}\bigg]$$

- Once we solve the equation above, we will get a scalar as expected(watch video [here](https://www.coursera.org/learn/multivariate-calculus-machine-learning/lecture/Ht9dM/more-multivariate-chain-rule))
