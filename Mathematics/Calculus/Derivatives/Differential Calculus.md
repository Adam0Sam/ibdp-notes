A derivative is an expression representing the *[[rate of change]]* of a [[Functions|function]] with respect to an independent variable

For two points $A(a, f(a))$ and $B(a+h, f(a+h))$ on a function, the chord of $AB$ is $\frac{f(a+h)-f(a)}{h}$

As $h\to 0$, $a+h\to a$, thus the **gradient of the tangent** to the curve $y=f(x)$ at the point where $x=a$ is $$\lim_{h\to 0}\frac{f(a+h)-f(a)}{h}$$
$f'(x)$ is defined as the derivative function whose outputs matches the values of the gradient of the tangent to the curve $y=f(x)$

> [!Tip] Leibniz Notation
> If we are given a function $f(x)$ then $f'(x)$ represents the derivative function
> 
> However, if we are given $y$ in terms of $x$, then we use the *Leibniz notation* $\frac{\mathrm{d}x}{\mathrm{d}y}$ to represent the derivative.
> 
> Important to note that $\frac{\mathrm{d}x}{\mathrm{d}y}$ is not a fraction, but the result of taking the limit of a fraction. 
>5t
  
$f'(x)$ unlocks the concept of **[[Function Differentiability|differentiability]]** 

> [!Tip] The process of differentiation need not be conducted from the limit definition
> Instead, utilize [[Rules of Differentiation]]
> 
> Relationships can also be differentiated using [[Implicit Differentiation]]


> [!Info] Higher Order Derivatives
> The $n$th derivative of $f(x)$ is obtained by differentiating $y=f(x)$ $n$ times
>$$
f^{(n)}(x) \quad \text{ or } \quad \frac{\mathrm{d}^ny}{\mathrm{d}x^n}
>$$

Equations involving derivatives are called [[differential equations]]