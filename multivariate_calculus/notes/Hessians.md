# Hessians

- Extension of jacobian vector
- Collect all 2nd order derivates of a func $f$ into a matrix
$$\boldsymbol{H}=\begin{bmatrix}\frac{\partial^2{f}}{\partial{x_1^2}}&\frac{\partial^2{f}}{\partial{x_1x_2}}...&\frac{\partial^2{f}}{\partial{x_1x_n}}\\\frac{\partial^2{f}}{\partial{x_2x_1}}&\frac{\partial^2{f}}{\partial{x_2^2}}...&\frac{\partial^2{f}}{\partial{x_2x_n}}\\\frac{\partial^2{f}}{\partial{x_nx_1}}&\frac{\partial^2{f}}{\partial{x_nx_2}}...&\frac{\partial^2{f}}{\partial{x_n^2}}\end{bmatrix}$$
- It will be an $nxn$ square matrix, where $n$ is the number of variables

## Properties

- If $\det({\boldsymbol{H}})$ is positive, we know it is either a maximum or a minimum
- If first term in top left column i.e $\boldsymbol{H}[0,0]$ is ALSO positive, then it is a MINIMUM. If negative, then it is a MAXIMUM
- If $\det({\boldsymbol{H}})$ is negative, so it is not a maximum or a minimum. BUT, at point $(0,0)$, the gradient is flat i.e the slopes are coming down towards it in one direction and up towards it in the other direction(minute 5:08 [here](https://www.coursera.org/learn/multivariate-calculus-machine-learning/lecture/hyqnv/the-hessian)). This point is called a SADDLE POINT
- The column vectors in the Hessian are essentially the eigen vectors