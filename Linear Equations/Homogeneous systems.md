Linear systems of the form $A\mathbf{x}=\mathbf{0}$ are homogeneous.
Linear systems of the form $A\mathbf{x}=\mathbf{b}$ where $\mathbf{b} \neq \mathbf{0},$ are inhomogeneous.

Here the **trivial**/**nontrivial** refers to $\mathbf{x}$. 
If $\mathbf{x}=\left[ \matrix{0 \\ 0 \\ \vdots \\ 0} \right]$ it is **trivial** solution. Otherwise it is **nontrivial**

# Observations
![[Homogeneous systems.png|500]]

# Example
Identify the free variables, and the solution set, of the system.
![[Homogeneous systems-1.png|400]]
In [[Echelon Form]]: 
$$\left[ \begin{array}{ccc|c} 1 &0&-2&0 \\ 0&1&1&0 \\ 0 &0&0&0 \end{array} \right]$$
$$ \array{
x_1 + -2x_3 = 0 \\
x_2+x_3=0 \\
0=0
}
$$
$$ \array{
x_1 = 2x_3 \\
x_2=-x_3 \\
x_3 = x_3
}
$$
$$\text{Solution set} = \textbf{x}= \left[ \array{2x_3 \\ -x_3 \\ x_3} \right] = x_3\left[ \array{2 \\ -1 \\ 1} \right]$$

