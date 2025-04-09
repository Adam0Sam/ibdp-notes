> [!example] The Taylor Series
>$$
>f(x)=\sum_{k=0}^{\infty} \frac{f^{(k)}(a)}{k!}(x-a)^k
>$$

the Maclaurin series is a special case of the Taylor Series where $a=0$, thus the Maclaurin series is defined as
$$
f(x)=\sum_{k=1}^{\infty} \frac{f^{f(k)}(0)}{k!}x^k
$$
> [!tip] the $n$-th degree approximation
>$$
>M_{n}(x)=\sum_{k=1}^{n} \frac{f^{(k)}(0)}{k!}x^k
>$$
>$M_{n}(x)$ might also be called the $n$-th order polynomial of best fit. Since $M_{n}(x)$ is generated using $f$ and its derivatives at $x=0$, $M_{n}(x)$ will generally be most accurate near to $x=0$. 
>
>> [!warning] Asymptotes
>> It is not possible for any polynomial approximation to model a vertical asymptote
>
> Notice that $M_{n}(x)$ may explode, disabling approximation. 
>$$
>\text{For } \lim_{ n \to \infty } M_{n}(x)=f(x) \ \text{to hold}, \ x \in \text{interval of convergence}
>$$


[[Maclaurin Series of Functions]]

> [!tip] Composite Functions
> It is unnecessary to derive a series for each function, since composition can be used
> > [!example]
> > $$\frac{1}{1-x}=\sum_{k=1}^{\infty} x^{k} \Rightarrow \frac{1}{1-x^{2}}=\sum_{k=1}^{\infty} x^{2k}$$

Since $M_{n}(x)$ is, fundamentally, a simple [[Polynomials|polynomial]] the same mathematical operations of addition, subtraction, multiplication, division, [[Differential Calculus|differentiation]] and [[Integral Calculus|integration]] similarly apply to $M_{n}(x)$ (the latter of which are especially useful for differentiating/integrating functions which generally don't have elementary integrals)

> [!info] Division
> To perform the division of two Maclaurin series $f(x)$ $g(x)$ we assume the result is another Maclaurin series $$p(x)=\frac{f(x)}{g(x)}=\sum_{k=0}^{\infty}a_{k}x^k $$

