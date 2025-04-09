 
notice that $\frac{d}{dx} (e^{ax+b})=ae^{ax+b}$
$$
\therefore \int e^{ax+b} \, dx =\frac{1}{a}e^{ax+b}+c
$$

likewise if $n\ne 1$ , $\frac{d}{dx}((ax+b)^{n+1})=a(n+1)(ax+b)^{n}$

$$
\therefore \int (ax+b)^{n} \, dx =\frac{1}{a} \frac{(ax+b)^{n+1}}{n+1} + c \quad \text{for } n\ne -1, a\ne 0
$$
In a similar manner it follows that for $a\ne 0$
$$
\begin{align}
 & \int \cos(ax+b) \, dx = \frac{1}{a}\sin(ax+b)+c \\
 & \int -\sin(ax+b) \, dx =\frac{1}{a}\cos(ax+b)+c \\
& \int \sec ^{2}(ax+b) \, dx = \frac{1}{a}\tan(ax+b)+c
\end{align}
$$
Finally, $\frac{d}{dx}\left( \frac{1}{a}\ln(ax+b) \right)=\frac{1}{a} \frac{a}{ax+b}=\frac{1}{ax+b}$ (same goes for $\frac{d}{dx}\left( \frac{1}{a} \ln(-(ax+b))\right)$)
$$
\therefore \int \frac{1}{ax+b} \, dx = \frac{1}{a}\ln|ax+b|+c
$$

### Aditionally

When a constant $a^{2}$ replaces the $1$ in the following expressions
$$
\begin{align}
&\int \frac{a}{x^{2}+a^{2}} \, dx =\arctan\left( \frac{x}{a} \right)+c \\
&\int \frac{1}{\sqrt{ a^{2}-x^{2} }} \, dx = \arcsin \left( \frac{x}{a} \right)+c \\
&\int -\frac{1}{\sqrt{ a^{2}-x^{2} }} \, dx =\arccos\left( \frac{x}{a} \right)+c
\end{align}
$$


