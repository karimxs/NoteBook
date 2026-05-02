# 1.
![[Pasted image 20260412114806.png]]
$$
dq=\sigma dA
$$
$$
d\vec{E}=k\cdot \frac{\sigma dA}{R^{2}}
$$
Due to the symmetry, we are left with the $\hat{z}$ component.
Therefore, we will calculate $E_z$.
$$
dE_{z}=dE \cos \theta
$$
$$
dA=R^{2}\sin \theta d\theta d\phi
$$
$$
\Downarrow
$$
$$
dE_{z}=-k\sigma \frac{\cancel{R^{2}}\sin\theta}{\cancel{R^{2}}}\cos \theta d\theta d\phi
$$
$$
\int dE_{z}=-k\sigma \int_{0}^{2\pi}\int_{0}^{\pi/2}\sin\theta\cos \theta d\theta d\phi
$$

$$
\int \sin \theta \cos \theta \, d\theta = \left[ \frac{\sin^2 \theta}{2} \right]_{0}^{\pi/2}=\frac{1}{2}
$$
$$
E_{z}=-k\sigma 2\pi \frac{1}{2}=-k\sigma \pi
$$
---
# 2.
![[Pasted image 20260412133201.png]]
$$
\begin{cases}
\vec{r}=(0,0,z) \\
\vec{r}^{'}=R\cos \theta \hat{x}+R\sin \theta \hat{y} \\
\lambda=\lambda_{0} \\
\theta=0-\frac{\pi}{5}
\end{cases}
$$

$$
\Downarrow
$$

$$
\vec{R}=-R\cos \theta \hat{x}+R\sin \theta \hat{y}+z\hat{z}
$$

$$
\left| \vec{R} \right|=\sqrt{ R^{2}+z^{2} } 
$$

$$
\hat{R}=\frac{\vec{R}}{\left| \vec{R} \right| }
$$

$$
\begin{cases}
dq=\lambda dl \\
dl=Rd\theta \\
\Downarrow \\
dq=\lambda Rd\theta
\end{cases}
$$

$$
d\vec{E}=k \frac{dq}{\left| \vec{R} \right| }\hat{R}
$$

$$
d\vec{E}=k\lambda \frac{R}{\left| \vec{R} \right|^3 }d\theta
$$


$$
= \frac{k \lambda R}{(R^2 + z^2)^{3/2}} \cdot (-R \cos \phi \hat{x} - R \sin \phi \hat{y} + z \hat{z}) d\phi
$$


$$
E = \frac{k \lambda R}{(R^2 + z^2)^{3/2}} \int_{0}^{\pi/5} (-R \cos \phi \hat{x} - R \sin \phi \hat{y} + z \hat{z}) d\phi
$$




$$-R \int_{0}^{\pi/5} \cos \phi \, d\phi = -R \sin \phi \bigg|_{0}^{\pi/5} = -R \sin \frac{\pi}{5}$$




$$\int_{0}^{\pi/5} -R \sin \phi \, d\phi = R \cos \phi \bigg|_{0}^{\pi/5} = R \left( \cos\left(\frac{\pi}{5}\right) - 1 \right)$$




$$\int_{0}^{\pi/5} z \, d\phi = \frac{z \pi}{5}$$

$$
E = \frac{k \lambda_0 R}{(R^2 + z^2)^{3/2}} \left( -R \sin\left(\frac{\pi}{5}\right) \hat{x} + R \left(\cos\left(\frac{\pi}{5}\right) - 1\right) + z \frac{\pi}{5} \hat{z} \right)
$$
---
# 3.
![[Pasted image 20260414115301.png]]
At point a:
$$
dq = \lambda dl=\lambda R d\theta
$$
$$
dE=k \frac{dq}{R^{2}}=k \frac{\lambda}{R}d\theta
$$
$$
\begin{cases}
dE_{x}=0 \\
dE_{y}=dE\sin \theta
\end{cases}
$$
$$
E=\int_{0}^\pi \frac{k\lambda}{R}\sin \theta d\theta
$$
$$
E_{a}=\frac{k\lambda}{R}[-\cos \theta]^\pi_{0}=\frac{2k\lambda}{R}
$$
At point b:
$$dE = \frac{k\lambda}{R} d\theta$$

$$\Downarrow$$

$$d\vec{E} = -\frac{k\lambda}{R} \hat{r} d\theta = -\frac{k\lambda}{R^2} \vec{R} d\theta$$

$$= -\frac{k\lambda}{R^2} R(\cos\theta \hat{x} + \sin\theta \hat{y}) d\theta$$

$$= -\frac{k\lambda}{R} (\cos\theta \hat{x} + \sin\theta \hat{y}) d\theta$$

$$-\frac{\pi}{2} \le \theta \le \frac{\pi}{2}$$

$$E = -\frac{k\lambda}{R} \int_{-\pi/2}^{\pi/2} (\cos\theta \hat{x} + \sin\theta \hat{y}) d\theta$$

$\underline{x:}$

$$\int_{-\pi/2}^{\pi/2} \cos\theta d\theta = \sin\theta \Big|_{-\pi/2}^{\pi/2} = 1 - (-1) = 2$$

$\underline{y:}$

$$\int_{-\pi/2}^{\pi/2} \sin\theta d\theta = -\cos\theta \Big|_{-\pi/2}^{\pi/2} = 0$$

$$\Downarrow$$

$$E = -\frac{2k\lambda}{R} \hat{x}$$

---
# 4.
![[Pasted image 20260502202445.png]]

$$dE = \frac{k}{R^2} dq \hat{r} \quad\quad\quad\quad dq = \lambda dx$$

$\underline{\text{B:}}$

$$R = b - x$$

$$E_b = \int_{-\infty}^{0} \frac{k\lambda}{(b-x)^2} dx = -k\lambda \left( \frac{1}{\infty} - \frac{1}{b^2} \right) = \frac{k\lambda}{b^2} \hat{x}$$

$\underline{\text{A:}}$

$$\vec{r} = x\hat{x} + a\hat{y}$$

$$\hat{r} = \frac{\vec{r}}{|\vec{r}|}$$

$$|\vec{r}| = \sqrt{x^2+a^2}$$

$$E_x = k\lambda \int_{0}^{\infty} \frac{x}{(x^2+a^2)^{3/2}} dx$$

$$u = x^2 + a^2 \quad \implies \quad du = 2x dx \quad \implies \quad \frac{du}{2} = x dx$$

$$\frac{k\lambda}{2} \int u^{-3/2} du = k\lambda \left( \frac{-1}{\sqrt{u}} \right)$$

$$= \frac{k\lambda}{\sqrt{x^2+a^2}} \Bigg|_{0}^{\infty} = \frac{k\lambda}{\sqrt{a^2}} = \frac{k\lambda}{a} \hat{x} = E_x$$

$$E_y = k\lambda \int_{0}^{\infty} \frac{a}{(x^2+a^2)^{3/2}} dx$$

$$= k\lambda a \int_{0}^{\infty} \frac{dx}{(x^2+a^2)^{3/2}}$$

$$= k\lambda a \left( \frac{x}{a^2 \sqrt{x^2+a^2}} \right) \Bigg|_{0}^{\infty} = \frac{k\lambda}{a} \hat{y}$$

$$E_A = \frac{k\lambda}{a} (\hat{x} + \hat{y})$$

$$\lim_{x\rightarrow\infty} \frac{x}{\sqrt{x^2+a^2}} = 1$$

$\underline{\text{C:}}$

$$\vec{r} = (b-x)\hat{x} + a\hat{y}$$

$$d\vec{E} = \frac{k\lambda}{r^3} ((b-x)\hat{x} + a\hat{y}) dx$$

$$= \frac{k\lambda ((b-x)\hat{x} + a\hat{y})}{((b-x)^2+a^2)^{3/2}} dx$$

$$dE_x = \frac{k\lambda (b-x)}{((b-x)^2+a^2)^{3/2}} dx$$

$$|\vec{r}| = \sqrt{(b-x)^2+a^2}$$

$$u = b-x \quad \implies \quad du = -dx \quad \implies \quad -du = dx$$

$$E_x = k\lambda \int_{-\infty}^{0} \frac{b-x}{((b-x)^2+a^2)^{3/2}} dx$$

$$= -k\lambda \int \frac{u}{(u^2+a^2)^{3/2}} du$$

$$w = u^2+a^2 \quad \implies \quad dw = 2u du$$

$$= k\lambda \left( \frac{-1}{\sqrt{w}} \right) = \frac{-k\lambda}{\sqrt{(b-x)^2+a^2}} \Bigg|_{-\infty}^{0}$$

$$E_x = \frac{k\lambda}{\sqrt{b^2+a^2}} \hat{x}$$

$$E_y = k\lambda a \int_{-\infty}^{0} \frac{1}{((b-x)^2+a^2)^{3/2}} dx \quad \rightarrow \quad u = b-x$$

$$= -k\lambda a \left( \frac{u}{a^2 \sqrt{u^2+a^2}} \right)$$

$$= \frac{-k\lambda(b-x)}{a\sqrt{(b-x)^2+a^2}} \Bigg|_{-\infty}^{0} = \frac{-k\lambda b}{a\sqrt{b^2+a^2}} + \frac{k\lambda}{a}$$

$$= \frac{k\lambda}{a} \left( 1 - \frac{b}{\sqrt{b^2+a^2}} \right) \hat{y}$$

$$E_C = \frac{k\lambda}{\sqrt{b^2+a^2}} \hat{x} + \frac{k\lambda}{a} \left( 1 - \frac{b}{\sqrt{b^2+a^2}} \right) \hat{y}$$

---
# 5.
![[Pasted image 20260502203653.png]]

$$\rho(r,\theta,\varphi) = \rho_0 r \cos\theta$$

$$dE = k\frac{dq}{r^2}$$

$$dq = \rho(r,\theta,\varphi) dV \quad \leftarrow \quad dV = r^2 \sin\theta dr d\theta d\varphi$$

$$E = \int \frac{k \rho r \cos\theta}{r^3} dV$$

$$E = k\rho_0 \int \frac{r \cos\theta}{r^3} (r^2 \sin\theta dr d\theta d\varphi) \hat{r}$$

$$= k\rho_0 \int \cos\theta \sin\theta dr d\theta d\varphi \hat{r}$$

$$\hat{r} = \sin\theta \cos\varphi \hat{x} + \sin\theta \sin\varphi \hat{y} + \cos\theta \hat{z}$$

$\underline{\text{x:}}$

$$E_x = k\rho_0 \int r dr \int \cos\theta \sin^2\theta d\theta \int \cos\varphi d\varphi = 0$$

$\underline{\text{y:}}$

$$E_y = k\rho_0 \int r dr \int \cos\theta \sin^2\theta d\theta \int \sin\varphi d\varphi = 0$$

$\underline{\text{z:}}$

$$E_z = k\rho_0 \int_{R/2}^{R} r dr \int_{0}^{\pi} \cos^2\theta \sin\theta d\theta \int_{0}^{2\pi} d\varphi$$

$$\int_{R/2}^{R} r dr = \frac{r^2}{2} \Bigg|_{R/2}^{R} = \frac{1}{2} \left( R^2 - \frac{R^2}{4} \right) = \frac{3}{8}R^2$$

$$\int_{0}^{\pi} \cos^2\theta \sin\theta d\theta \quad \rightarrow \quad \cos\theta = u, \quad -\sin\theta d\theta = du$$

$$\int -u^2 du = \frac{-u^3}{3}$$

$$\frac{-\cos^3\theta}{3} \Bigg|_{0}^{\pi} = \frac{1}{3} - \left(-\frac{1}{3}\right) = \frac{2}{3}$$

$$\int_{0}^{2\pi} d\varphi = 2\pi$$

$$E_z = k\rho_0 \left( \frac{3}{8}R^2 \right) \left( \frac{2}{3} \right) (2\pi)$$

$$E_z = \frac{k\rho_0 \pi R^2}{2} \hat{z} \quad \implies \quad \vec{E} = \frac{k\rho_0 \pi R^2}{2} \hat{z}$$