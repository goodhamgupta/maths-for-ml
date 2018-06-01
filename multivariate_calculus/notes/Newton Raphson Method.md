# Newton Raphson Method

- Method to find derivative/gradient 
- For the eq

$$y=x^3-2x+2$$

$$\frac{\partial f}{\partial x}=3x^2-2$$

- The derivative will have two solutions. Hence, there will be two points that exist(one at the maxima and one at the minima)

- If we don't know what the equation looks like or do not have the resources the visualize the equation at every point (because it has many dimensions) and we only need to find the solutions to the equation at $y=0$($x^3-2x+2=0$). We can see that it already has one solution but there could be more if the equation was different
- If we are trying to estimate the root of the equation from an initial guess value, we first
  - Evaluate the function at this guess value
  - Evaluate the gradient at this value. Extrapolate the gradient to intersect at the x-axis.
  - Take the intersect as the new value of the guess. Continue the process 
- Expression for newton method

$$f(x_{i+1}=f(x_i)-\frac{f(x_i)}{f'(x_i)}$$

## Edge cases

- Sometimes, if the initial guess value is incorrect, we will get a loop of guess values after using the newton raphson equation. Because of this the equation will not converge.
- If we are at a maxima/minima, the gradient at this point will be small. Hence, our next estimate will be huge. 