A differential equation is an equation involving a [[Differential Calculus|derivative]] of a function.

A solution of a differential equation is a function of $y$ in terms of $x$, which satisfies the differential equation.

Solutions can be classified as *general* and *particular* (which is a member function of the general solution family)


[[Euler's Method for Numerical Integration]] allows approximating a particular solution's value for a differential equation



> [!info] Separability
> Differential equations of two variables may be separated (for example, [[Homogeneous Differential Equations]])
>$$
\begin{align}
&\frac{dy}{dx} = f(x)g(y) \Rightarrow \frac{1}{g(y)}\frac{dy}{dx}  =f(x) \\
&\therefore \int \frac{1}{g(y)}\frac{dy}{dx}  \, dx =\int f(x) \, d \Rightarrow \int \frac{1}{g(y)} \, dy =\int f(x) \, dx  
\end{align}
>$$
>This same process is used to model [[Logistic Growth|logistic growth]]



> [!warning] Separating generally non-separable equations
> A differential equation of form 
>$$
\frac{dy}{dx}  + P(x)y=Q(x) 
>$$
> is generally non-separable
> 
> However, suppose there is a function $I(x)$ called the **integrating factor**, such that
>$$
\begin{align}
\frac{d}{dx}(I(x)y) &= I(x) \left( \frac{dy}{dx} +P(x)y \right ) \\
&= I(x)Q(x)
\end{align}
>$$
>Thus, if $I(x)$ exists, then
>$$
\begin{align}
&I(x)\frac{dy}{dx} + I'(x)y = I(x)\frac{dy}{dx} + I(x)P(x)y  \\
&I'(x)y=I(x)P(x)y \\
& \frac{I'(x)}{I(x)} = P(x) \\ \\
&\therefore \int \frac{I'(x)}{I(x)} \, dx = \ln |I|+c = \int P(x) \, dx  \\
&\therefore I(x) = Ae^{\int P(x) \, dx }, \quad \text{where } A = e^{-c}
\end{align}
>$$
>It follows that
>$$
\begin{align}
&\int \frac{d}{dx} (I(x)y) \, dx = \int I(x)Q(x) \, dx  \\
&y= \frac{1}{I(x)} \int I(x)Q(x) \, dx 
\end{align}
>$$
