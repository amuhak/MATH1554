#matrix_multiplication 

Let $A$ be a $m \times n$ matrix, and $B$ be a $n \times p$ matrix. The product is $AB$ an $m \times p$ matrix, equal to:
$$AB=A\left( \mathbf{b_1} \  \dots \ \mathbf{b_p} \right) = \left( A\mathbf{b_1} \ \dots \ A\mathbf{b_p}  \right) $$
$$
\begin{aligned}
AB &= \left[ \begin{array}  \\ 1 & 0\\1&1 \end{array} \right] \left[ \begin{array}  \\ 2 & 0 &0\\3&4&0 \end{array} \right] \\
&=\left( \left[ \begin{array}  \\ 1 & 0\\1&1 \end{array} \right] \left[ \begin{array}  \\ 2 \\ 3\end{array} \right] \ \ \ \ \left[ \begin{array}  \\ 1 & 0\\1&1 \end{array} \right] \left[ \begin{array} \\ 0 \\4 \end{array} \right] \ \ \ \  \left[ \begin{array}  \\ 1 & 0\\1&1 \end{array} \right] \left[ \begin{array} \\0\\0 \end{array} \right] \right)\\
&=\left[ \begin{array} \\ 2&0&0\\5&4&0 \end{array} \right]
\end{aligned}
$$
(Note: This is very similar to [[Matrix Vector Product]])
![[Matrix Multiplication.png]]

# Important! 
![[Matrix Multiplication-1.png]]

