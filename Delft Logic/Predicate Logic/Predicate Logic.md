A predicate is a kind of incomplete proposition, which becomes a proposition when it is applied to some entities. This is in contrast to [[propositional logic]], which only treats complete propositions contained within proposition variables

> [!example]
> In the proposition "*the rose is red*", the predicate is "_is red_". By itself, ‘is red’ is not a proposition.

> [!tip] Domain of discourse
> Generally, it is not useful to apply predicates to all entities (e.g. *My sofa is mortal*), therefore the **domain of discourse for the predicate** defines the category of entities for which the predicate may be applied

The setup allows for a formal definition of a [[One-Place Predicate]], 

Similarly, definitions can be made for multi-place predicates (e.g. $Q(a,b)$ might denote a proposition that is obtained when $Q$ is applied to the entities $a$ and $b$)

> [!tip] Domain of discourse for multi-place predicates
> Each 'slot' in a multi-place predicate may have its own domain of discourse

Predicates, once applied to entities, produce propositions which abide all the same laws of [[propositional logic]]

General statements on the value of predicate based statements can be acquired with the use of [[Quantifiers]]

> [!info] Logical Equivalence
> In predicate logic, two formulas ore logically equivalent if they have the same truth value for all possible predicates
> 
> This in contrast to the notion of logical equivalence in [[propositional logic]]. This is also much more complicated and required the use of "formulas"
> 
> > [!tip] Formal Definition
> > Let $\mathcal{P}$ be a formula of predicate logic which contains one or more predicate variables. $\mathcal{P}$ is said to be a tautology if it is true whenever all the predicate variables it contains are replaced by actual predicates. Two formulas $\mathcal{P}$ and $\mathcal{L}$ are said to be logically equivalent if $\mathcal{P} \leftrightarrow \mathcal{L}$ is a tautology.

> [!example]
> Finding logical equivalence in predicate logic requires much more intricate reasoning that just truth table mapping
> 
> The following are examples of some important predicate formula equivalences
> 
> > [!tip] DeMorgan's laws for predicate logic
> > $$
 >\begin{array}{}
> \lnot(\forall xP(x))\equiv \exists x(\lnot P(x)) \\
> \lnot(\exists xP(x))\equiv \forall x(\lnot P(x)) \\
> \end{array}$$
> >
> 
There are two other useful laws to remember for two-place predicate formulas
>$$
\begin{array}{}
\forall x\forall yQ(x,y)\equiv \forall y\forall xQ(x,y) \\
\exists x\exists yQ(x,y)\equiv\exists y\exists xQ(x,y)
\end{array}
>$$

