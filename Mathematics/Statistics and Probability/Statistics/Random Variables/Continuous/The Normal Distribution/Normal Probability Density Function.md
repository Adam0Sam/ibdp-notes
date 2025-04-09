If $X$ is a **normally** distributed random variable with a mean $\mu$ and a standard deviation $\sigma$, then $\mu$ and $\sigma$ are parameters of the variable's normal distribution $X \sim \mathrm{N}(\mu,\sigma^{2})$ 

For $X$ to be normally distributed, its [[Probability Density Functions|probability density function]] must have the form $\forall x \in \mathbb{R}$
$$
f(x)=\frac{1}{\sigma \sqrt{ 2\pi }}e^{ -\frac{1}{2}\left( \frac{x-\mu}{\sigma} \right)^{2}}
$$

> [!Tip] Properties of the normal curve
> - The curve is symmetrical around $x=\mu$ (i.e. $f(x+a)=f(x-a) \quad \forall a \in \mathbb{R}$)
> - $f(x)>0 \quad\forall x \in \mathbb{R}$
> - The $x$-axis is a horizontal asymptote
> - $\max(f(x))=f(\mu)$
> - The points of inflection occur at $x\pm \mu$ (so it can be interpreted that $\sigma$ of $f(x)$ is the horizontal distance from $\mu$ to a point of inflection)

> [!example] Normal Probability Distribution
> - $68\%$ in the $(\mu-\sigma, \mu+\sigma)$
> - $95\%$ in the $(\mu-2\sigma, \mu+2\sigma)$
> - $99.7\%$ in the $(\mu-3\sigma, \mu+3\sigma)$
> 
>![[Pasted image 20250107175415.png]]


> [!info] [[The Standard Normal Distribution]]
> Any normal distribution can be transformed using the [[The z-score|Z-transformation]] to produce [[The Standard Normal Distribution]] $\mathrm{N}(0,1^{2})$

