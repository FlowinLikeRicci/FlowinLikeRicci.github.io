---
layout: default
---
{%- include mathjax.html -%}
In these notes we will discuss the basic properties of sequences and convergence. To begin, we present some basic definitions.

*Definition* (metric): A metric, $d$, is a function that takes two elements of a set and returns a real number and which satisfies three properties:

1. $d(x,y) = d(y,x),$ for any $x,y \in X$
2. $d(x,y) = 0 \iff x = y$, for any $x,y \in X$
3. $d(x,y) + d(y,z) \leq d(x,z)$ for any $x,y,z \in X.$ 
