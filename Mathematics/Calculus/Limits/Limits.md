If $f(x)$ is as close as we like to some real number $A$ for all $x$ sufficiently close (*but not equal to*) $a$, then we say that $f(x)$ has a **limit** of $A$ as $x$ approaches $a$, and we write $$\lim_{x\to a} = A$$
More formally, 
$$
\begin{align}
\text{The limit } \lim_{x\to a}f(x) \text{ exists and is equal to the finite value } A \\ \text{ if } \lim_{x\to a^-}f(x)=\lim_{x\to a^+}f(x) = A.
\end{align}
$$
The above expression uses the concept of [[Function Continuity|continuity]] to describe a curve

> [!Tip] Finding a limit
> The function $f$ doesn't necessarily need to be defined at $a$, the limit simply describes the functions behaviour as $x\to a$ 
> 
> Consider $f(x)=\frac{5x+x^2}{x}$
> ![[Pasted image 20240409102819.png]]
> Even though a **point of discontinuity** exists at $(0,5)$, as $x\to0$ from both directions, $f(x)\to 5$

[[Limit Laws]] simplify the process of solving limits

> [!Info] Limits at Infinity
> $$\lim_{x\to \infty}\frac{1}{x^n}=0 \text{ for all } n>0$$

> [!Tip] The Sin-Radian limit
> #todo proof
> $$\text{If }\theta \text{ is in radians, then } \lim_{\theta\to 0}\frac{\sin\theta}{\theta}=1$$
> This is an example of a limit in [[Indeterminate Limit Forms|indeterminate form]].
> 
> This particular limit lays the foundation of evaluating the [[Differential Calculus|derivatives]] of [[trigonometric functions]] and also the basis for [[l'Hopital's rule]], which seeks to generalize the values of other [[Indeterminate Limit Forms|indeterminate limits]]
