If $f(x)=\sin x, \quad -\frac{\pi}{2}\le x \le \frac{\pi}{2}$, then $f^{-1}(x)=\arcsin x$

With this, consider the following differentiation of $y=\arcsin x$
$$
\begin{align}
&\text{Mark the inverse function } x=\sin y \\
&\therefore \frac{\mathrm{d}x}{\mathrm{d}y} =\cos y = \sqrt{ 1-\sin^2y }=\sqrt{ 1-x^2 }   \\
 \\
&\text{From the chain rule}, \frac{\mathrm{d}y}{\mathrm{d}x}\frac{\mathrm{d}x}{\mathrm{d}y} = \frac{\mathrm{d}y}{\mathrm{d}y} = 1, \\
& \frac{\mathrm{d}y}{\mathrm{d}x} \text{ and }\frac{\mathrm{d}x}{\mathrm{d}y} \text{ are reciprocals}
 \\ &\therefore \frac{\mathrm{d}y}{\mathrm{d}x} = \frac{1}{\sqrt{ 1 - x^2 }}, \quad \text{if } -1<x<1
\end{align}
$$
The same logic is followed for $\arccos x$ and $\arctan x$
$$
\begin{align}
&\frac{\mathrm{d}}{\mathrm{d}x}\arccos x = -\frac{1}{\sqrt{ 1-x^2 }}, \quad -1<x<1 \\ \\
&\frac{\mathrm{d}}{\mathrm{d}x}\arctan x=\frac{1}{1+x^2}, \quad x \in \mathbb{R}
\end{align}
$$


Extending these functions to also include composite functions as parameters, we get similar derivatives as with [[Trigonometric Function Derivatives]]

$$
\begin{align}
& \frac{\mathrm{d}}{\mathrm{d}x}\arcsin(f(x)) = \frac{f'(x)}{\sqrt{ 1-x^2 }} \\ \\
& \frac{\mathrm{d}}{\mathrm{d}x}\arccos(f(x)) = -\frac{f'(x)}{\sqrt{ 1-x^2 }} \\ \\
& \frac{\mathrm{d}}{\mathrm{d}x}\arctan(f(x)) = \frac{f'(x)}{1+x^2} \\

\end{align}
$$