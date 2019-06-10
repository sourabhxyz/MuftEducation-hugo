+++
title = "Cyclic Groups"
weight = 6
pre = "<b> </b>"
+++

**Example** The set $Z\_n = \\{0, 1, . . . , n - 1\\}$ for $n \geq 1$ is a cyclic group under addition modulo $n$. Again (was in case for group $Z$), 1 and -1 = n - 1 are generators.

**Example** $Z\_8 = <1> = <3> = <5> = <7>$.

**Theorem 4.1:** Let $G$ be a group, and let $a$ belong to $G$. If $a$ has infinite order, then $a\_i = a\_j$ if and only if $i = j$. If $a$ has finite order, say, $n$, then $< a > = \\{e, a, a^2, . . . , a^{n-1}\\}$ and $a\_i = a\_j$ if and only if $n$ divides $i - j$. (Easy to prove)

**Corollary** For any group element $a$, $|a| = |< a >|$.

**Corollary** $a^k = e$ Implies That $|a|$ Divides $k$.

What is important about Theorem 1 in the finite case is that it says that multiplication in $< a >$ is essentially done by addition modulo $n$. That is, if $(i+j) \bmod n = k$, then $a^ia^j = a^k$.

Thus, no matter what group $G$ is, or how the element $a$ is chosen, multiplication in $< a >$ works the same as addition in $Z\_n$ whenever $|a| = n$. Similarly, if $a$ has infinite order, then multiplication in $< a >$ works the same as addition in $Z$, since $a^ia^j = a^{i+j}$ and no modular arithmetic is done.
For these reasons, the cyclic groups $Z\_n$ and $Z$ serve as prototypes for all cyclic groups, and algebraists say that there is essentially only one cyclic group of each order.

**Theorem 4.2:** let $a$ be an element of order $n$ in a group and let $k$ be a positive integer. Then kakl 5 kagcd(n,k)l and |ak| 5 n/gcd(n, k).
