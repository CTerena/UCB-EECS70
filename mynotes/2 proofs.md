## 1.Proofs  
A **proof** is a finite sequence of steps, called *logical deductions*, which establishes the truth off a desired statement.  

In particular, the power of a proof lies in the fact that using *finite* means, we can guarantee the truth of a statement with *infintely* many cases.  

Recall that there are certain statements, called axioms(公理) and postulates(假设), that we accept without proof.  

## 2.Notations and basic facts:  
$\mathbb{Z}$ denotes the set of integers.  
$\mathbb{N}$ denotes the set of natural numbers.  
These two sets above are closed under addition and multiplication.  

Given integers $a$ and $b$, we say that $a$ divides $b$ (denoted $a|b$) iff there exists an integer $p$ that $b=ap$.   
We use the noatation $:=$ to indicate a definition.  

## 3.Direct Proof
  *Goal*: To prove *P*\Longrightarrow *Q*.  
  *Approach*:  
Assume *P*  
...  
Therefore *Q*  

Whenever you wish to prove an equivalence $P\Longleftrightarrow Q$, always proceed by showing $P\Longrightarrow Q$ and $Q\Longrightarrow P$ separately.  

## 4.Proof by Contraposition
*Goal*: To prove $P\Longrightarrow Q$.  
*Approach*:  
Assume $\urcorner Q$  
...  
Therefore $\urcorner P$  
*Conclusion*: $\urcorner Q\Longrightarrow \urcorner P$, which is equivalent to $P\Longrightarrow Q$  

example: Pigeonhole Principle  

## 5.Proof by Contradiction  
*Goal*: To prove $P$  
*Approach*:  
Assume $\urcorner P$.  
...  
$R$  
...  
$\urcorner R$  
*Conclusion*: $\urcorner P\Longrightarrow \urcorner R\wedge R$, which is a contradiction. Thus, $P$.  

example: Prove the theorem: *There are infinitely many prime numbers*.  

## 6.Proof by Cases
Prove some object $X$ exists, but without explicitly revealing what $X$ itself is.

## 7.Some advice  
First, get in the habit of thinking carefully before you write down the next sentence of your proof. If you cannot explain clearly why the step is justified, you are making a leap and you nned to go back and think some more. In theory, each step in a proof must be justified by appealing to a definition or general axiom. In practice the depth to which one must do this is a matter of taste.  
A justification can be stated without proof only if you are absolutely confident that (1) it is correct and (2) the reader will automatically agree that it is correct. A subsidiary result that is useful in a more complex proof is called a *lemma*. It is often a good idea to break down a long proof into several lemmas.  
The dividing line between lemmas and theorems is not clear-cut. Usually, when writing a paper, the theorems are those propositions that you want to "export" from the paper to the rest of the world, whereas the lemmas are propositions used locally in the proofs of your theorems.

