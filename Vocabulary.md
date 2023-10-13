|           Word          	|                          Meaning                          	|
|:-------------------------:	|---------------------------------------------------------|
| Consistent | If it has at least one solution.|
| Row equivalent | If a sequence of row operations transforms one matrix into the other.|
| Unique solution | If and only if there are no free variables 	|
| Homogeneous | Linear systems of the form $A\mathbf{x}=\mathbf{0}$ |
| Inhomogeneous | Linear systems of the form $A\mathbf{x}=\mathbf{b}$ where $\mathbf{b} \neq \mathbf{0}$ |
| Trivial solution | The solution is the zero vector |
| Linearly independent | If no vector can be made from other vectors |
| Row operations | Addition, Interchange, Scaling |
| Pivot position | A leading 1 in the RREF of A |
| Pivot column | Is a column of A that contains a pivot position |
| Domain | $T: \mathbb{R}^n$ $\rightarrow \mathbb{R}^m$; $\mathbb{R}^n$ is the domain of $T$ |
| Codomain | $T: \mathbb{R}^n$ $\rightarrow \mathbb{R}^m$; $\mathbb{R}^m$ is the codomain of $T$ |
| Image | The vector $T(\vec{x})$ is the image of $\vec{x}$ under $T$ |
| Range | The set of all possible images $T(\vec{x})$ or simply the **span of A** |
| Standard vectors| The column of the identity matrix (think $\begin{bmatrix}1 \\ 0\end{bmatrix}$ and $\begin{bmatrix} 0 \\ 1\end{bmatrix}$)|
| Onto | All the elements in the codomain are mapped to. (A spans the entire codomain), Every **row** is pivotal |
| One-To-One | Each mapping is unique (2 vectors can **NOT** map to the same vector), Every **column** is pivotal|
| Transpose | The matrix whose columns are the rows of $A$ |
| Invertible | $A \in \mathbb{R}^{n \times n}$ is invertible if there is a $C \in \mathbb{R}^{n \times n}$ such that: $AC=CA=I_n$ |
| Elementary Matrix | Differs from $I_n$ by one row operation. |
| Singular | A matrix that is not invertible ($A^{-1}$ DNE)|
| Subset | A subset of $\mathbb{R}^n$ any collection of vectors that are in $\mathbb{R}^n$ |
| Subspace | If $H \in \mathbb{R}^n$, for $c \in \mathbb{R}$ and $\vec{u},\vec{v} \in H$, $c\vec{u} \in H$ and $\vec{u}+\vec{v} \in H$ must be true if $H$ is a subspace. |
| Column Space | This is a subspace spanned by the column of $A$. |
| Null Space | This is a subspace spanned by all $\vec{x}$ such that $A\vec{x}=\vec{0}$. |
| Basis | This is a set of linearly independent vectors in $H$ that spans $H$ assuming $H$ is a subspace.|
| Coordinate Vector | These are the vectors that are used to describe the coordinate systems. |
| Coordinates | These are the weights of the coordinate vector used to describe the point.  |
| Dimension | This is the number of vectors in a basis of $H$. |
| Cardinality | Same thing as Dimension |
| Rank | $\text{Rank} (A)=\text{dim}(\text{Col} (A) ) = \text{no of pivot columns}$ |
| Determinant | It is the scaling factor that tells us how a transformation will change the area or volume of a region. |
| Probability Vector | A vector with non-negative elements that sum to $1$ |
| Stochastic Matrix | Square matrix, $P$, whose columns are probability vectors. |
| Markov Chain | The sequence: $\vec{x_{k+1}} = P \vec{x_k}$ ($0 \leq k$) |
| Steady-State Vector | Is the a probability vector such that $P\vec{q}=\vec{q}$ |
| Regular Stochastic Matrix | If there is some $k$ such that $P^k$ only contains positive entries. |
| Trace | The sum of the elements of the main diagonal. |
| Characteristic Polynomial | $\det(A-\lambda I)$ |
| Characteristic Equation | $\det(A-\lambda I)=0$ |
| Multiplicity | The number of times that its associated factor appears in the polynomial. |
| Algebraic Multiplicity | Multiplicity of the characteristic polynomial. |
| Geometric Multiplicities | Dimentions of $\text{Null}{(A-\lambda I)}$  |
