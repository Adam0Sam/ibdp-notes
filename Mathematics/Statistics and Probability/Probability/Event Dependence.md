For events $A$ and $B$, $A \ | \ B$ denotes the event "*$A$ given that $B$ has occurred*"

If both outcomes exist in the same [[The Sample Space|sample space]] $U$, meaning that they are equally likely, then

$$
\mathrm{P}(A \ | \ B) = \frac{n(A \cap B)}{n(B)} = \frac{\frac{n(A \cap B)}{n(U)}}{\frac{n(B)}{n(U)}} = \frac{\mathrm{P}(A \cap B)}{\mathrm{P}(B)}
$$


> [!info] Definition of Independent Events
> $A$ and $B$ are **independent** events if the occurrence of each one of them does not affect the probability that the other occurs
>$$
\begin{align}
\text{This means that } &\quad \mathrm{P}(A\ | \ B) = \mathrm{P}(A\ | \ B')=\mathrm{P}(A) \\
\text{and that } &\quad \mathrm{P}(B\ | \ A) = \mathrm{P}(B\ | \ A')=\mathrm{P}(B) \\
\end{align}
>$$
>
>thus
>$$
A \text{ and } B \text{ are independent events} \ \Leftrightarrow \ \mathrm{P}(A\cap B)=\mathrm{P}(A)\mathrm{P}(B)
>$$


[[Bayes' Theorem]] follows from the definition of dependence