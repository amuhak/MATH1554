If $Q(x)$ is a function, then,$\newcommand\b[1]{\begin{bmatrix}#1\end{bmatrix}}$ 
$$
Q(\vec{x})=
\vec{x}^TA\vec{x}
$$
$A$ is [[Symmetric Matrices|symmetric]] 

# Examples
## Find $Q$
$Q(\vec{x})=\vec{x}^TA\vec{x}$, $A = \begin{bmatrix} 4 & 1 \\ 1 & -3 \end{bmatrix}$
$$
\b{x & y} \b{4 &1 \\ 1 &-3} \b{x \\ y} = 4x^2+2xy-3y^2
$$
The $2xy$ term is called a cross-product due to it having both variables. 

## Finding $A$
### $\mathbb{R}^2$
$Q=x^2-6xy+9y^2$
We will use our eyes, the main diagonal will be the coefficients for second order terms. The other diagonal will be $\frac{1}{2}$ of the coefficient of the cross-product.
So, $A = \b{1 &-3 \\ -3 & 9}$.
We could compute $\vec{x}^TA\vec{x}$ to verify this result.
### $\mathbb{R}^3$
$Q= 5x_1^2 - x_2^2 + 3x_3^3 + 6x_1x_3 - 12x_2x_3$
$Q= 5x_1^2 - x_2^2 + 3x_3^3 + 6x_1x_3 - 12x_2x_3 + 0 x_1x_2$
We will once again use our eye (consider resting them after this). Like last time the main diagonal will be the coefficients for second order terms. 