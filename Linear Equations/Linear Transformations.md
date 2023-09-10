$$
\begin{equation} T: R^n \to R^m \text{ is linear if } \begin{cases} T\left(u + v\right) &= T\left(u\right) + T\left(v\right) \\ T\left(cv\right) &= cT\left(v\right) \end{cases} \end{equation}
$$

Create a $2\times2$ matrix $A$ that applies a linear transformation that rotates by an angle $\theta$ counterclockwise 

$$
\begin{align*}
A &=[\vec{a_1},\vec{a_2}] \\
T\left(\vec{e_1}\right) &= \vec{a_1} \\
T\left(\vec{e_1}\right) &= \begin{bmatrix} a \\ b \end{bmatrix} &= \begin{bmatrix}\cos{ \theta} \\ \sin{ \theta} \end{bmatrix} \\
\vec{a_1} &= \begin{bmatrix}\cos{ \theta} \\ \sin{ \theta} \end{bmatrix} \\
T\left(\vec{e_2}\right) &= \vec{a_2} \\
T\left(\vec{e_2}\right) &= \begin{bmatrix} a \\ b \end{bmatrix} &= \begin{bmatrix} -\sin{ \theta} \\ \cos{ \theta}\end{bmatrix} \\
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
T \left( \begin{bmatrix} 1 \\ 1  \end{bmatrix} \right) =  \begin{bmatrix} 1 \\ -1  \end{bmatrix} 
$$
So,
$$A = \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}$$
### Through $x_2-\text{axis}$ 
$$
T \left( \begin{bmatrix} 1 \\ 1  \end{bmatrix} \right) = \begin{bmatrix} -1 \\ 1  \end{bmatrix}
$$
So,
$$A = \begin{bmatrix} -1 & 0 \\ 0 & 1 \end{bmatrix}$$
### Through $x_2=x_1$ 
$$
\begin{aligned}
T \left( \begin{bmatrix} 1 \\ 0 \end{bmatrix} \right) &= \begin{bmatrix} 0 \\ 1 \end{bmatrix}\\
T \left( \begin{bmatrix} 0 \\ 1 \end{bmatrix} \right) &= \begin{bmatrix} 1 \\ 0 \end{bmatrix}
\end{aligned}
$$
So,
$$A = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}$$
### Through $x_2=-x_1$ 
$$
\begin{aligned}
T \left( \begin{bmatrix} 1 \\ 0 \end{bmatrix} \right) &= \begin{bmatrix} 0 \\ -1 \end{bmatrix}\\
T \left( \begin{bmatrix} 0 \\ 1 \end{bmatrix} \right) &=  \begin{bmatrix} -1 \\ 0 \end{bmatrix} 
\end{aligned}
$$

So,
$$A = \begin{bmatrix} 0 & -1 \\ -1 & 0 \end{bmatrix}$$
## Contractions and Expansions
### Horizontal
#### Contractions \left(${|k|}<1$\right)

$$
\begin{aligned}
T \left( \begin{bmatrix} 1 \\ 0 \end{bmatrix} \right) &=  \begin{bmatrix} k \\ 0 \end{bmatrix} \\
T \left( \begin{bmatrix} 0 \\ 1 \end{bmatrix} \right) &=  \begin{bmatrix} 0 \\ 1 \end{bmatrix} 
\end{aligned}
$$
So,
$$A = \begin{bmatrix} k & 0 \\ 0 & 1 \end{bmatrix}$$
#### Expansions\left(${|k|}>1$\right)

$$
\begin{aligned}
T \left( \begin{bmatrix} 1 \\ 0 \end{bmatrix} \right) &=  \begin{bmatrix} k \\ 0 \end{bmatrix} \\
T \left( \begin{bmatrix} 0 \\ 1 \end{bmatrix} \right) &=  \begin{bmatrix} 0 \\ 1 \end{bmatrix} 
\end{aligned}
$$

So,
$$A = \begin{bmatrix} k & 0 \\ 0 & 1 \end{bmatrix}$$
### Vertical
#### Contractions \left(${|k|}<1$\right)

$$
\begin{aligned}
T \left( \begin{bmatrix} 1 \\ 0 \end{bmatrix} \right) &=  \begin{bmatrix} 1 \\ 0 \end{bmatrix} \\
T \left( \begin{bmatrix} 0 \\ 1 \end{bmatrix} \right) &=  \begin{bmatrix} 0 \\ k \end{bmatrix} 
\end{aligned}
$$
So,
$$A = \begin{bmatrix} 1 & 0 \\ 0 & k \end{bmatrix}$$
#### Expansions\left(${|k|}>1$\right)

$$
\begin{aligned}
T \left( \begin{bmatrix} 1 \\ 0 \end{bmatrix} \right) &=  \begin{bmatrix} 1 \\ 0 \end{bmatrix} \\
T \left( \begin{bmatrix} 0 \\ 1 \end{bmatrix} \right) &=  \begin{bmatrix} 0 \\ k \end{bmatrix} 
\end{aligned}
$$
So,
$$A = \begin{bmatrix} 1 & 0 \\ 0 & k \end{bmatrix}$$

## Shears
### Horizontal Shear
#### Left\left($k<0$\right)
$$
\begin{aligned}
T \left( \begin{bmatrix} 1 \\ 0 \end{bmatrix} \right) &=  \begin{bmatrix} 1 \\ 0 \end{bmatrix} \\
T \left( \begin{bmatrix} 0 \\ 1 \end{bmatrix} \right) &=  \begin{bmatrix} k \\ 1 \end{bmatrix} 
\end{aligned}
$$
So,
$$A = \begin{bmatrix} 1 & k \\ 0 & 1 \end{bmatrix}$$
#### Right\left($k>0$\right)
$$
\begin{aligned}
T \left( \begin{bmatrix} 1 \\ 0 \end{bmatrix} \right) &=  \begin{bmatrix} 1 \\ 0 \end{bmatrix} \\
T \left( \begin{bmatrix} 0 \\ 1 \end{bmatrix} \right) &=  \begin{bmatrix} k \\ 1 \end{bmatrix} 
\end{aligned}
$$
So,
$$A = \begin{bmatrix} 1 & k \\ 0 & 1 \end{bmatrix}$$

### Vertical Shear
#### Down\left($k<0$\right)
$$
\begin{aligned}
T \left( \begin{bmatrix} 1 \\ 0 \end{bmatrix} \right) &=  \begin{bmatrix} 1 \\ k \end{bmatrix} \\
T \left( \begin{bmatrix} 0 \\ 1 \end{bmatrix} \right) &=  \begin{bmatrix} 0 \\ 1 \end{bmatrix} 
\end{aligned}
$$
So,
$$A = \begin{bmatrix} 1 & 0 \\ k & 1 \end{bmatrix}$$
#### Up\left($k>0$\right)

$$
\begin{aligned}
T \left( \begin{bmatrix} 1 \\ 0 \end{bmatrix} \right) &=  \begin{bmatrix} 1 \\ k \end{bmatrix} \\
T \left( \begin{bmatrix} 0 \\ 1 \end{bmatrix} \right) &=  \begin{bmatrix} 0 \\ 1 \end{bmatrix} 
\end{aligned}
$$
So,
$$A = \begin{bmatrix} 1 & 0 \\ k & 1 \end{bmatrix}$$
## Projections
### On to the $x_1-\text{Axis}$
$$
\begin{aligned}
T \left( \begin{bmatrix} 1 \\ 0 \end{bmatrix} \right) &=  \begin{bmatrix} 1 \\ 0 \end{bmatrix} \\
T \left( \begin{bmatrix} 0 \\ 1 \end{bmatrix} \right) &=  \begin{bmatrix} 0 \\ 0 \end{bmatrix} 
\end{aligned}
$$
So,
$$A = \begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix}$$
### On to the $x_2-\text{Axis}$
$$
\begin{aligned}
T \left( \begin{bmatrix} 1 \\ 0 \end{bmatrix} \right) &=  \begin{bmatrix} 0 \\ 0 \end{bmatrix} \\
T \left( \begin{bmatrix} 0 \\ 1 \end{bmatrix} \right) &=  \begin{bmatrix} 0 \\ 1 \end{bmatrix} 
\end{aligned}
$$
So,
$$A = \begin{bmatrix} 0 & 0 \\ 0 & 1 \end{bmatrix}$$





