# Jacobian

- Represents a vector where each entry is a partial derivative of the function $f(x_1,x_2,x_3..x_n)$ with respect to each of the variables in trun
- This is a ROW vector
- It represents a vector pointing in the direction of the steepest slope for a function
- Jacobian describes the gradient of a multivariate system
- Overall, it determines the direction and the magnitude of the gradient
$$f(x,y,z)=x^2y+3z$$
$$J = [2xy, x^2, 3]$$
$$J(0,0,0)=[0,0,3]$$

- Contour plot => Draw a map with lines around the regions that have the same height
- Largest jacobian vectors are found in areas where the contour lines are tightly packed


## Sandpit

- Optimization: Process of making something/a value as good as it can be
- Tallest Peaks of a contour plot are called maxima
- Deepest troughs of a contour plot are called minima