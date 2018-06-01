# Linearisation

- Helps estimate the error in our approximations
- We know
$$g(x)=\sum_{n=0}^{\infty}\frac{f^{(n)}p}{n!}(x-p)^n$$
- When we use the first order approximation, we get

$$g_1(x)=f(p)+f'(p)(x-p)$$

- This expression imples that => Starting from the height $f(p)$, as we move away from p, the corresponding change in height is equal to distance away from $p$ times the gradient at $p$. Using the gradient formula, we get

$$rise=gradient*run$$
$$rise=f'(p)*(x-p)$$

- Lets call our distance $x-p$ as $\Delta p$ which represents a small step size away from $p$
- Hence, $x=p+\Delta p$
- Therefore, we can rewrite our expression as
$$g_1(p+\Delta p)=f(p)+f'(p)\Delta p$$
- We can swap all $p$ terms with $x$ 
$$g_1(x+\Delta x)=f(x)+f'(x)\Delta x$$
- Hence, the taylor series can now be expressed as

$$f(x+\Delta x)=\sum_{n=0}^{\infty}\frac{f^{(n)}x}{n!}\Delta x^n$$

- We know the above expression can help us represent any equation as a sum of the infinitely long series. What if we want to find the error in our approximation?
- Expanding the expression, we get
$$f(x+\Delta x)=f^{0}x+f^{1}x\Delta x+\frac{f^2x}{2}\Delta x^2...$$
- If $\Delta x$ is a small number, $\Delta x^2$ will be an even smaller number, $\Delta x^3$ will be further smaller
- Hence, we can include the order of the $\Delta x$ term in our first approximation i.e _on the order of $\Delta x^2$_
- Second order accurate => First order taylor series

$$f(x+\Delta x)=f(x)+f'(x)(\Delta x)+O(\Delta x^2)$$

- This process of taking a function and ignoring the terms above $\Delta x$ is called *Linearisation*
- After a bunch of equations and derivations, we get

$$f'(x)=\frac{f(x+\Delta x)-f(x)}{\Delta x}+O(\Delta x)$$


