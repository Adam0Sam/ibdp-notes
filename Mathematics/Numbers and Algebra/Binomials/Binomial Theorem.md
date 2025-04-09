The **Binomial Theorem**, derived from [[Pascal's triangle]]

$$
\begin{align}
\text{For} \ n \in \mathbb{z}^+, \quad
(a+b)^n &= a^n + \binom{n}{1}a^{n-1}b + \ ... \ +  \binom{n}{r}a^{n-r}b^r + \ ... \ + b^n = \\
&= \sum_{r=0}^n\binom{n}{r}a^{n-r}b^r \\ \\
\end{align}
$$
$$\text{where} \ \binom{n}{r}=\frac{n!}{r!(n-r)!} \quad \text{is the binomial coefficient for } n \in \mathbb{Z}^+, \ r\in \mathbb{N}, \ r \le n
$$

The **general term** or $(r+1)th$ term in the binomial expansion $(a+b)^n$ is
$$T_{r+1} = \binom{n}{r}a^{n-r}b^r$$

## The Extension for $n \in \mathbb{Q}$
$$
\begin{align}
\text{For} \ n \in \mathbb{Q}, \quad (a+bx)^n = a^n\sum_{r=0}^n\binom{n}{r}(\frac{bx}{a})^r 
\end{align}
$$
$$\text{where} \ \binom{n}{r}=\frac{n(n-1)(n-1)...(n-r+1)}{r!} \quad \text{is the binomial coefficient for} \ n \in \mathbb{Q}, \ r\in \mathbb{Z}^+
$$
The **interval of convergence** is $|\frac{bx}{a}|<1$, which means $$-|\frac{a}{b}| < x < |\frac{a}{b}|$$ 

---

> [!Example] Useful?
> $$\binom n0 + \binom n1 + \binom n2 + \ ... \ + \binom{n}{n-1} + \binom nn = 2^n$$


