# Multivariate Taylor Series

- Power series can be expressed in it's multivariate form
- Notational options

$$f(x)=\sum_{n=0}^{\infty}\frac{f^{n}p}{n!}(x-p)^n$$
$$f(x+\Delta x)=\sum_{n=0}^{\infty}\frac{f^{n}x}{n!}(\Delta x)^n$$

- For a two dimensional case, we will have

$$f(x+\Delta x, y + \Delta y)=?$$

$$f(x)=e^{-{x^2+y^2}}$$
For the above function, we have
- The zeroth order approximation for the above function will a plane surface passing through the point
- The first order approximation should have a height and a gradient. Hence, the straight surface will be at an angle
  - At the peak, the gradient is 0. Hence it would be a normal straight surface
  - At any other point, we would get a plane with the same height and gradient at the point
- The second order approximation will be some kind of a parabolic surface
  - At the peak, the parabola will be INSIDE the bell curve
  - At a point on the side of the bell curve(i.e the function $f(x)$), we would get a parabola with a saddle point. The gradient and the curvature will match up at this point. HOWEVER, this is not a very useful approximation as it matches only at that given point
## General expression
- The first order approximation will be

$f(x+\Delta x, y+ \Delta y)=f(x,y)+\partial_xf(x,y)\Delta x+\partial_yf(x,y)\Delta y$
- The second order approxmation will consist of double derivatives
$f(x+\Delta x, y+ \Delta y)=f(x,y)+\partial_xf(x,y)\Delta x+\partial_yf(x,y)\Delta y+\frac{1}{2}\big(\partial_{xx}f(x,y)\Delta x^2+\partial_{xy}f(x,y)\Delta x \Delta y+\partial_{yy}f(x,y)\Delta y^2\big)$

- First order approximation can be expressed in terms of the Jacobian(which consists of first derivatives) as

$$f(x+\Delta x,y+\Delta y)=[\partial_xf(x,y), \partial_yf(x,y)]\begin{bmatrix}\Delta x\\\Delta y\end{bmatrix}$$
$$=J_f\boldsymbol{\Delta x}$$

- Similary, the second order terms contains double derivatives. Hence, it can be expressed in terms of the _Hessian_ as follows

$$\frac{1}{2}\big(\partial_{xx}f(x,y)\Delta x^2+\partial_{xy}f(x,y)\Delta x \Delta y+\partial_{yy}f(x,y)\Delta y^2\big)$$
$$=\frac{1}{2}[\Delta x, \Delta y]\begin{bmatrix}\partial_{xx}f(x,y)&\partial_{xy}f(x,y)\\\partial_{yx}f(x,y)&\partial_{yy}f(x,y)\end{bmatrix}\begin{bmatrix}\Delta x\\\Delta y\end{bmatrix}$$
$$=\frac{1}{2}\boldsymbol{\Delta x}^TH_f\boldsymbol{\Delta x}$$

- Hence, our final compact expression for multivariate taylor series expansion is

$$f(x+\Delta x, y+\Delta y)=f(x)+J_f\boldsymbol{\Delta x}+\frac{1}{2}\boldsymbol{\Delta x}^TH_f\boldsymbol{\Delta x}...$$

- This expression can be extended to include any number of dimensions

  