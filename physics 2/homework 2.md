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
