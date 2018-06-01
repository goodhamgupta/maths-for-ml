# Gradient Descent

- Method used to find the fastest/steepest way to get down the graph and find your roots(i.e place where the value of your function is minimum)
- For the function

$$f(x,y)=x^2y$$
$$\frac{\partial f}{\partial x}=2xy$$
$$\frac{\partial f}{\partial y}=x^2$$

- We can write these terms in a vector i.e 

$$\nabla f=\begin{bmatrix}\frac{\partial f}{\partial x}\\\frac{\partial f}{\partial y}\end{bmatrix}$$
$$=\begin{bmatrix}2xy\\x^2\end{bmatrix}$$

- When we multiply this with a vector $\vec r$ say, we get

$$\nabla f. \vec r$$
$$\begin{bmatrix}\frac{\partial f}{\partial x}\\\frac{\partial f}{\partial y}\end{bmatrix}.\begin{bmatrix}dx\\0\end{bmatrix}$$
$$=dx*\frac{\partial f}{\partial x}$$

- This shows that we take a small step $dx$ along the x-axis of the vector
- Using this, we can estimate how much the function will change when we move along a direction
- $\nabla f . \vec r$ is called the _directional gradient_


## Max value of directional gradient

- We want the max value because at every iteration we want to take the largest step towards in maxima/minima value
- Suppose $\vec r$ is $\begin{bmatrix}c\\d\end{bmatrix}$. Dot product of $\nabla f$ with $\vec r$ will be

$$\nabla f . \vec r$$
$$=|\nabla f||\vec r|cos(\theta)$$

- The above equation will have maximum value when value of $cos(\theta)$ is highest i.e $cos(\theta)=1 => \theta = 0$
- Hence, $\nabla f$ should be parallel to $\vec r$
- Therefore, we want $\vec r$ that is the normalized version of $\nabla f$
- Hence, the dot product will become

$$\nabla f . \frac{\nabla f}{||\nabla f||}$$
- Since dot product of $\nabla f$ with itself will be $||\nabla f||^2$, we get

$$\frac{||\nabla f||^2}{||\nabla f||}$$
$$=||\nabla f||$$

- Hence, the steepest gradient we can possibly have is just the size of the $\nabla f$ vector

## Which way does $\nabla f$ point?

- It points up the direction of the steepest slope. Hence, if we want to find the lowest point(or minimize the function) we go in direction opposite to the gradient i.e $- \nabla f$
- In gradient descent method, when we are trying to minimize a function, we take small steps in the direction of the gradient. Hence

$$S_{n+1}=S_n-\lambda \nabla f$$

- Here, $\lambda$ specifies the small step that we take i.e the learning rate
- There can be multiple local minima in the function and we can get stuck in them using this method. The minima we find will depend on the starting step. There are other gradient descent techniques to combat this


