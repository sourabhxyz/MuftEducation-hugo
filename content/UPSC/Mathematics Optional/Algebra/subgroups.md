+++
title = "Subgroups"
weight = 5
pre = "<b> </b>"
+++

**Definition: (Order of a group)** The number of elements of a group (finite or infinite) is called its order. We will use $\vert G \vert$ to denote the order of G.

**Definition: (Order of an element)** The order of an element $g$ in a group $G$ is the smallest positive integer $n$ such that $g^n = e$. (In additive notation, this would mean $ng = 0$.) If no such integer exists, we say that $g$ has infinite order. The order of an element $g$ is denoted by $\vert g \vert$

**Example:** Consider U(15) = {1, 2, 4, 7, 8, 11, 13, 14} under multiplication modulo 15. This group has order 8. $\vert 13 \vert$? Soln: Compute $13^1, 13^2, 13^3, 13^4$ to get answer as 4, however there is trick: $13 = -2 \bmod 15 \Rightarrow 13^2 = (-2)^2 = 4, 13^3 = -2 \cdot 4 = -8, 13^4 = (-2)(-8) = 1.$

**Example:** Consider $Z$ under ordinary addition. Here every nonzero element has infinite order, since the sequence $a, 2a, 3a, \dots$ never includes 0 when $a \neq 0$.

**Definition: (Subgroup)** If a subset $H$ of a group $G$ is itself a group under the operation of $G$, we say that $H$ is a subgroup of $G$.

We use the notation $H \leq G$ to mean that $H$ is a subgroup of $G$. If we want to indicate that $H$ is a subgroup of $G$ but is not equal to $G$ itself, we write $H < G$. Such a subgroup is called a proper subgroup. The subgroup ${e}$ is called the trivial subgroup of $G$; a subgroup that is not ${e}$ is called a nontrivial subgroup of G.

When determining whether or not a subset $H$ of a group $G$ is a subgroup of G, one need not directly verify the group axioms as it will become evident from discussion below. 

**Theorem 1: (One-Step Subgroup Test)**
Let $G$ be a group and $H$ a nonempty subset of $G$. If $ab^{-1}$ is in $H$ whenever $a$ and $b$ are in $H$, then $H$ is a subgroup of $G$. (In additive notation, if $a - b$ is in $H$ whenever $a$ and $b$ are in $H$, then $H$ is a subgroup of $G$.)

**Proof:** Since the operation of $H$ is the same as that of $G$, it is clear that this operation is associative. Next, we show that $e$ is in $H$. Since $H$ is nonempty, we may pick some $x$ in H. Then, letting $a = x$ and $b = x$ in the hypothesis, we have $e = xx^{-1} = ab^{-1}$ is in $H$. To verify that $x^{-1}$ is in $H$ whenever $x$ is in $H$, all we need to do is to choose $a = e$ and $b = x$ in the statement of the theorem. Finally, the proof will be complete when we show that $H$ is closed; that is, if $x, y$ belong to $H$, we must show that $xy$ is in $H$ also. Well, we have already shown that $y^{-1}$ is in $H$ whenever $y$ is; so,letting $a = x$ and $b = y^{-1}$, we have $xy = x(y^{-1})^{-1} = ab^{-1}$ is in $H$.

To apply the above theorem, follow these steps:-

1. Identify the property $P$ that distinguishes the elements of $H$; that is, identify a defining condition.
2. Prove that the identity has property $P$. (This verifies that $H$ is nonempty.)
3. Assume that two elements $a$ and $b$ have property $P$.
4. Use the assumption that $a$ and $b$ have property $P$ to show that $ab^{-1}$ has property $P$.

**Example (easy):** Let $G$ be an Abelian group under multiplication with identity $e$. Then $H = \\{x^2 \vert x \in G\\}$ is a subgroup of $G$. Since $e^2 = e$, the identity has the correct form. Next, we write two elements of $H$ in the correct form, say, $a^2$ and $b^2$. We must show that $a^2(b^2)^{-1}$ also has the correct form; that is, $a^2(b^2)^{-1}$ is the square of some element. Since $G$ is Abelian, we may write it as $(ab^{-1})^2$, which is the correct form. Thus, $H$ is a subgroup of $G$.

**Theorem 2: (Two-Step Subgroup Test)**
Let $G$ be a group and let $H$ be a nonempty subset of $G$. If $ab$ is in $H$ whenever $a$ and $b$ are in $H$ ($H$ is closed under the operation), and $a^{-1}$ is in $H$ whenever $a$ is in $H$ ($H$ is closed under taking inverses), then $H$ is a subgroup of $G$.

**Proof:**
By Theorem 1, it suffices to show that $a, b \in H$ implies $ab^{-1} \in H$. So, we suppose that $a, b \in H$. Since $H$ is closed under taking inverses, we also have $b^{-1} \in H$. Thus, $ab^{-1} \in H$ by closure under multiplication.

{{% notice note %}}
A notice disclaimer
{{% /notice %}}