> [!Example]
> - [[#Multiplication]]
> - [[#Division]]
> - [[#Raising to a power]]


## Multiplication
One can easily multiply complex numbers in [[Forms of Complex Numbers|polar form]]$e^{\theta_1 i} \cdot e^{\theta_2 i} = e^{(\theta_1+\theta_2)i}$ 

Or in the [[Forms of Complex Numbers|polar form]] with $cos(\alpha + \beta)$ and $sin(\alpha + \beta)$ [[old trig functions|formulas]]
$$
\begin{align} 
r(\cos \alpha+i \sin \alpha) \cdot s(\cos \beta+i \sin \beta) &=
rs(\cos (\alpha+\beta)+i \sin (\alpha+\beta))
\end{align}
$$
or with [[cis]]
$$cis\alpha \cdot cis\beta = cis(\alpha+\beta)$$
## Division
It can easily be expressed through the [[#Multiplication|multiplication]] of the conjugation (*with the help of [[#The sum of two squares factorization]]*)
$$\frac{z}{w}=\frac{a+b i}{c+d i}=\frac{a+b i}{c+d i} \cdot \frac{c-d i}{c-d i}=\frac{(a+b i)(c-d i)}{c^2+d^2}=\frac{z \cdot \bar{w}}{|w|^2}$$
or with [[cis]]
$$\frac{4cis\frac{\pi}{12}}{2cis\frac{7\pi}{12}} = 2cis(\frac{\pi}{12} -\frac{7\pi}{12}) = 2cis(-\frac{\pi}{2})$$

<br>

>[!Tip] Visualization
>Both division and multiplication can be understood as a modulus $r$ scaling and an argument $\theta$ rotation
>[Relation visualized](https://www.khanacademy.org/math/algebra-home/alg-complex-numbers/alg-multiplying-and-dividing-complex-numbers-in-polar-form/a/visualizing-complex-multiplication)
>
>Division rotates a point by $-\theta$ and scales by $\frac{1}{r}$
>Multiplication rotates a point by $\theta$ and scales it by $r$


### Raising to a power
As demonstrated [here](https://www.khanacademy.org/math/algebra-home/alg-complex-numbers/alg-multiplying-and-dividing-complex-numbers-in-polar-form/v/powers-of-complex-numbers)
Raising a complex number simply rotates the number in the polar plane.
The most simply way to express this is via exponential form
$$(e^{\alpha i})^{\beta} = e^{\alpha \beta i}$$
*E.g.:* $${\begin{array}\ (cos(\frac{2\pi}{3}) + i\sin(\frac{2\pi}{3}))^{20} = e^{20\cdot (\frac{2\pi}{3})i} = e^{\frac{40\pi}{3}i}, \ \text{then} \\ \frac{40\pi}{3} = 13\frac{1}{3}\pi \\ \text{Subtract by the largest multiple of } 2\pi \\ 
13\frac{1}{3}\pi-12\pi=\frac{4\pi}{3} \\
\text{ans: } cos(\frac{4\pi}{3})+isin(\frac{4\pi}{3})\end{array}}$$
or with [[cis]]
$$(|z|cis\theta)^3 = |z|cis\theta \cdot |z|cis\theta \cdot |z|cis\theta = |z|^3cis(\theta+\theta+\theta)=|z|^3cis(3\theta) $$
> [!Info] The generalization of this process is called **[[De Moivre's Theorem]]**
> $$(|z|cis\theta)^n = |z|^ncis(n\theta), \quad \text{for all } n \in \mathbb{Q}$$



---

### The sum of two squares factorization
$$
\begin{array}{l}
z\cdot\bar{z} =\Re(z)^2 +  \Im(z)^2 \\
(a+bi)(a-bi) = a^2 + b^2
\end{array}
$$