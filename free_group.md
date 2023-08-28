# Free group on a set

Let $X$ be a set, $X \neq \emptyset$.

If $X \neq \emptyset$,
define $I:X \to X$ for $x \in X$ by $I(x)=x$.

Let $Y$ be a set disjoint from $X$ for
which there is a bijection $J:X \to Y$.

For $x \in X$, write $x^{-1} = J(x)$. 

Let

$$
L = X \cup Y = \bigcup_{x \in X} \lbrace I(x), J(x) \rbrace = \bigcup_{x \in X} \lbrace x, x^{-1} \rbrace,
$$

elements of which we call characters.

Let $a \in L^+$, a string comprised of one or more characters from $L$. For some $n \geq 1$, $a \in L^n$:

$$
a = a_1 \cdots a_n, \qquad a_i \in L, 1 \leq i \leq n.
$$

If $a_i a_{i+1} = I(x)J(x)$ or $a_i a_{i+1} = J(x)I(x)$, call

$$
a_1 \codts a_{i-1} a_i a_{i+1} a_{i+2} \cdots a_n \to a_1 \cdots a_{i-1} a_{i+2} \cdots a_n 
$$

a reduction.

If $a \in L^+$ has no reductions, it is called reduced.
