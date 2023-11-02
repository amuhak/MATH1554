Given n [[Linear Independence|linearly independent]] vectors that form the subspace $W$, you can use the Gram-Schmidt Process to find the orthogonal basis for $W$.

# $2$ Vectors  
We take one of the 2 vectors and find its 'z' using the other vector. Now this new vector and 'other' vector are the new orthogonal basis. As math:
Given the linearly independent vectors: $\vec{v},\vec{u}$ the orthogonal basis is $\{\vec{v},\vec{u}-\text{Proj}_\vec{v}{\vec{u}}\}$.

More formally, given the linearly independent vectors: $\vec{x_1},\vec{x_2}$,
$$
\begin{aligned}
\vec{v_1}&=\vec{x_1}\\
\vec{v_2}&=\vec{x_2}-\frac{\vec{x_2} \cdot\vec{x_1}}{\vec{x_1} \cdot \vec{x_1}} \vec{x_1}
\end{aligned}
$$
Then the set $\{ \vec{v_1},\vec{v_2} \}$ is the orthogonal basis.

# n-Vectors
Given the linearly independent vectors: $\vec{x_1},\vec{x_2}, \dots, \vec{x_n}$
$$
\begin{aligned}
\vec{v_1}&=\vec{x_1}  & W_1=\text{Span}\{ v_1 \}\\
\vec{v_2}&=\vec{x_2}-\text{Proj}_{W_1}{\vec{x_2}} & W_2=\text{Span}\{ v_1,v_2 \}\\
\vec{v_3}&=\vec{x_3}-\text{Proj}_{W_2}{\vec{x_3}} & W_3=\text{Span}\{v_1,v_2,v_3\}\\
\vdots & & \vdots\\
\vec{v_n}&=\vec{x_n}-\text{Proj}_{W_{n-1}}{\vec{x_n}} & W_n=\text{Span}\{v_1,\dots,v_n\}\\
\end{aligned}
$$
The orthogonal basis will be $\{ \vec{v_1},\vec{v_2}, \dots \vec{v_n} \}$
We will use the Orthogonal Decomposition Theorem that can be found in [[Orthogonality/Formulas|Formulas]]
