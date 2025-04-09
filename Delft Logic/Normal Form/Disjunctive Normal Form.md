A compound proposition is said to be in *disjunctive normal form*, or *DNF*, if it is a **disjunction** of **conjunctions** of **[[Simple Terms in a Compound Proposition|simple terms]]**, and if, furthermore, each propositional variable **occurs at most once** in each conjunction and each conjunction occurs at most once in the disjunction.

> [!example] Examples of propositions in DNF
> ![[Pasted image 20250223162923.png]]

#### *Informal* demonstration that propositions in DNF may correspond to any truth table

> [!info] Theorem
> Consider a table that lists a logical output value for every combination of values of several propositional variables. *Assume* that at least one of the output values is true. Then there is a proposition containing those variables such that the value of the proposition for each possible combination of the values of the variables is precisely the value specified in the table. It is possible to choose the proposition to be in disjunctive normal form.

**Proof.** Consider any row in the table for which the output value is $\mathbb{T}$. Form a conjunction of simple terms as follows: For each variable, $p$, whose value is $\mathbb{T}$ in that row, include $p$ itself in the conjunction; for each variable, $q$, whose value is $\mathbb{F}$ in the row, include $\lnot q$ in the conjunction. The value of this conjunction is $\mathbb{T}$ for the combination of variable values given in that row of the table, since each of the terms in the conjuction is true for that combination of variables. Furthermore, for any _other_ possible combination of variable values, the value of the conjunction will be $\mathbb{F}$, since at least one of the simple terms in the conjunction will be false.

Take the disjunction of all such conjunctions constructed in this way, for each row in the table where the output value is true. This disjunction has the value $\mathbb{T}$ if and only if one of the conjunctions that make it up has the value $\mathbb{T}$—and that is precisely when the output value specified by the table is $\mathbb{T}$. So, this disjunction of conjunctions satisfies the requirements of the theorem.