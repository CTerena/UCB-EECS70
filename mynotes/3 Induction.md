## 1.Mathematical Induction

Induction is a powerful tool which is used to establish that a statement holds for *all *natural* numbers. In other words, induction provides a way to reason infinitely many natural numbers by *finite* means.  
An example of formal proof:  
**Theorem** $$\forall n\in \mathbb{N} ,\sum_0^n i=n(n+1)/2.$$  
*Proof.* We proceed by *induction* on the variable *n*.  

*Base case (n=0):* Here, we have $\sum_0^0 i=0=0(0+1)/2. Thus, the base case is correct.  

*Induction Hypothesis:* For arbitrary $n=k\geq 0, assume that \sum_0^k i = k(k+1)/2. In words, the Induction HYpothesis says "let's assume we have proved the statement for an arbitrary value of $n=k\geq 0$"  

*Induction Step*: Prove the statement for $n=(k+1)$, i.e., show that $\sum_0^{k+1} i=(k+1)(k+2)/2$:  
$$\sum
