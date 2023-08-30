# Categories

A category **C** comprises the following data: [^1] [^2]

[^1]: [category in nLab](https://ncatlab.org/nlab/show/category)

[^2]: [4.2 Definitions \| The Stacks project](https://stacks.math.columbia.edu/tag/0013)

1. A class of **objects** $\textrm{Obj}(\mathbf{C})$.

2. For each pair of objects $X,Y$, a class of **morphisms**
```math
\mathrm{hom}_{\mathbf{C}}(X,Y)$$.
```
A morphism $$f \in \textrm{hom}_{\mathbf{C}}(X,Y)$$ has **domain** $\textrm{dom}(f)=X$ and **codomain** $\textrm{cod}(f)=Y$.

3. For each triple of objects $X,Y,Z$, a map
```math
\circ_{X,Y,Z}:\textrm{hom}_{\mathbf{C}}(X,Y) \times \textrm{hom}_{\mathbf{C}}(Y,Z) \to \textrm{hom}_{\mathbf{C}}(X,Z)
```
called **composition** and denoted by $\circ_{X,Y,Z}:(f,g) \mapsto g \circ f$. [^3]

4. For each object $X$, a morphism
```math
\textrm{id}_X \in \textrm{hom}_{\mathbf{C}}(X,X),
```
called the **identity morphism**.

[^3]: [composition in nLab](https://ncatlab.org/nlab/show/composition)

The data has to satisfy the following rules:

1. For each morphism $f$, it holds that $f \circ \textrm{id}_{\textrm{dom}(f)} = f$, called the **right identity law**. [^4]

2. For each morphism $f$, it holds that $\textrm{id}_{\textrm{cod}(f)} \circ f = f$, called the **left identity law**.

3. For each triple of morphisms $f,g,h$, if
$\textrm{cod}(f)=\textrm{dom}(g)$ and $\textrm{cod}(g)=\textrm{dom}(h)$ then  
```math
h \circ (g \circ f) = (h \circ g) \circ f,
```
called the **associative law**. [^5]

[^4]: [identity element in nLab](https://ncatlab.org/nlab/show/identity+element)

[^5]: [associativity in nLab](https://ncatlab.org/nlab/show/associativity)

# The category structure of **Set**

$\textrm{Obj}(\mathbf{Set})$ is the class of sets.

For each pair of sets $X,Y$, the class of morphisms
$\textrm{hom}_{\mathbf{Set}}(X,Y)$ is the set of functions $Y^X$. [^small]

Halmos, Section 8, "Functions":

> $Y^\emptyset$ has exactly one element, namely $\emptyset$,
> whether $Y$ is empty or not, and (ii) if $X$ is not empty, then $\emptyset^X$
> is empty.

For each triple of objects $X,Y,Z$, the composition

$\circ_{X,Y,Z}:Y^X \times Z^Z \to Z^X$

## $X \neq \emptyset, Y \neq \emptyset, Z \neq \emptyset$

$$
\circ_{X,Y,Z}(f,g)(x) = g(f(x)),\quad f \in Y^X, g \in Z^Y, \quad x \in X.
$$

## $X = \emptyset, Y \neq \emptyset, Z \neq \emptyset$

$$
Y^X=\lbrace\emptyset\rbrace
$$

$$
\circ_{X,Y,Z}(\emptyset,g) = \emptyset, \quad g \in Z^Y.
$$

## $X \neq \emptyset, Y = \emptyset, Z \neq \emptyset$

...

## $X \neq \emptyset, Y \neq \emptyset, Z = \emptyset$

...

## $X = \emptyset, Y = \emptyset, Z \neq \emptyset$

...

## $X = \emptyset, Y \neq \emptyset, Z = \emptyset$

...

## $X \neq \emptyset, Y = \emptyset, Z = \emptyset$

...

## $X = \emptyset, Y = \emptyset, Z = \emptyset$

...

For each set $X$ that is not empty, the identity morphism $\textrm{id}_X \in X^X$ is

$$
\textrm{id}_X(x) = x, \quad x \in X.
$$

When $X$ is empty,

$$
\mathrm{id}_\emptyset = \emptyset \in \emptyset^\emptyset.
$$

When for each pair of objects $X,Y$ it holds that the class of morphisms
```math
\textrm{hom}_{\mathbf{C}}(X,Y)
```
is a **set**, the category **C** is called **locally small**. See [locally small category in nLab](https://ncatlab.org/nlab/show/locally+small+category) When the class of objects and the class of morphisms are both sets, the category is called **small**. For doing algebraic geometry my impression is that there one works with small categories. See [The Stacks project](https://stacks.math.columbia.edu/)