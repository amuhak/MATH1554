Consider the augmented matrix:
![[Pasted image 20230822105608.png]]
### The leading one's are in first, third, and fifth columns.
- The pivot columns (leading ones) of A are the first, third, and fifth columns
- The corresponding variables of the system $A \vec{x}= \vec{b}$. are $x_1, x_2, \text{and} x_5$ Variables that correspond to a pivot are basic variables.
- Variables that are not basic are free variables. They can take any value.
- The free variables are $x_2$ and $x_4$. Any choice of the free variables leads to a solution of the system.

**Unique solution** exists if and only if there are no free variables.

A linear system is **consistent** if it has at least one solution.

## Note
If you see something like this (b is a non-zero number): 
$$
\left( \begin{array}{ccccc|c} 0 & 0 & 0 & ... & 0 & b \end{array} \right)
$$
~~RUN~~ you **don't** have a [[Consistent Systems|Consistent System]]. 