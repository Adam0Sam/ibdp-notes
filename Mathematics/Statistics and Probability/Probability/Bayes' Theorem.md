Bayes' Theorem follows from an ability to express $\mathrm{P}(A\cap B)$ with either $\mathrm{P}(A \ | \ B)$ or $\mathrm{P}(B \ | \ A)$ (from the definition of [[event dependence]])

$$
\begin{cases}
\mathrm{P}(A \ | \ B) = \frac{\mathrm{P(A \cap B)}}{\mathrm{P(B)}} \\
\mathrm{P}(B \ | \ A) = \frac{\mathrm{P}(A \cap B)}{\mathrm{P}(A)}
\end{cases}
\implies
\mathrm{P}(A \ | \ B) = \frac{\mathrm{P}(B \ | \ A )P(A)}{P(B)}
$$
> [!info] Partitions of [[the sample space]]
> It is clear that $A \cap A'=\varnothing$ and $A \cup A'=U$ are both true
> 
> Thus any other event $B$ can be expressed via the partition of $U$ as 
>$$
\begin{align}
\mathrm{P}(B) &= \mathrm{P}(B \cap A) + \mathrm{P}(B \cap A') \\
&=\mathrm{P}(B \ | \ A)\mathrm{P}(A) + \mathrm{P}(B \ | \ A')\mathrm{P}(A') 
\end{align}
>$$
> ![[Pasted image 20250119213443.png]]
> 
> Thus Bayes' Theorem may be rewritten (as is commonly done) as such
>$$
\mathrm{P}(A \ | \ B) = \frac{\mathrm{P}(B \ | \ A )P(A)}{\mathrm{P}(B \ | \ A)\mathrm{P}(A) + \mathrm{P}(B \ | \ A')\mathrm{P}(A') }
>$$
>
> This reasoning extends to greater partition counts
