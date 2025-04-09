### First Substitution Law

Suppose that $Q$ is any proposition, and that $p$ is a propositional variable. Consider any [[tautology]]. If $Q$ is substituted for $p$ in all places where $p$ occurs in the tautology, then the result is also a tautology

### Second Substitution Law

Suppose $P$ and $Q$ are any propositions such that $P\equiv Q$. Suppose $R$ is any compound proposition in which $P$ occurs as a sub-proposition. Let $R'$ be the proposition that is obtained by substituting $Q$ for the occurrence of $P$ in $R$. Then $R \equiv R'$

> [!note]
> Note that in this case, the theorem does not require $Q$ to be substituted for _every_ occurrence of $P$ in $R$. You are free to substitute for one, two, or as many occurrences of $P$ as you like, and the result is still logically equivalent to $R$.

> [!example] 
> The [[#Second Substitution Law]] allows us to use logical equivalence to 'simplify' a compound proposition.
> 
> For example, take the use of the [[Basic of Boolean Algebra#Double negation|double negation law]], with which the equivalence below follows
>$$
q \to (\lnot(\lnot p)) \equiv q\to p
>$$

> [!tip] Simplifications
> The power of the second substitution law lies in a kind of "associativity" of propositions. If $P\equiv Q$ and $Q\equiv R$, then by substituting $Q$ with $R$, we get that $P\equiv R$. This is formally called the [[Law of Syllogism]]
> 
> This effectively enables chains of logical equivalences which "simplify" the work of doing "simplifications"
