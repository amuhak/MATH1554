#matrix_multiplication 

|           Symbol          	|                          Meaning                          	|
|:-------------------------:	|:---------------------------------------------------------:	|
|           $\in$           	|                         belongs to                        	|
|       $\mathbb{R}^n$      	|       the set of vectors with n real-valued elements      	|
| $\mathbb{R}^{m \times n}$ 	| the set of real-valued matrices with m rows and n columns 	|

## Definition of Matrix Vector Multiplication
If $A \in \mathbb{R}^{m \times n}$ has vectors $\mathbf{a_1} , \dots , \mathbf{a_n}$ and $\mathbf{x} \in \mathbb{R}^{n},$ then the matrix Vector Product $A \mathbf{x}$ is a linear combination of the columns of $A$. It can be shown as shown:
$$A \mathbf{x} = \left[ \matrix{| & | & \dots & | \\ \mathbf{a_1} & \mathbf{a_2} & \dots & \mathbf{a_n} \\ | & | & \dots & |} \right] \left[ \matrix {x_1 \\ x_2 \\ \vdots \\ x_n}  \right] = x_1\mathbf{a_1} + x_2\mathbf{a_2} + \dots +x_n\mathbf{a_n} = \left[ \matrix{ \vdots   \\ x_1\mathbf{a_1} + x_2\mathbf{a_2} + \dots +x_n\mathbf{a_n} \\  \vdots } \right]$$
**NOTE: $A \mathbf{x}$ is always in the span of $A$**

# Existence of Solutions

The equation $A \mathbf{x} = \mathbf{b}$ has a solution if and only if $\mathbf{b}$ is a linear combination of the columns of $A$.

### Example
For what vectors $\mathbf{b}=\left[ \matrix {b_1 \\ b_2 \\ b_3}  \right]$ does the equation have a solution?

$$\left[ \begin{array}{ccc|c}1 &3&4&b_1\\2&8&4&b_2\\0&1&-2&b_3 \end{array} \right]$$
$$\left[ \begin{array}{ccc|c} 1 & 3 & 4 & b_1 \\ 0 & 2 & -4 & b_2-2b_1 \\ 0 & 0 & 0 & b_3- \frac{1}{2}b_2 + b_1\\ \end{array} \right]$$
Solving for $b_1$ from the last row,
$$b_1=\frac{1}{2}-b_3$$
$$\boxed{\mathbf{b}=\left[ \array{\frac{1}{2}-b_3 \\ b_2 \\ b_3} \right]}$$
