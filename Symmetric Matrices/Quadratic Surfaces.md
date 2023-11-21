# Curves in $\mathbb{R}^2$
Say we have a constant $C$ and $Q(x)=x^TAx$ where $A\in\mathbb{R}^{2 \times2}$. Then,$\newcommand\b[1]{\begin{bmatrix}#1\end{bmatrix}}$
$$C=x^TAx$$
Is a curve in $\mathbb{R}^2$.
Say $A=\b{2&1\\1&2}$. Then $Q(x)=2x^2+2y^2+2xy=C$.
If $C=1$ we can plot, 
![[Quadratic Surfaces-1.png|400]]
Here is it plotted when we changed $C$ from 1 to 10.
![[animation.gif|300]]

# Curves in $\mathbb{R}^3$
Say we have $z=Q(x)$ , $z=x^2+y^2=x^T\b{1&0\\0&1}x$ 
We can graph this,
![[animation1.gif]]
# Definitions
| Word | Definition |
|----|-----|
| Positive Definite | If $Q>0$ for all $\vec{x} \ne 0$ |
| Negative Definite | If $Q<0$ for all $\vec{x} \ne 0$ |
| Positive Semidefinite | If $Q \ge 0$ for all $\vec{x}$ |
| Negative Semidefinite | If $Q \le 0$ for all $\vec{x}$ |
| Indefinite | If $Q$ takes on positive and negative values for $\vec{x} \ne 0$ |
