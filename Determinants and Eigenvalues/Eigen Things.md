If $A \in \mathbb{R}^{n \times n}$, and there is a $\vec{v} \ne 0 \in \mathbb{R}^n$, and 
$$A\vec{v}=\lambda \vec{v}$$
Then $\vec{v}$ is an **eigenvectors** for A, and $\lambda$ is the **eigenvalue**. 

# Eigenspaces
The span of the eigenvector of $A$ is the eigenspace of $A$. It spans a subspace of $\mathbb{R}^n$ called the $\lambda$-eigenspace of $A$.

The $\lambda$-eigenspace of $A$ is $\text{Nul}{(A-\lambda I)}$ 
$$
\begin{aligned}
A\vec{v}&=\lambda\vec{v}\\
A\vec{v}-\lambda\vec{v}&=0\\
(A-\lambda I)\vec{v}&=0
\end{aligned}
$$
# Theorems
- The diagonal elements of a triangular matrix are its eigenvalues.
- A not invertible $\Longleftrightarrow$ 0 is an eigenvalue of A.
- Stochastic matrices have an eigenvalue equal to 1.
- Eigenvectors with distinct eigenvalues are  linearly independent vectors.

# Compute Eigenvalues
We know that $(A-\lambda I)$ is non invertible, so $\det(A-\lambda I)=0$.
We can solve $\det(A-\lambda I)=0$ for $\lambda$.

$\det(A-\lambda I)$ is the characteristic polynomial
$\det(A-\lambda I)=0$ is the characteristic equation
The **trace** of a matrix is the sum of its diagonal elements.
The sum of the Eigenvalues of $A$ = the trace.

# Algebraic and Geometric Multiplicities
