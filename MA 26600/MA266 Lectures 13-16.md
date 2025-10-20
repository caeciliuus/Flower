---
Class: "[[MA 26600.base|MA 26600]]"
Type: Lecture notes
Date: 2025-10-06
tags:
  - lecture
  - s1
  - ma266
  - exam
---
- Second-order linear differential equartion: $a(x)y''+b(x)y'+c(x)y=f(x)$ or $y''+p(x)y'+q(x)y=f(x)$
	- Is homogenous if $f(x)=0$, so $f(x)y''+b(x)y'+c(x)y=0$ is homogenous
- Homogenous: if $y_{1},y_{2}$ solve the second order homogenous equation, then so does $c_{1}y_{1}+c_{2}y+2$ for any constants $c_{1},c_{2}$
- Given second order linear IVP $y''+p(x)y'+q(x)y=f(x),y(a)=b_{0},y'(a)=b$, if $p(x),q(x),f(x)$ are continuous on the same interval containing $x=a$, then there is a unique solution $y$ to this problem on that interval

> [!Linear Algebra Review]
> $$\text{Given }a=\begin{bmatrix}
a &b\\c&d
\end{bmatrix},x=\begin{bmatrix}
x_{1}\\x_{2} 
\end{bmatrix},w=\begin{bmatrix}
w_{1}\\w_{2}  
\end{bmatrix}\text{ we get a 2x2 system} \begin{cases}
x_{1}a+x_{2}b=w_{1}\\x_{1}c+x_{2}d=w_{2}
\end{cases}\to Ax=w=\begin{bmatrix}
a&b\\c&d 
\end{bmatrix}
\begin{bmatrix}
x_{1}\\x_{2}  
\end{bmatrix}$$
>$$Ax=\begin{bmatrix}
a&b\\c&d
\end{bmatrix} \begin{bmatrix}
x_{1}\\x_{2}
\end{bmatrix}=x_{1}\begin{bmatrix}
a\\c
\end{bmatrix}+x_{2}\begin{bmatrix}
b\\d 
\end{bmatrix}=\begin{bmatrix}
x_{1}a+x_{2}b\\x_{1}c+x_{2}d 
\end{bmatrix}\text{ with }x,x_{0}\text{ as coefficients of columns of A}$$
>$$\text{System }Ax=w \text{ has a unique solution }x=\begin{bmatrix}
x_{1}\\x_{2} 
\end{bmatrix} \text{ if and only if }\det(A)\neq0~(\det(A)=ad-bc)$$
> Vectors $v_{1}=\begin{bmatrix}a\\c\end{bmatrix},v_{2}=\begin{bmatrix}b\\d\end{bmatrix}$ are linearly independent if, letting $A=\begin{bmatrix}v_{1}&v_{2}\end{bmatrix}=\begin{bmatrix}a&b\\c&d\end{bmatrix}$ then $Ax=0\to x=0,0$ is the only solution
> Linear dependence means the equation $Ax=0$ has a nontrivial solution ($x\neq0$) $x=\begin{bmatrix}x_{1}\\x_{2}\end{bmatrix}$
> **Independent**: $v_{1}$ cannot be expressed in terms of $v_{2}$ and vice versa
> **Dependent**: $v_{1}$ can be expressed in terms of $v_{2}$, vice versa
> System will have a unique solution if and only if $\det(A)\neq0$

- IF we find two "different enough" solutions $y_{1} ,y_{2}$ then maybe we could build up any solution $y=c_{1}y_{1}+c_{2}y_{2}$
	- "Different enough" turns out to be when $y_{1}$ and $y_{2}$ are linearly independent -> only if eq. $c_{1}y_{1}+c_{2}y_{2}=0$ implies $c_{1}=c_{2}=0$ for all $x=0$ has a solution $c_{1},c_{2}$ where one of $c_{1},c_{2}$ is nonzero
- For unique solution, we need $\det\left(\begin{bmatrix}y_{1}(c)&y_{2}(c)\\y_{1}'(c)&y_{2}'(c)\end{bmatrix}\right)=0$, known as the Wronskian

>[!exm] Find a general solution to $y''-y'-56y=0$
>Take a guess $y=e^{rx}$
> $$y''=r^2e^{rx},y'=re^{rx}\to r^2e^{rx}-re^{rx}-56e^{rx}=0$$
> $$e^{rx}(r^2-r-56)=0\to r=8,-7$$
> $$W(y_{1},y_{2})=y_{1}y_{2}'-y_{2}y_{1}'=e^{8x}(-7e^{-7x})-e^{7x}(8e^{8x})=-15e^x\neq0 \therefore y_{1}=c_{1}e^{8x}\text{ and } y_{2}=c_{2}e^{-7x}\text{ are linearly independent}$$
> 

- If roots repeat, we use trick $y_{1}=e^{rx},y_{2}=xe^{rx}\to W(y_{1},y_{2})\neq0\therefore\text{ independent}$
- Let $r_{1},r_{2}$ be real roots to $ar^2+br+c=0$
	- $r_{1}\neq r_{2}\to y=c_{1}e^{r_{1}x}+c_{2}e^{r_{2}x}$
	- $r_{1}=r_{2}\to y=c_{1}e^{rx}+c_{1}xe^{rx}$
- General $n$th order linaer equations: $y^{(n)}+a_{n-1}y^{n-1}+\dots+c_{n}y_{n}=0$ for all $x$, then $c_{1}=c_{2}=\dots=c_{n}=0$
- In general, $y^{(n)}+a_{n-1}(x)y^{n-1}\dots a_{0}(x)y=0$ has general solution $y=c_{1}y_{1}+c_{2}y_{2}+\dots+c_{n}y_{n}$ where $y_{1},y_{2},\dots, y_{n}$ are independent

> [!exm] Show that functions $f(x)=e^x,g(x)=4x,h(x)=4x^2$ are linearly dependent on $\mathbb{R}$
> $$f'=e^x,g'=4,h'=8x$$
> $$f''=e^x,g''=0,h''=8$$
> $$W(f,g,h)=\det \begin{bmatrix}
> e^x&4x&4x^2\\e^x&4&8x\\e^x&0&8
>\end{bmatrix}=e^x\det \begin{bmatrix}
> 4&8x\\0&8
\end{bmatrix}+e^x\det \begin{bmatrix}
> 4x&4x^2\\0&8
\end{bmatrix}+e^x\begin{bmatrix}
> 4x&4x^2\\4&8x
\end{bmatrix}=32e^x-32xe^x+16x^2e^x=e^x(32-16x^2)\neq0\therefore f,g,h\text{ are linearly independent}$$
- If characteristic equation has no real roots, i.e $r=a\pm ib$
	- $r=a\pm ib$ (repeated once):
		- Building blocks are $e^{ax}\cos bx,e^{ax}\sin(bx)$.
	- $r=a\pm ib$ (repeated multiple times), $\begin{pmatrix}m\text{ from }a+ ib\\m\text{ from }a-ib\end{pmatrix}$:

$$\begin{bmatrix}
e^{ax}\cos bx&e^{ax}\sin bx\\xe^{ax}\cos bx&xe^{ax}\sin bx \\
\vdots &\vdots \\
x^{m-1}e^{ax}\cos bx&x^{m-1}e^{ax}\sin bx
\end{bmatrix}\to\text{Linearly independent}$$