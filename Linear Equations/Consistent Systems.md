## Augmented Matrices
This:
$$
\begin{equation}
    \begin{cases}
	x_1-2x_2+x_3=0 \\
		2x_2-8x_3=7
    \end{cases}
\end{equation}
$$
Becomes:
$$\left( \begin{array}{ccc|c} 1 & -2 & 1 & 0 \\ 0 & 2 & -8 & 7 \\ \end{array} \right)$$
A linear system is **consistent** if it has at least one solution.
Two matrices are **row equivalent** if a sequence of row operations transforms one matrix into the other.

![[Pasted image 20230822082952.png]]
A and B are row equivalent
A and C are not row equivalent
![[Pasted image 20230822083132.png]]
$$\left( \begin{array}{c|c} A & \vec{b} \end{array} \right) =\left( \begin{array}{cc|c} 1 & 1 & 1 \\ 0 & 1 & 1 \\ \end{array} \right)$$
$$\left( \begin{array}{c|c} A & \vec{b} \end{array} \right) =\left( \begin{array}{cc|c} 1 & 0 & 0 \\ 0 & 1 & 1 \\ \end{array} \right)$$
So A and $\vec{b}$ are consitent.
A and C are not consitent.