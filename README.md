# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$


$f(n) \in O(g(n)) \iff \exists c > 0, \exists n_0, \forall n \geq n_0: f(n) \leq c \cdot g(n)$ 


There is two differences here. 

1. The first difference is seen within the context of constants, where little o requires all constants for it to hold seen in $\forall c > 0$. In big O notation though, this is not the case where we instead only need one constant for it to hold in $\exists c > 0$ 

2. The second reason comes in with the difference in the last art of the inequality where little o uses a < and big O uses a ≤. Little o uses this as it is considered more strict, where f(n) grows slower compared to g(n) and big O is looser in a sense that it can grow to be as fast as g(n). 


As a result $f(n)\in o(g(n))$ implies that $f(n)\in O(g(n))$ because little o  is stricter than big O.


Sources:
TA Ali -  helped to explain what the initial inequality meant. 

https://github.com/Experience-Monks/math-as-code - looked at this to write notation 


