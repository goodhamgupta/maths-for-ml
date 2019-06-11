# Approximations

## Taylor Series

- Approximate a complex function using a series of simple functions
- Also called _power series_ as it is expressed as they are expressed as coefficients in front of increasing powers of x
$$g(x) = a+bx+cx^2...$$

- $g_1$ will be called the first order series
$$g_0=a$$
$$g_1=a+bx$$
$$g_2=a+bx+cx^2$$
- Collectively, these series are called _Truncated Series_

## Power series derivation

- This works only for functions that are _well behaved_ i.e functions which are continous and can be diffferentiated as many times as needed
- At each level of differentiation, express the coefficients($a,b,etc$) as a result of the derivation. This will help approximate it
- See [this](https://www.coursera.org/learn/multivariate-calculus-machine-learning/lecture/C6x2C/power-series-derivation) video
- This series is called _MacLaurin series_

$$e^x=\sum_{n=0}^{\infty}\frac{f^{(n)}(0)}{n!}x^n$$
- It states that if we know everything about a function at a particular point, we can find out everything about the function at EVERY POINT
- *Taylor series* =>Extension of MacLaurin series. It states that if we know everything about the function at any point, then we can reconstruct the function anywhere.
- For eg

$$e^x=1+x+\frac{x^2}{2}+\frac{x^3}{6}...$$
$$=> e^x=\sum_{x=0}^{\infty}\frac{x^n}{n!}$$

- Instead of expanding at point $x=0$, we will try to approximate the function at a arbitary point $p$
- The first approximation will be a line through the point p i.e $f(p)$
- For the second approximation, it will be a tangent to the curve at point $p$. It will be expressed as a line
$$y=mx+c$$
- We know the gradient at point $p$ is m. It can be expressed as $f'(p)$. Hence,
$$y=f'(p)x+c$$
- To find the value of $c$, we need the values of $y$ and $x$. We already know the point $(p, f(p))$. Hence we get,
$$f(p)=f'(p)p+c$$
$$=> c=f(p)-f'(p)p$$
- Therefore,
$$y=f'(p)x+f(p)-f'(p)p$$
$$y=f(p)+f'(p)(x-p)$$

- When using the term $f'(p)$, rather than using the term around point $x$, we will apply it at point $x-p$ i.e how far are we away from $p$
- Therefore, we get

$$g_0(x)=f(p)$$
$$g_1(x)=f(p)+f'(p)(x-p)$$
- Hence, the Taylor series can be expressed as

$$g(x)=\sum_{n=0}^{\infty}\frac{f^{(n)}(p)}{n!}(x-p)^n$$
- 
