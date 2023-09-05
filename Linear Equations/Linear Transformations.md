$$
\begin{equation} T: R^n \to R^m \text{ is linear if } \begin{cases} T(u + v) &= T(u) + T(v) \\ T(cv) &= cT(v) \end{cases} \end{equation}
$$

Create a $2\times2$ matrix $A$ that applies a linear transformation that rotates by an angle $\theta$ counterclockwise 

$$
\begin{align*}
A &=[\vec{a_1},\vec{a_2}] \\
T(\vec{e_1}) &= \vec{a_1} \\
T(\vec{e_1}) &= \begin{bmatrix} a \\ b \end{bmatrix} &= \begin{bmatrix}\cos{ \theta} \\ \sin{ \theta} \end{bmatrix} \\
\vec{a_1} &= \begin{bmatrix}\cos{ \theta} \\ \sin{ \theta} \end{bmatrix} \\
T(\vec{e_2}) &= \vec{a_2} \\
T(\vec{e_2}) &= \begin{bmatrix} a \\ b \end{bmatrix} &= \begin{bmatrix} -\sin{ \theta} \\ \cos{ \theta}\end{bmatrix} \\
\vec{a_2} &= \begin{bmatrix} -\sin{ \theta} \\ \cos{ \theta}\end{bmatrix} \\
\end{align*}
$$
$$
\boxed 
{A = \begin{bmatrix} \cos{ \theta} & -\sin{ \theta} \\ \sin{ \theta}  & \cos{ \theta} \end{bmatrix}}
$$

# Geometric Transformations
## Reflections
### Through $x_1-\text{axis}$ 
$$
T ( \begin{bmatrix} 1 \\ 1  \end{bmatrix} ) =  \begin{bmatrix} 1 \\ -1  \end{bmatrix} 
$$
So,
$$A = \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}$$
### Through $x_2-\text{axis}$ 
$$
T ( \begin{bmatrix} 1 \\ 1  \end{bmatrix} ) = \begin{bmatrix} -1 \\ 1  \end{bmatrix}
$$
So,
$$A = \begin{bmatrix} -1 & 0 \\ 0 & 1 \end{bmatrix}$$
### Through $x_2=x_1$ 
$$
\begin{aligned}
T ( \begin{bmatrix} 1 \\ 0 \end{bmatrix} ) &= \begin{bmatrix} 0 \\ 1 \end{bmatrix}\\
T ( \begin{bmatrix} 0 \\ 1 \end{bmatrix} ) &= \begin{bmatrix} 1 \\ 0 \end{bmatrix}
\end{aligned}
$$
So,
$$A = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}$$
### Through $x_2=-x_1$ 
$$
\begin{aligned}
T ( \begin{bmatrix} 1 \\ 0 \end{bmatrix} ) &= \begin{bmatrix} 0 \\ -1 \end{bmatrix}\\
T ( \begin{bmatrix} 0 \\ 1 \end{bmatrix} ) &=  \begin{bmatrix} -1 \\ 0 \end{bmatrix} 
\end{aligned}
$$

So,
$$A = \begin{bmatrix} 0 & -1 \\ -1 & 0 \end{bmatrix}$$
## Contractions and Expansions
### Horizontal
#### Contractions (${|k|}<1$)

$$
\begin{aligned}
T ( \begin{bmatrix} 1 \\ 0 \end{bmatrix} ) &=  \begin{bmatrix} k \\ 0 \end{bmatrix} \\
T ( \begin{bmatrix} 0 \\ 1 \end{bmatrix} ) &=  \begin{bmatrix} 0 \\ 1 \end{bmatrix} 
\end{aligned}
$$
So,
$$A = \begin{bmatrix} k & 0 \\ 0 & 1 \end{bmatrix}$$
#### Expansions(${|k|}>1$)

$$
\begin{aligned}
T ( \begin{bmatrix} 1 \\ 0 \end{bmatrix} ) &=  \begin{bmatrix} k \\ 0 \end{bmatrix} \\
T ( \begin{bmatrix} 0 \\ 1 \end{bmatrix} ) &=  \begin{bmatrix} 0 \\ 1 \end{bmatrix} 
\end{aligned}
$$

So,
$$A = \begin{bmatrix} k & 0 \\ 0 & 1 \end{bmatrix}$$
### Vertical
#### Contractions (${|k|}<1$)

$$
\begin{aligned}
T ( \begin{bmatrix} 1 \\ 0 \end{bmatrix} ) &=  \begin{bmatrix} 1 \\ 0 \end{bmatrix} \\
T ( \begin{bmatrix} 0 \\ 1 \end{bmatrix} ) &=  \begin{bmatrix} 0 \\ k \end{bmatrix} 
\end{aligned}
$$
So,
$$A = \begin{bmatrix} 1 & 0 \\ 0 & k \end{bmatrix}$$
#### Expansions(${|k|}>1$)

$$
\begin{aligned}
T ( \begin{bmatrix} 1 \\ 0 \end{bmatrix} ) &=  \begin{bmatrix} 1 \\ 0 \end{bmatrix} \\
T ( \begin{bmatrix} 0 \\ 1 \end{bmatrix} ) &=  \begin{bmatrix} 0 \\ k \end{bmatrix} 
\end{aligned}
$$
So,
$$A = \begin{bmatrix} 1 & 0 \\ 0 & k \end{bmatrix}$$

## Shears
### Horizontal Shear
#### Left($k<0$)
$$
\begin{aligned}
T ( \begin{bmatrix} 1 \\ 0 \end{bmatrix} ) &=  \begin{bmatrix} 1 \\ 0 \end{bmatrix} \\
T ( \begin{bmatrix} 0 \\ 1 \end{bmatrix} ) &=  \begin{bmatrix} k \\ 1 \end{bmatrix} 
\end{aligned}
$$
So,
$$A = \begin{bmatrix} 1 & k \\ 0 & 1 \end{bmatrix}$$
#### Right($k>0$)
$$
\begin{aligned}
T ( \begin{bmatrix} 1 \\ 0 \end{bmatrix} ) &=  \begin{bmatrix} 1 \\ 0 \end{bmatrix} \\
T ( \begin{bmatrix} 0 \\ 1 \end{bmatrix} ) &=  \begin{bmatrix} k \\ 1 \end{bmatrix} 
\end{aligned}
$$
So,
$$A = \begin{bmatrix} 1 & k \\ 0 & 1 \end{bmatrix}$$

### Vertical Shear
#### Down($k<0$)
$$
\begin{aligned}
T ( \begin{bmatrix} 1 \\ 0 \end{bmatrix} ) &=  \begin{bmatrix} 1 \\ k \end{bmatrix} \\
T ( \begin{bmatrix} 0 \\ 1 \end{bmatrix} ) &=  \begin{bmatrix} 0 \\ 1 \end{bmatrix} 
\end{aligned}
$$
So,
$$A = \begin{bmatrix} 1 & 0 \\ k & 1 \end{bmatrix}$$
#### Up($k>0$)

$$
\begin{aligned}
T ( \begin{bmatrix} 1 \\ 0 \end{bmatrix} ) &=  \begin{bmatrix} 1 \\ k \end{bmatrix} \\
T ( \begin{bmatrix} 0 \\ 1 \end{bmatrix} ) &=  \begin{bmatrix} 0 \\ 1 \end{bmatrix} 
\end{aligned}
$$
So,
$$A = \begin{bmatrix} 1 & 0 \\ k & 1 \end{bmatrix}$$
## Projections
### On to the $x_1-\text{Axis}$
$$
\begin{aligned}
T ( \begin{bmatrix} 1 \\ 0 \end{bmatrix} ) &=  \begin{bmatrix} 1 \\ 0 \end{bmatrix} \\
T ( \begin{bmatrix} 0 \\ 1 \end{bmatrix} ) &=  \begin{bmatrix} 0 \\ 0 \end{bmatrix} 
\end{aligned}
$$
So,
$$A = \begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix}$$
