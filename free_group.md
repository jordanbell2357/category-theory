# Free group on a set

## Words

Let $X$ be a set.

If $X \neq \emptyset$, for $x \in X$ define $I(x)=x$.

Let $Y$ be a set disjoint from $X$ for which there is a bijection $J:X \to Y$.

For $x \in X$, write $x^{-1} = J(x)$.

Let

$$
\begin{align*}
A &= X \cup Y\\
&= \left( \bigcup_{x \in X} \lbrace I(x) \rbrace \right) \cup \left( \bigcup_{x \in X} \lbrace J(x) \rbrace \right)\\
&= \bigcup_{x \in X} \lbrace I(x), J(x) \rbrace,
$$

elements of which we call **characters**.

The **Kleene star** of $$A$ is

$$
A^* = \bigcup_{n \geq 0} A^n.
$$

Elements of $W(X)=A^*$ are called **words over the set** $X$.

$$
A^0 = \lbrace \epsilon \rbrace
$$

We call $\epsilon$ the **empty word**. [^1]

[^1]: <https://arbital.com/p/5zr/empty_set_universal_property/>

For $n \geq 1$ and for  $a \in A^n$, we have

$$
a = a_1 \cdots a_n, \qquad a_i \in A, 1 \leq i \leq n.
$$

## Reduction

If $a_i a_{i+1} = I(x)J(x)$ for some $x \in X$
or $a_i a_{i+1} = J(x)I(x)$ for some $x \in X$,
we call

$$
a_1 \cdots a_i a_{i+1} \cdots a_n \longrightarrow a_1 \cdots a_{i-1} \epsilon a_{i+2} \cdots a_n 
$$

a **reduction**.

If a word $a$ has no reductions, it is called a **reduced word**. [^2]

[^2]: <https://arbital.com/p/freely_reduced_word/>

Let $W_R(X)$ be the set of reduced words over $X$.

## Free group on a set



[^3]

[^3]: [Formal definition of the free group \| Arbital](https://arbital.com/p/free_group/?l=5s1)



## Universal property


[^4]

[^4]: [Free group universal property \| Arbital](https://arbital.com/p/free_group/?l=6gd)
