---
layout: default
---
{%- include mathjax.html -%}
In these notes we will discuss the basic properties of sequences and convergence. To begin, we present some basic definitions.

**Definition** (Metric): A metric, $d$, is a function that takes two elements of a set and returns a real number and which satisfies three properties:

1. $d(x,y) = d(y,x),$ for any $x,y \in X$
2. $d(x,y) = 0 \iff x = y$, for any $x,y \in X$
3. $d(x,z) \leq d(x,y) + d(y,z)$ for any $x,y,z \in X.$

**Definition** (Metric Space): A metric space is a pairing of a set and a metric, usually written as $(X,d)$, for a set $X$ and a metric $d : X \times X \to \mathbb{R}.$ 

**Definition** (Sequence): Let $S$ be a countable set and $X$ a set. A sequence is a subset $\{a_j\}_{j \in S} \subset X.$ Usually, $S$ is chosen to be $\mathbb{N}$ for ordinary sequences. 

**Definition** (Convergence of a Sequence): Let $(a_j) \subset X$. If there exists some element $a \in X$ such that for all $\epsilon > 0$, there exists some $N \in \mathbb{N}$, $d(a_n,a) < \epsilon$ for $n > N$, we say that $(a_n)$ converges to $a$ with respect to $d.$ This is written as $(a_n) \xrightarrow{n \to \infty} a.$

**Definition** (Limit): If $(a_n) \to a$, we call $a$ the limit of $(a_n)$.

We can now prove a basic fact about sequences.

**Proposition** (Uniqueness of Limit): Suppose $(a_n) \to a \in X,$ then $(a_n)$ does not converge to any other $a' \in X.$

*Proof*. Suppose that $(a_n) \to b$ and $(a_n) \to c$. Note that because we assume $b \neq c,$ we have that $d(b,c) = C > 0$. Thus, if we take $\epsilon > 0$ so that $0 < \epsilon < C/2$, we can find $N_1$ and $N_2$ large enough so that for $n > \max_i N_i$, $d(a_n,b) < \epsilon$ and $d(a_n,c) < \epsilon.$ This implies that

$$d(b,c) = d(b,a_n) + d(c,a_n) < \dfrac{C}{2} + \dfrac{C}{2} = C,$$

which is, of course, a contradiction. 
