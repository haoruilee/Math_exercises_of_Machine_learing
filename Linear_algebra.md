$\begin{array}{|l|}
\hline \text { Machine Learning } \\\\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \textbf { Assignment #1 (Linear Algebra) }\\\\
\text {Instructor: Beilun Wang }\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \text{ Name: 61518407 Haoruili}\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \text {   (Due:2.27) } \\
\hline
\end{array}$

### Problem 1

Let two vectors a=(1 2 3)^T^and b=(-8 1 2)^T^answer the following equations:

**(1) Compute the $\ell_{2}$ norm of a and b**

**Answer：**
$$
||a||=\sqrt{\sum_{i}^{n}\left(a_{i}\right)^{2}}=\sqrt{\left(a_{1}\right)^{2}+\left(a_{2}\right)^{2}+\cdots+\left(a_{n}\right)^{2}}=\sqrt{1+4+9}=\sqrt{14}
$$
Foe the same reason
$$
||b||=\sqrt{64+1+4}=\sqrt{69}
$$
**(2) Calculate the Euclidean distance between a and b**

**Answer：**
$$
||a-b||=||b-a||=\sqrt{\sum_{i}^{n}\left(b_{i}-a_{i}\right)^{2}}==\sqrt{81+1+1}=\sqrt{83}
$$
**(3) Are a and b orthogonal?**

**Answer：**

Yes.
$$
\begin{align}
\because&\ a\times b=0→a\perp b \\
\because&\  a\times b=(-8+2+6)=0\\
\therefore&\ a\perp b
\end{align}
$$

### Problem 2

Suppose $A=\left[\begin{array}{ccc}{1} & {-3} & {3} \\ {3} & {-5} & {3} \\ {6} & {-6} & {4}\end{array}\right]$, answer the following questions:

**(1) Calculate $A^{-1}$ and $\operatorname{det}(A)$.**

**Answer**:
$$
\begin{align}
det(A)&=\left|\begin{array}{ccc}{1} & {-3} & {3} \\ {3} & {-5} & {3} \\ {6} & {-6} & {4}\end{array}\right|\\&=1\cdot\left|\begin{array}{ccc}{-5}&{3}\\{-6}&{4}\end{array}\right|+3\cdot\left|\begin{array}{ccc}{3}&{3}\\{6}&{4}\end{array}\right|+3\cdot\left|\begin{array}{ccc}{3}&{-5}\\{6}&{-6}\end{array}\right|\\&=-20+18+3\times(12-18)+3\times(-18+30)\\&=-2-18+36=16
\end{align}
$$

Therefore:
$$
\begin{align}
\because |A|\ \not=& \ 0
\\

\therefore A^{-1}=&\frac{1}{|A|}\left[\begin{array}{cccc}
A_{11} & A_{21} & \dots & A_{m 1} \\
A_{12} & A_{22} & \dots & A_{12} \\
\dots & \dots & \dots & \dots \\
A_{1 n} & A_{2 n} & \dots & A_{m n}
\end{array}\right]=\left[\begin{array}{ccc}
-1 / 8 & -3 / 8 & 3 / 8 \\
3 / 8 & -7 / 8 & 3 / 8 \\
3 / 4 & -3 / 4 & 1 / 4
\end{array}\right]
\end{align}
$$


**(2) The Rank of $A$ is?**

**Answer**: 
$$
rank(A)=3
$$


**(3) The trace of $A$ is?**

**Answer**:
$$
tr(A)=(1-5+4)=0
$$


**(4) Calculate $A+A^{T}$**

**Answer**:
$$
A+A^{T}=\left[\begin{array}{ccc}{1} & {-3} & {3} \\ {3} & {-5} & {3} \\ {6} & {-6} & {4}\end{array}\right]+\left[\begin{array}{ccc}{1} & {3} & {6} \\ {-3} & {-5} & {-6} \\ {3} & {3} & {4}\end{array}\right]
=\left[\begin{array}{ccc}{2} & {0} & {9} \\ {0} & {-10} & {-3} \\ {9} & {-3} & {8}\end{array}\right]
$$

**(5) Is $A$ an orthogonal matrix? State your reason.**

**Answer**:
$$
\begin{align}
\because &\ A^{T}A=\left[\begin{array}{ccc}{1} & {-3} & {3} \\ {3} & {-5} & {3} \\ {6} & {-6} & {4}\end{array}\right]\left[\begin{array}{ccc}{1} & {3} & {6} \\ {-3} & {-5} & {-6} \\ {3} & {3} & {4}\end{array}\right]
=\left[\begin{array}{ccc}{46} & {-54} & {36} \\ {-54} & {70} & {-48} \\ {36} & {-48} & {34}\end{array}\right]\not=I\\
\therefore &\ A^{T} \text {is not an orthogonal matrix.}
\end{align}
$$

**(6) Calculate all the eigenvalue $\lambda$ and corresponding eigenvectors of $A$.**

**Answer**:
$$
\begin{align}
&[ λE-A ]=\left|\begin{array}{ccc}
\lambda-1 & 3 & -3 \\
-3 & \lambda+5 & -3 \\
-6 & 6 & \lambda-4
\end{array}\right|=0
\\
&(\lambda+2)^{2}(\lambda-4)=0
\\
&→\lambda_{1,2}=-2,λ_{3}=4
\\
&a_{1}=\left[\begin{array}{ccc}{0} \\ {1} \\ {1}\end{array}\right]，a_{2}=\left[\begin{array}{ccc}{1} \\ {1} \\ {0}\end{array}\right]，a_{3}=\left[\begin{array}{ccc}{1} \\ {1} \\ {2}\end{array}\right]
\end{align}
$$

**(7) Diagonalize the matrix $A$.**

Answer:
$$
A=\left[\begin{array}{ccc}{-2} & {0} & {0} \\ {0} & {-2} & {0} \\ {0} & {0} & {4}\end{array}\right]
$$
**(8) Calculate the $\ell_{2,1}$ norm $\|A\|_{2,1}$ and the Frobenius norm (i.e. $\ell_{2}$ norm) $\|A\|_{F}$**

Answer:
$$
\begin{align}
&\|A\|_{2,1}=\sqrt{46}+\sqrt{70}+\sqrt{34}\\
&\|A\|_{F}=\sqrt{46+70+34}=\sqrt{150}
\end{align}
$$
**(9) Calculate the nuclear norm $\|A\|$. and the spectral norm $\|A\|_{2}$**

**Answer**:
$$
\left|\begin{array}{ccc}
\lambda-46 & 54 & -36 \\
54 & \lambda-70 & 48 \\
-36 & 48 & \lambda-34
\end{array}\right|=0
$$

$$
\lambda^{3}-150 \lambda^{2}+648 \lambda-256=0
$$

$$
\begin{array}{c}
\lambda_{1}=4 \\
\lambda_{2}=73+9 \sqrt{65} \\
\lambda_{3}=73-9 \sqrt{65}
\end{array}
$$

$$
\|A\|_{*}\approx 14.727922061357859\\
\|A\|_{2}=\sqrt{\max \left(A^{T} A\right)} \approx 12.064838156174618
$$



### Problem 3

Please give some proper steps to show how you get the answer. Let $x=\left(x_{1}, x_{2}, x_{3}\right)^{T}$ and
$$
\left\{\begin{array}{l}
2 x_{1}+2 x_{2}+3 x_{3}=1 \\
x_{1}-x_{2}=-1 \\
-x_{1}+2 x_{2}+x_{3}=2
\end{array}\right.
$$
Answer the following questions:
**(1) Solve the linear equations**

**Answer**: 
$$
\left\{\begin{array}{l}
x_{1}=-1 \\
x_{2}=0 \\
x_{3}=1
\end{array}\right.
$$


**(2) Write it into matrix form(i.e. $A x=b$ ) and we will use the same $A$ and $b$ in the following questions.**

**Answer**:
$$
\left[\begin{array}{ccc}{2} & {2} & {3} \\ {1} & {-1} & {0} \\ {-1} & {2} & {1}\end{array}\right]\left[\begin{array}{ccc}{x_{1}}\\{x_{2}} \\{x_{3}}\end{array}\right]=\left[\begin{array}{ccc}{{1}}\\{{-1}} \\{{2}}\end{array}\right]
$$


**(3) The Rank of $A$ is?**

**Answer**：
$$
\because\ |A|\not= \ 0
\\
\therefore\ rank(A)=3
$$


**(4) Calculate $A^{-1}$ and $\operatorname{det}(A)$**

**Answer:**
$$
det(A)=-1\\
A^{-1}=\left[\begin{array}{ccc}{1} & {-1} & {-1} \\ {4} & {-5} & {-6} \\ {-3} & {3} & {4}\end{array}\right]
$$


**(5) Use (4) to solve the linear equations**

**Answer:**
$$
\left[\begin{array}{ccc}{x_{1}}\\{x_{2}} \\{x_{3}}\end{array}\right]=\frac{1}{det(A)}\left[\begin{array}{ccc}{D_{1}}\\{D_{2}} \\{D_{3}}\end{array}\right]=\frac{1}{-1}\left[\begin{array}{ccc}{{1}}\\{{0}} \\{{-1}}\end{array}\right]=\left[\begin{array}{ccc}{{-1}}\\{{0}} \\{{1}}\end{array}\right]
$$


**(6) Calculate the inner product and outer product of $x$ and $b$.(i.e. $\langle x, b\rangle$ and $x \otimes b$ )**

**Answer：**
$$
\langle x, b\rangle=1
\\
x \otimes b^{T}=\left[\begin{array}{ccc}{-1} & {1} & {-2} \\ {0} & {0} & {0} \\ {1} & {-1} & {2}\end{array}\right]
$$


**(7) Calculate the $\ell_{1}, \ell_{2}$ and $\ell_{\infty}$ norm of $b$**

**Answer:**
$$
\begin{align}
\ell_{1}&=4\\
\ell_{2}&=\sqrt{6}\\
\ell_{\infty}&=2
\end{align}
$$


**(8) Suppose $y=\left(y_{1}, y_{2}, y_{3}\right)^{T},$ calculate $y^{T} A y, \nabla_{y} y^{T} A y$**

**Answer:**
$$
\begin{align}
&y^{T} A y=y^{T}\left[\begin{array}{ccc}{2} & {2} & {3} \\ {1} & {-1} & {0} \\ {-1} & {2} & {1}\end{array}\right]y

=\left[\begin{array}{ccc}{2y_{1}+y_{2}-y_{3}} \\ {2y_{1}-y_{2}+y_{3}}\\ {3y_{1}+y_{3}}\end{array}\right]y
=2y^{2}_{1}-y^{2}_{2}+y^{2}_{3}+3y_{1}y_{2}+2y_{1}y_{3}+y_{2}y_{3}
\\
&\nabla_{y} y^{T} A y=\left[\begin{array}{ccc}{4y_{1}+3y_{2}+2y_{3}}\\{-2y_{2}+3y_{1}+y_{3}} \\{2y_{3}+2y_{1}+y_{2}}\end{array}\right]
\end{align}
$$



**(9) We add one linear equation $-x_{1}+2 x_{2}+x_{3}=2$ into linear equations above. Write it into matrix form(i.e. $\left.A_{1} x=b\right)$**

**Answer:**
$$
\left\{\begin{array}{l}
2 x_{1}+2 x_{2}+3 x_{3}=1 \\
x_{1}-x_{2}=-1 \\
-x_{1}+2 x_{2}+x_{3}=2\\
-x_{1}+2 x_{2}+x_{3}=2
\end{array}\right.
$$
Therefore:
$$
\left[\begin{array}{ccc}{2} & {2} & {3} \\ {1} & {-1} & {0} \\ {-1} & {2} & {1}\\{-1}&{2}&{1}\end{array}\right]\left[\begin{array}{ccc}{x_{1}}\\{x_{2}} \\{x_{3}}\end{array}\right]=\left[\begin{array}{ccc}{{-1}}\\{{0}} \\{{1}\\{1}}\end{array}\right]
$$


**(10) The rank of $A_{1}$ is?**

**Answer:**
$$
rank(A)=3
$$


**(11) Could these linear equations $A_{1} x=b$ be solved? State reasons.**

Answer:

Yes.
$$
\begin{align}
\because\ &rank(A)=3<4
\\
\therefore\ &A_{1}x=b \text{ can be solved.}
\end{align}
$$

