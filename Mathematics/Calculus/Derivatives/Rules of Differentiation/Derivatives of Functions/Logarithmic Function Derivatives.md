$$
\text{If } y=\ln x \quad \text{then } \frac{\mathrm{d}y}{\mathrm{d}x}=\frac{1}{x},\ x > 0
$$
( #todo proof with implicit differentiation)
#todo proof with limit definition



#### General form of $\frac{\mathrm{d}}{\mathrm{d}x}\ln(f(x))$
$$
\text{If } y=\ln(f(x))=\ln u
$$
Using [[the chain rule]]
$$
\begin{align}
\frac{\mathrm{d}y}{\mathrm{d}x} &= \frac{\mathrm{d}y}{\mathrm{d}u} \cdot \frac{\mathrm{d}u}{\mathrm{d}x}  \\
&= \frac{1}{u}\cdot\frac{\mathrm{d}u}{\mathrm{d}x} \\
&= \frac{f'(x)}{f(x)}
\end{align}
$$

#### General form of $\frac{\mathrm{d}}{\mathrm{d}x}\log_{a}f(x)$
$$
\text{If } y=\log_{a}(f(x))=\log_{a}u = \frac{\ln u}{\ln a}
$$
Using [[the chain rule]]

$$
\begin{align}
\frac{\mathrm{d}y}{\mathrm{d}x} &= \frac{\mathrm{d}y}{\mathrm{d}u} \cdot \frac{\mathrm{d}u}{\mathrm{d}x}  \\
&= \frac{1}{u\ln a}\cdot\frac{\mathrm{d}u}{\mathrm{d}x} \\
&= \frac{f'(x)}{f(x)\ln a}
\end{align}
$$
