An integral is described as improper if one of the following is true:
1. The function being integrated approaches $\infty$ or $-\infty$ for one or more points on the domain of integration
   
   For example, $\int_{-1}^{2} \frac{1}{x^{2}}  \, dx$ is improper since $\frac{1}{x^{2}}$ is discontinuous at $x=0$. As $x \rightarrow 0$, $f(x)\rightarrow \infty$

2. The integral has the form $\int_{a}^{\infty} f(x) \, dx$, $\int_{-\infty}^{b} f(x) \, dx$, or $\int_{-\infty}^{\infty} f(x) \, dx$, where $a,b \in \mathbb{R}$


Provided the limit exists and that as $x \rightarrow \infty$, $f(x)\rightarrow 0$, one of the improper integrals can defined as follows

$$
\int_{a}^{\infty} f(x) \, dx = \lim_{ b \to \infty } \int_{a}^{b} f(x) \, dx 
$$
