The method of **integration by substitution** comes from the [[The Chain Rule]] of differentiation

$$
\text{Integrals in the form } \int f(u)\frac{du}{dx}  \, dx  \ \text{ can be rewritten to } \int f(u) \, du 
$$

### Explanation

Suppose $F(u)$ is the antiderivative of $f(u)$ such that $\frac{dF}{du}=f(u)$ 
$$
\therefore \int f(u) \, du =F(u)+c
$$
but $\frac{dF}{dx}=\frac{dF}{du}\cdot \frac{du}{dx}$
$$
\therefore \int f(u)\cdot \frac{du}{dx}  \, dx = F(u)+c
$$

> [!example] Using this method
> 
>$$
\begin{align}
\int (x^{2}+3x)^{4}(2x+3) \, dx &= \int u^{4}\frac{du}{dx}  \, dx  \\
&=\int u^{4} \, du  \\
&= \frac{u^{5}}{5}+c  \\
&= \frac{1}{5}(x^{2}+3x)^{5}+c
\end{align}
$$

