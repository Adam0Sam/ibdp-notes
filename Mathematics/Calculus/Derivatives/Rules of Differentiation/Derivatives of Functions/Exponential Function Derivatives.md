$$
\text{If } f(x)=b^x\quad \text{ then } f'(x) = f'(0)\cdot b^x 
$$

#### Proof
$$
\begin{align}
f'(x) &= \lim_{ h \to 0 } \frac{b^{x+h}-b^x}{h} \\
&= \lim_{ h \to 0 } \frac{b^x(b^{h}-1)}{h} \\
&= b^x \cdot\lim_{ h \to 0 } \frac{b^{h}-1}{h} \\
 \\ \\
\text{But } f'(0) &=\lim_{ h \to 0 } \frac{f(0+h)-f(0)}{h}  \\
&= \lim_{ h \to 0 } \frac{b^h-1}{h}  \\
 \\
 \\
& \therefore f'(x)=b^x\cdot f'(0)
\end{align}
$$


> [!Tip]  $\frac{\mathrm{d}}{\mathrm{d}x}(e^x)$
> For $f(x)=f'(x)$, $\lim_{ h \to 0 } \frac{b^h-1}{h} = 1$, following this logic
> $$
\begin{align}
& \lim_{ h \to 0 } b^h = \lim_{ h \to 0 } (h+1)  \\
& b = \lim_{ h \to 0 } (h+1)^{1/h}  \\ \\
& \text{Letting } h = \frac{1}{n}, \quad b = \lim_{ n \to \infty } \left( 1+\frac{1}{n} \right)^n = e  \\ \\
&\therefore \text{If } f(x)=e^x \quad \text{then } f'(x)=f(x)
\end{align}
$$

#### General Derivatives

All proofs done using [[The Chain Rule]]


> [!Example]  $f(x)=e^x$
> Suppose $y=e^{f(x)}=e^u$, where $u=f(x)$
>
>$$
\begin{align}
\frac{\mathrm{d}y}{\mathrm{d}x} &= \frac{\mathrm{d}y}{\mathrm{d}u}\cdot\frac{\mathrm{d}u}{\mathrm{d}x} \\
&= e^u \cdot\frac{\mathrm{d}u}{\mathrm{d}x} \\
&= e^{f(x)}\cdot f'(x)
\end{align}
$$

> [!Example] $f(x)=a^x$
>
>Suppose $y=a^{f(x)}=a^u$, 
>$$
\begin{align}
\frac{\mathrm{d}y}{\mathrm{d}x} &= \frac{\mathrm{d}y}{\mathrm{d}u}\cdot\frac{\mathrm{d}u}{\mathrm{d}x} \\
&= \frac{\mathrm{d}}{\mathrm{d}u}a^u \cdot\frac{\mathrm{d}u}{\mathrm{d}x} \\
&= \frac{\mathrm{d}}{\mathrm{d}u} e^{\ln a\cdot u} \cdot\frac{\mathrm{d}u}{\mathrm{d}x} \\ 
&= e^{\ln a\cdot u}\ln a \cdot \frac{\mathrm{d}u}{\mathrm{d}x} \quad \text{(from ) } \frac{\mathrm{d}}{\mathrm{d}x}e^{f(x)}\\
&= a^{u}\ln a\cdot \frac{\mathrm{d}u}{\mathrm{d}x} = a^{f(x)}\ln a\cdot f'(x)
\end{align}
$$
