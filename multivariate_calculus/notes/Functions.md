# Functions

- Relationship between input and output

$$f(x) = x2+3$$

- Select a function which represents a graph/dataset
- Calculus is the study of how these function change with respect to their input variables and allows to investigate and manipulate them

## Gradients

- Tangent at a point on a graph will give the rate of change of the function at that point. This rate of change is called gradient.
- Derivate at a particular point is called _local gradient_
- The gradient is not defined at points which are not smooth(eg: lowest point of the symbol 'V')
- Shifting a function up/down does not change the gradient
- If one function is a vertical shift of another function, they MAY have the same 

## Derivative

- _Rise_ => Increase in the vertical direction
- _Run_ => Distance along the horizontal axis
$$gradient=\frac{rise}{run}$$
- For calculating the gradient of more complex function, we will do the following
  - Choose a point on the function. Draw a line down to the x-axis. This point will be called $x$
  - Hence, the $y$ coordinate will be $f(x)$
  - For drawing our rise over run traingle, we need another point
  - Select a point which is $\Delta{x}$ away from our point $x$. $\Delta{x}$ represents the horizontal distance between $x$ and our new point. Used to express a small change in something
  - Hence, location of new point will be $x+\Delta{x}$.
  - The $y$ value at this point will be $f(x+\Delta{x})$.
$$gradient \approx \frac{rise}{run}=\frac{f(x+\Delta{x})-f(x)}{\Delta{x}}$$
  - As $\Delta{x}$ becomes smaller, the gradient at that point will become more accurate
  - In limit terms,

$$\frac{df}{dx}=f\prime(x) = \lim_{\Delta{x}->0} \frac{f(x+\Delta{x})-f(x)}{\Delta{x}}$$

### Sum rule
$$\frac{d}{dx}(f(x)+g(x)) = \frac{d}{dx}f(x)+\frac{d}{dx}g(x)$$
### Power rule
$$\frac{d}{dx}ab^{x}=xab^{x-1}$$

## Special derivatives

$$\frac{d}{dx}\bigg(\frac{1}{x}\bigg) = -\frac{1}{x^2}$$
$$\frac{d}{dx}e^x = e^x$$
$$\frac{d}{dx}\sin{x}=\cos{x}$$
$$\frac{d}{dx}\cos{x}=-\sin{x}$$
$$\frac{d}{dx}-\sin{x}=-\cos{x}$$
$$\frac{d}{dx}-\cos{x}=sin{x}$$

- We can see that in the case of trignometric function, there is a pattern. We return to the original function after every _4th_ derivative

## Product Rule

$$\frac{d}{dx}\bigg(f(x)g(x)\bigg)=f(x)g'(x)+f'(x)g(x)$$

## Chain Rule

$$\frac{dh}{dm}=\frac{dh}{dp}*\frac{dp}{dm}$$