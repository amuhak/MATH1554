#matrix_multiplication 

|           Symbol          	|                          Meaning                          	|
|:-------------------------:	|:---------------------------------------------------------:	|
|           $\in$           	|                         belongs to                        	|
|       $\mathbb{R}^n$      	|       the set of vectors with n real-valued elements      	|
| $\mathbb{R}^{m \times n}$ 	| the set of real-valued matrices with m rows and n columns 	|

## Definition of Matrix Vector Multiplication
If $A \in \mathbb{R}^{m \times n}$ has vectors $\vec{a_1} , \dots , \vec{a_n}$ and $\vec{x} \in \mathbb{R}^{n},$ then the matrix Vector Product $A \vec{x}$ is a linear combination of the columns of $A$. It can be shown as shown:
$$A \vec{x} = \left( \matrix{| & | & \dots & | \\ \vec{a_1} & \vec{a_2} & \dots & \vec{a_n} \\ | & | & \dots & |} \right) \left( \matrix {x_1 \\ x_2 \\ \vdots \\ x_n}  \right) = x_1\vec{a_1} + x_2\vec{a_2} + \dots +x_n\vec{a_n} = \left( \matrix{ \vdots   \\ x_1\vec{a_1} + x_2\vec{a_2} + \dots +x_n\vec{a_n} \\  \vdots } \right)$$
**NOTE: $A \vec{x}$ is always in the span of $A$**

# Existence of Solutions

The equation $A \vec{x} = \vec{b}$ has a solution if and only if $\vec{b}$ is a linear combination of the columns of $A$.

### Example
$$\vec{b}=\left( \matrix {b_1 \\ b_2 \\ b_3}  \right)$$






