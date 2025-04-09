$$
\begin{array}{}
\text{If } f\ \text{ is differentiable at }\ x=a, \ \text{then }  \\
f  \ \text{ is also continuous at x=a}
\end{array}
$$
> [!Warning]  [[Function Continuity|Continuous]] != differentiable
> If a function is continuous at $x=a$, it is not necessarily differentiable at $x=a$
#### Proof

$$
\begin{align}
\lim_{ h \to 0 }f(a+h)-f(a)  
&=\lim_{ h \to 0 } \frac{f(a-h)-f(a)}{h} \cdot h  \\
&= \lim_{ h \to 0 } \frac{f(a-h)-f(a)}{h} \cdot \lim_{ h \to 0 } h \\
&= f'(a) \cdot 0  \\
&= 0 
\end{align}
$$
$$
\begin{align}
 & \text{Letting } x=a+h \text{, this is equivalent to } \lim_{ x \to a } f(x)=f(a)  \\
& \therefore f \ \text{is continuous at } x=a
\end{align}
$$

> [!Tip] Testing for differentiability
> A function $f$ with domain ${\mathrm{D}}$ is differentiable at $x=a, \ a \in \mathrm{D}$ if:
>
>$$
\begin{align}
& \text{1. } f \ \text{ is continuous at } x=a \\
& \text{2. } f'_{-}(a)=\lim_{ h \to 0^- } \frac{f(a-h)-f(a)}{h}, \quad f'_{+}(a)=\lim_{ h \to 0^+ } \frac{f(a-h)-f(a)}{h} \quad \text{ and } f'_{-}(a)=f'_{+}(a)
\end{align}
> $$
>

