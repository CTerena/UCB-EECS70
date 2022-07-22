Induction is a powerful tool which is used to establish that a statement holds for *all *natural* numbers. In other words, induction provides a way to reason infinitely many natural numbers by *finite* means.  

Letting $P(n)$ denote the statement $\sum_0^n i=n(n+1)/2, our goal was to prove that $\forall n\in \mathbb{N} , P(n)$. The *principle of induction* asserts that to prove this requires three simple steps:  
1. **Base Case**: Prove that $P(0)$ is true.  
2. **Induction Hypothesis**: For arbitrary $k\geq 0$, assume that $P(k)$ is true.  
3. **Inductive Step**: With the assumption of the Induction Hypothesis in hand,show that $P(k+1)$ is true.  

Sometimes, we couldn't prove a statement, but instead we can hypothesize a stronger one and manage to prove that. The reason is that the original claim did not capture the true *structure* of the underlying fact we were trying to prove - it may be too vague.  

*Strong* induction cannot prove statements which *weak* induction cannot prove.  
