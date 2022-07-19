## 1.Propositional Logic  
**proposition**: a statement which is either true of false  
 
For examples, these statements are all propositions:  
- $\sqrt{3}$ is irrational.    
- $1 + 1 = 5$.  
- Li Yang likes touching fish.  
  
On the other hand, these statements aren't propositions:  
- $2 + 2$  
- $x^2+3x=5$ [What's *x*?]  
  
Furthermore, these statements aren't propositions either, which can be a little contradictive:   
- Guan Shengzhong often eats in dining hall.  
- Kang Yuyu is popular among girls.  

What we should notice is that **propositions should not include fuzzy terms.**  
  
Next thing, propositions may be joined together to form more complex statements. Let *P*, *Q* and *R* be variables representing propositions. The simplest way of joiningthese propositions together is to use the connectives "and", "or" and "not."  
      1. **Conjunction**: $P\wedge Q$(*p* and *Q*). True only when both *P* and *Q* are true.  
      2. **Disjunction**:  $P\vee Q$(*P* or *Q*). True when at least one of P and Q is true.  
      3. **Negation**:   $\urcorner P$(not *P*). True when P is false.  
Statements like these, with variables, are called *propositional forms.*  

A fundamental principle known as the **law of the excluded middle** says that, for any proposition *P*, either *P* or \urcorner*P* is true.

A propositional form that is always true regardless of the truth values of its variables is called a *tautology*.

Conversely, a statement such as *P* \bigvee\urcorner*P*, which is always false, is called a *contradiction*.  

The most important and subtle propositional form is an **implication**:  
  **Implication**: $P\Longrightarrow Q$("*P* implies *Q*"). This is the same as "If *P*, then *Q*."  
Here, *P* is called the *hypothesis* of the implication, and *Q* is the *conclusion.*  

Note that $P\Longrightarrow Q$ is always true when *P* is false. This may be against our intuition, but we stipulate it in this way. When an implication is stupidly true because the hypothesis is false, we say that it is *vacuously true*.  
Note also that $P\Longrightarrow Q$ is **logically equivalent** to $\urcorner P \vee Q$, you can draw a truth table and see it. We write this as  
$$(P\Longrightarrow Q)\equiv (\urcorner P \vee Q)$$.  
Also, here are some of the different ways of saying $P\Longrightarrow Q$:  
- if *P*, then *Q*  
- *Q* is *P*  
- *P* only if *Q*  
- *P* is **sufficient** for *P*  
- *Q* is **necessary** for *P*  
- *Q* unless not *P*  

If both $P\Longrightarrow Q$ and $Q\Longrightarrow P$ are ture, then we say "*P* if and only if *Q*"(abbreviated "*P* iff *Q*). Formally, we write $P\Leftrightarrow Q$.  

## 2.Quantifiers  
Just remember these two names:  
- The *universal quantifier* :  $\forall$  
- The *existential quantifier* :  $\exists$  

## 3.Much Ado About Negation  
You have already known *De Morgan's Laws*, now let's remember theirs propositional form:  

$$\urcorner (P\wedge Q) \equiv (\urcorner P \vee \urcorner Q)$$  

$$\urcorner (P\vee Q) \equiv (\urcorner P \wedge \urcorner Q)$$  

Besides, there're two laws that hold for any proposition *P* quantified over any universe(incluing infinite ones):  
$$\urcorner(\forall xP(x)) \equiv \exists x\urcorner P(x)$$  

$$\urcorner(\exists xP(x)) \equiv \forall x\urcorner P(x)$$

## 4.Some examples  
Write the sentence "there're at least three distinct integers x that satisfy $P(x)$" as a proposition:  
$$\exists x\exists y\exists z(x\neq y\wedge y\neq z\wedge z\neq x\wedge P(x)\wedge P(y)\wedge P(z))$$  

Now write the sentence "there're **at most** three distinct integers x that satisfy $P(x)$" as a proposition:  
$$\exists x\exists y\exists z\forall d(P(d)\Longrightarrow d=x\vee d=y\vee d=z)$$  

Finally, if we want to express the sentence "there're **exactly** three distinct integers x that satisfy $P(x)", we can just use the *conjuction* of the two propositions above!
