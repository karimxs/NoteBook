$$
f_{n}(x)=x^n
$$
$$
x \in [0,1]
$$
$$
f(x)=\lim_{ n \to \infty }f_{n}(x) 
$$
$$
=\lim_{ n \to \infty }x^n;0<x<1 
$$
$$
=0
$$
$$
f(x)=\begin{cases}
0  & x \in [0,1] \\
1  & x=1
\end{cases}
$$
---
$$
f_{n}(x)=x^{n}-x^{2n}
$$
$$
=x^{n}(1-x^n)
$$
$$
x \in [0,1]
$$
$$
f(x)=0
$$
---
$$
f_{n}(x)=nxe^{-nx^{2}}
$$
$$
x \in[0,\infty)
$$
$$
\frac{nx}{e^{nx^2}}[l'hopital]=\frac{x}{x^2e^{nx^2}}=\frac{1}{xe^{nx^2}}
$$
$$
f(x)=0
$$
---
$$
f_{n}(x)=\left( 1+\frac{1}{n} \right)\cdot x^2
$$
$$
x \in [0,1]
$$
$$
f_{n}(x)=1\cdot x^{2}
$$
$$
f(x)=x^2
$$
$$
\left| \left( 1+\frac{1}{n} \right)\cdot x^2 -x^2\right|<\epsilon 
$$
$$
x^2\left| \frac{1}{n} \right|<\epsilon 
$$
$$
\frac{x^{2}}{n}\leq \frac{1}{n}<\epsilon
$$
$$
n> \frac{1}{\epsilon}
$$
---
$$
\lim_{ n \to \infty }sup \left| f_{n}(x)-f(x) \right|=0\Leftrightarrow  
$$
$$
f_{n}(x)=x^{n}-x^{2n}
$$
$$
f_{n}(x)=x^{n}(1-x^{n})
$$
---
$$
f_{n}(x)=nxe^{-nx^{2}}
$$
$$
x \in[0,\infty)
$$
$$
\lim_{ n \to \infty } sup_{x}\left| nxe^{-nx^{2}}-0 \right| 
$$
$$
\frac{nx}{e^{nx^2}}=0
$$
$$\frac{
n\cdot e^{nx^2}-x^2e^{nx^2}\cdot x}{e^{nx^2}}
$$