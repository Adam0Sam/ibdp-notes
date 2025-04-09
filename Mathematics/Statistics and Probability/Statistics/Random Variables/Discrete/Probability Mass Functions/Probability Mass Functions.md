The probability distribution of a discrete random variable may be describes using a **probability mass function** $P(x)=\mathrm{P}(X=x)$. The domain of such a function is set to $\{ x_{1},x_{2},x_{3},\dots,x_{n} \}$ and the range is set to $\{ p_{1},p_{2},p_{3},\dots,p_{n} \}$

> [!info] Expected value
> An [[Expectation|expected value]] is the average value we can *expect* to be awarded

> [!tip] Fair games
> A game is said to be fair if $E(X)=0$ (that is to say, on average the expected gain is 0)

In addition to [[Expectation]], [[Variance and Standard Deviation]] of a discrete random variable may be measured to obtain the **spread from the mean** of data values we expect to obtain when an experiment is performed many times.

If $\mu$ and $\sigma$ of $X$ are known, then the these properties ($\mu$ and $\sigma$) of [[Linear Transformation of a Random Variable|a related random]] variable $aX+b$ can be determined (where $a,b \in \mathbb{R}$)

> [!tip] The binomial experiment
> $P(x)$ denotes the probability of $x$ after one trial, however, the amount of trials can be extended to $n \in \mathbb{Z}^+$.
> 
> A $\mathrm{P}(X=x)$ with only two discrete values allows the formulation of a binomial experiment with $n$ independent trials and two possible results.
> 
> The probability distribution after $n$ trials in a binomial experiment is called a [[Binomial Distribution]] and the probability mass function of such a distribution is
>$$
P(x)=\mathrm{P(X=x)} = \binom{n}{x}p^{x}(1-p)^{n-x}
>$$

