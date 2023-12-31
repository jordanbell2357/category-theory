# Set theory

Paul R. Halmos. *Naive Set Theory*. Van Nostrand Reinhold Company. 1960.

## Section 1, "The Axiom of Extension"

> **Axiom of extension.** Two sets are equal if and only if they have the same elements.

## Section 2, "The Axiom of Specification"

> **Axiom of specification.** To every set $A$ and to every condition $S(x)$
> there corresponds a set $B$ whose elements are exactly those elements $x$ of
> $A$ for which $S(x)$ holds.
>
> A "condition" here is just a sentence. The symbolism is intended to 
> indicate that the letter $x$ is *free* in the sentence $S(x)$; that means that $x$ occurs in
> $S(x)$ at least once without being introduced by one of the phrases
> "for some $x$" or "for all $x$." It is an immediate consequence of the axiom of extension
> that the axiom of specification determines the set $B$ uniquely. To indicate
> the way $B$ is obtained from $A$ and from $S(x)$ it is customary to write
>
> $B = \lbrace x \in A : S(x) \rbrace.$

In other words, in the above $S(x)$ is a **predicate**.

## Section 3, "Unordered Pairs"

> **Axiom of pairing.** For any two sets there exists a set that they both belong to.

> If $a$ is a set, we may form the unordered pair $\lbrace a, a \rbrace$. That unordered pair is
> denoted by $\lbrace a \rbrace$ and is called the *singleton* of $a$; it is uniquely characterized by
> the statement that it has $a$ as its only element. Thus, for instance,
> $\emptyset$ and $\lbrace \emptyset \rbrace$ are very different sets;
> the former has no elements, whereas the latter has
> the unique element $\emptyset$. To say that $a \in A$ is equivalent to saying that
> $\lbrace a \rbrace \subset A$.

## Section 4, "Unions and Intersections"

> **Axiom of unions.** For every collection of sets there exists a set that contains
> all the elements that belong to at least one set of the given collection.

## Section 5, "Complements and Powers"

> **Axiom of powers.** For each set there exists a collection of sets that contains
> among its elements all the subsets of the given set.

For a set $A$, denote by $\mathscr{P}(A)$ the **power set of** $A$, the set whose elements are
the subsets of $A$.

## Section 6, "Ordered Pairs"

> The *ordered pair* of $a$ and $b$, with *first coordinate* $a$ and *second coordinate* $b$, is the set 
> $(a,b)$ defined by
>
> $(a,b) = \lbrace\lbrace a\rbrace,\lbrace a,b\rbrace\rbrace.$
>
> However convincing the motivation of this definition may be, we must still prove
> that the result has the main property that an ordered pair must have to deserve its
> name. We must show that if $(a, b)$ and $(x, y)$ are ordered pairs and if
> $(a,b)=(x,y)$, then $a = x$ and $b = y$. To prove this, we note first that if
> $a$ and $b$ happen to be equal, then the ordered pair $(a,b)$ is the same as the singleton
> $\lbrace\lbrace a\rbrace\rbrace$. If, conversely, $(a, b)$
> is a singleton, then $\lbrace a\rbrace=\lbrace a,b\rbrace$, so that $b \in \lbrace a\rbrace$,
> and therefore $a=b$. Suppose
> now that $(a,b)=(x,y)$. If $a = b$, then both $(a, b)$ and $(x, y)$ are singletons, so that
> $x = y$; since $\lbrace x\rbrace \in (a,b)$ and $\lbrace a\rbrace \in (x,y)$, it follows that
> $a$, $b$, $x$, and $y$ are all equal.
> If $a \neq b$, then both $(a, b)$ and $(x, y)$ contain exactly one singleton, namely $\lbrace a\rbrace$ and
> $\lbrace x\rbrace$ respectively, so that $a = x$. Since in this case it is also true that both $(a, b)$
> and $(x, y)$ contain exactly one unordered pair that is not a singleton,
> namely $\lbrace a, b\rbrace$
> and $\lbrace x, y\rbrace$ respectively, it follows that $\lbrace a,b\rbrace=\lbrace x,y\rbrace$, and therefore,
> in particular,
> $b \in \lbrace x,y\rbrace$. Since $b$ cannot be $x$ (for then we should have $a = x$
> and $b = x$, and,
> therefore, $a = b$), we must have $b = y$, and the proof is complete.


> If $A$ and $B$ are sets, does there exist a set that contains all the ordered pairs $(a,b)$ with $a$ in
> $A$ and $b$ in $B$? It is quite easy to see that the
> answer is yes. Indeed, if $a \in A$ and $b \in B$, then $\lbrace a\rbrace \subset A$
> and $\lbrace b\rbrace \subset B$, and therefore $\lbrace a,b\rbrace \subset A \cup B$. Since also
> $\lbrace a\rbrace \subset A \cup B$, it follows that both $\lbrace a\rbrace$ and $\lbrace a,b\rbrace$ are
> elements of $\mathscr{P}(A \cup B)$. This implies that $\lbrace\lbrace a\rbrace,\lbrace a,b\rbrace\rbrace$
> is a subset of $\mathscr{P}(A \cup B)$, and hence that it is an element of
> $\mathscr{P}(\mathscr{P}(A \cup B))$; in other words $(a,b) \in \mathscr{P}(\mathscr{P}(A \cup B))$
> whenever $a \in A$ and $b \in B$. Once this is known, it is a routine matter to apply the axiom of
> specification and the axiom of extension to produce the unique set $A \times B$ that consists exactly
> of the ordered pairs $(a,b)$ with $a$ in $A$ and $b$ in $B$. This set is called the
> *Cartesian product* of $A$ and $B$; it is characterized by the fact that
>
> $A \times B = \lbrace x : x=(a,b) \textrm{ for some } a \textrm{ in } A \textrm{ and for some } b \textrm{ in } B\rbrace.$

> The charge of artificiality is true, but it is not too high a price to pay for conceptual economy. The concept of an ordered pair could have been introduced as an
> additional primitive, axiomatically endowed with just the right properties, no more
> and no less. In some theories this is done. The mathematician’s choice is between
> having to remember a few more axioms and having to forget a few accidental facts;
> the choice is pretty clearly a matter of taste. Similar choices occur frequently in
> mathematics; in this book, for instance, we shall encounter them again in connection with the definitions of numbers of various kinds.

> *Exercise.* If either $A=\emptyset$ or $B=\emptyset$, then
> $A \times B = \emptyset$, and conversely. If $A \subset X$ and
> $B \subset Y$, then $A \times B \subset X \times Y$, and (provided
> $A \times B \neq \emptyset$) conversely.

## Section 7, "Relations"

> We may not know what a relation is, but we do know what a set is, and the
> preceding considerations establish a close connection between relations and sets.
> The precise set-theoretic treatment of relations takes advantage of that heuristic
> connection; the simplest thing to do is to define a relation to be the corresponding
> set. This is what we do; we hereby define a *relation* as a set of ordered pairs.
> Explicitly: a set $R$ is a relation if each element of $R$ is an ordered pair;
> this means, of course, that if
> $z \in R$, then there exist $x$ and $y$ so that $z=(x,y)$. If $R$ is a relation, it is sometimes
> convenient to express the fact that $(x,y) \in R$ by writing
>
> $xRy$
>
> and saying, as in everyday language, that $x$ stands in the relation $R$ to $y$.

> In the preceding section we saw that associated with every set $R$ of ordered pairs
> there are two sets called the projections of $R$ onto the first and second coordinates.
> In the theory of relations these sets are known as the *domain* and the *range* of $R$
> (abbreviated dom $R$ and ran $R$); we recall that they are defined by
>
> $\textrm{dom} R = \lbrace x :  \textrm{for some } y (x R y)\rbrace$
>
> and
>
> $\textrm{ran} R = \lbrace y: \textrm{for some }  x (x R y)\rbrace.$

> If $R$ is a relation included in a Cartesian product $X \times Y$
> (so that $\textrm{dom} R \subset X$ and $\textrm{ran} R \subset Y$),
> it is sometimes convenient to say that $R$ is a relation *from* $X$ *to* $Y$;
> instead of a relation from $X$ to $X$ we may speak of a relation *in* $X$.

## Section 8, "Functions"

> If $X$ and $Y$ are sets, a *function from* (or *on*) $X$ *to* (or *into*) $Y$ is a relation $f$ such
> that $\textrm{dom} f = X$ and such that for each $x$ in $X$ there is a unique element $y$ in $Y$ with
> $(x,y) \in f$. The uniqueness condition can be formulated explicitly as follows:
> if $(x,y) \in f$ and $(x,z) \in f$, then $y=z$. For each $x$ in $X$, the unique $y$ in $Y$ such that
> $(x,y) \in f$ is denoted by $f(x)$. For functions this notation and its minor variants supersede
> the others used for more general relations; from now on, if $f$ is a function, we shall write $f(x)=y$
> instead of $(x,y) \in f$ or $x f y$. The element $y$ is called the *value* that the function *sends* or
> *maps* or *transforms* $x$ onto $y$. The words *map* or *mapping*, *transformation*, *correspondence*,
> and *operator* are among some of the many that are sometimes used as synonyms for *function*. The symbol
>
> $$f:X \to Y$$
>
> is sometimes used as an abbreviation for "{}$f$ is a function from $X$ to $Y$."
> The set of all functions from $X$ to $Y$ is a subset of the power set
> $\mathscr{P}(X \times Y)$; it will be denoted by $Y^X$.


> *Exercise.* (i) $Y^\emptyset$ has exactly one element, namely $\emptyset$,
> whether $Y$ is empty or not, and (ii) if $X$ is not empty, then $\emptyset^X$
> is empty.

### The empty function

#### Theorem (The empty function)

For any set $Y$, $Y^\emptyset=\lbrace \emptyset \rbrace$.

#### Proof

A function $f:\emptyset \to Y$ is a relation (set of ordered pairs) such that $\mathrm{dom}(\emptyset) = \emptyset$ and such that for each $x$ in $\emptyset$ there is a unique element $y$ in $Y$ with
$(x,y) \in \emptyset$.
Vacuously, all elements of $\emptyset$ are ordered pairs so $\emptyset$ is a relation.
$\mathrm{dom}(\emptyset) = \emptyset$.
Vacuously, for each $x$ in $\emptyset$ there is a unique element $y$ in $Y$ with
$(x,y) \in \emptyset$. Therefore, 
$\emptyset \in Y^\emptyset$.

Suppose by contradiction there is some $f \in Y^\emptyset$, $f \neq \emptyset$.
Since $f \neq \emptyset$, it follows that
there is some $x \in \emptyset$ and some $y \in Y$ such that
$(x,y) \in f$ and $(x,y) \not \in \emptyset$.
But $\emptyset$ has no elements, which is a contradiction.
Therefore, if $f \in Y^\emptyset$ then $f = \emptyset$. □

[^arbital]

[^arbital]: [Universal property of the empty set - Arbital](https://arbital.com/p/empty_set_universal_property/)

#### Theorem (Universal property of the empty set)

#### Proof

## Section 10, "Inverses and Composites"

> A correspondence between the elements of $X$ and the elements of $Y$
> does always induce a well-behaved correspondence between the subsets of
> $X$ and the subsets of $Y$, not forward, by the formation of images, but
> backward, by the formation of inverse images. Given a function $f$ from
> $X$ to $Y$, let $f^{-1}$, the *inverse* of $f$, be the function from
> $\mathscr{P}(Y)$ to $\mathscr{P}(X)$ such
> that if $B \subset Y$, then
>
> $f^{-1}(B) = \lbrace x \in X: f(x) \in B\rbrace.$
>
> In words: $f^{-1}(B)$ consists of exactly those elements of X that $f$ maps into $Y$;
> the set $f^{-1}(B)$ is called the *inverse image* of $B$ under $f$.
> A necessary and sufficient condition that $f$ map X onto $Y$ is that the inverse image
> under $f$ of each non-empty subset of $Y$ be a non-empty subset of $X$. (Proof?)
> A necessary and sufficient condition that $f$ be one-to-one is that the inverse
> image under $f$ of each singleton in the range of $f$ be a singleton in $X$.
>
> If the last condition is satisfied, then the symbol $f^{-1}$ is frequently 
> assigned a second interpretation, namely as the function whose domain is
> the range of $f$, and whose value for each $y$ in the range of $f$ is the unique
> $x$ in $X$ for which $f(x) = y$. In other words, for one-to-one functions $f$ we may write
> $f^{-1}(y)=x$ if and only if $f(x) = y$. This use of the notation is
> mildly inconsistent with our first interpretation of $f^{-1}$, but the double
> meaning is not likely to lead to any confusion.

> The discussion of inverses shows that what a function does can in a certain sense be undone;
> the next thing we shall see is that what two functions
> do can sometimes be done in one step. If, to be explicit, $f$ is a function
> from $X$ to $Y$ and $g$ is a function from $Y$ to $Z$, then every element in the
> range of $f$ belongs to the domain of $g$, and, consequently, $g(f(x))$ makes
> sense for each $x$ in $X$. The function $h$ from $X$ to $Z$, defined by
> $h(x) = g(f(x))$ is called the *composite* of the functions $f$ and $g$; it is denoted by
> $g \circ f$ or, more simply, by $gf$. (Since we shall not have occasion to consider
> any other kind of multiplication for functions, in this book we shall use
> the latter, simpler notation only.)
>
> Observe that the order of events is important in the theory of functional
> composition. In order that $gf$ be defined, the range of $f$ must be included
> in the domain of $g$, and this can happen without it necessarily happening
> in the other direction at the same time. Even if both $fg$ and $gf$ are defined,
> which happens if, for instance, $f$ maps $X$ into $Y$ and $g$ maps $Y$ into $X$, the
> functions $fg$ and $gf$ need not be the same; in other words, functional 
> composition is not necessarily commutative.
>
> Functional composition may not be commutative, but it is always
> associative. If $f$ maps $X$ into $Y$, if $g$ maps $Y$ into $Z$, and if
> $h$ maps $Z$ into $U$, then we can form the composite of $h$ with $gf$
> and the composite of $hg$ with $f$; it is a simple exercise to show that
> the result is the same in either case.
>
> The connection between inversion and composition is important; 
> something like it crops up all over mathematics. If $f$ maps $X$ into $Y$
> and $g$ maps $Y$ into $Z$, then $f^{-1}$ maps $\mathscr{P}(Y)$ into $\mathscr{P}(X)$
> and $g^{-1}$ maps $\mathscr{P}(Z)$ into $\mathscr{P}(Y)$. In this situation, the composites that
> are formable are $gf$ and $f^{-1}g^{-1}$; the assertion is that the latter is the inverse of the former.
> Proof: if $x \in (gf)^{-1}(C)$, where $x \in X$ and $C \subset Z$, then
> $g(f(x)) \in C$, so that $f(x) \in g^{-1}(C)$, and therefore
> $x \in f^{-1}(g^{-1}(C))$; the steps of the argument are reversible.