Differential equations of the form $\frac{dy}{dx}=f\left( \frac{x}{y} \right)$, where $y=y(x)$ are known as **homogenous differential equations**.

They can be solved using the substitution $y=vx$ where $v$ is a function of $x$.

> [!example] For example, if $y=vx$ where $v$ is a function of $x$
>$$
\begin{align}
&\frac{dy}{dx} = \frac{dv}{dx} x+v \\
&\therefore \frac{dv}{dx}  x+v=f\left( \frac{vx}{x} \right)=f(v) \\
&\therefore \frac{dv}{dx} = \frac{f(v)-v}{x} \\
&\therefore \frac{1}{f(v)-v}\frac{dv}{dx}  = \frac{1}{x}, \quad \text{which is a seperable differential equation}
\end{align}
>$$
