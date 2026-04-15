# 1.
![[Pasted image 20260330141229.png]]
$$
\int_{0}^{2}\int_{0}^{1}\int_{0}^{4}3xyz^{2}\space dx\space dy\space dz
$$
Let's take every part of this integration 

$$
\int_{0}^{4}3xyz^{2} dx= \frac{3}{2}x^{2}yz^2|^{4}_{0}=24yz^2
$$
$$
\int^1_{0} 24yz^2dy=12y^2z^2|^{1}_{0}=12z^2
$$
$$
\int_{0}^2 12z^2dz=4z^3|^{2}_{0}=32
$$
$$
\int_{0}^{2}\int_{0}^{1}\int_{0}^{4}3xyz^{2}\space dx\space dy\space dz=32
$$
 ---
# 2.
![[Pasted image 20260330142339.png]]
$$
\int ^{3}_{1}\int ^{x^2}_{x} (x+y)dy\space dx
$$
$$
\int ^{x^2}_{x}(x+y)dy=xy+\frac{y^{2}}{2}|^{x^2}_{x}=x^{3}+\frac{x^{4}}{2}-x^{2}-\frac{x^{2}}{2}
$$
$$
=\frac{x^4}{2}+x^3-1.5x^2
$$
$$
\int^3_{1}x^4+x^3-1.5x^2dx =\frac{x^5}{10}+\frac{x^4}{4}-\frac{x^3}{2}|^3_{1}
$$
$$
=31.05--0.15=31.2
$$
$$
\int ^{3}_{1}\int ^{x^2}_{x} (x+y)dy\space dx=31.2
$$
---
# 3.
![[Pasted image 20260330143748.png]]
## a.
$$
Q=\int \int \sigma dA
$$
$$
=\int \int \alpha y^{2} \space dx \space dy
$$
$$
R^2=x^2+y^2
$$
$$
\int^R_{-R} \int_{-\sqrt{ R^{2}-x^2 }}^\sqrt{ R^{2}-x^{2} } \alpha y^2 \space dy \space dx
$$
$$
\int_{-\sqrt{ R^{2}-x^2 }}^\sqrt{ R^{2}-x^{2} } \alpha y^2 \space dy=\frac{\alpha y^{3}}{3}=\frac{\alpha(R^2-x^2)^{1.5}}{3}+\frac{\alpha(R^2-x^2)^{1.5}}{3}
$$
$$
=\frac{2\alpha(R^2-x^2)^{1.5}}{3}
$$
$$
\int^R_{-R} \frac{2\alpha(R^2-x^2)^{1.5}}{3} dx=\frac{4\alpha}{3}\int^R_{0} (R^2-x^2)^{1.5} dx
$$
$$
=\frac{4\alpha}{3} \int^{\frac{\pi}{2}}_{0}(R^2-R^2sin^2\theta)^{1.5} \cdot R\cos \theta d\theta
$$
$$
=\frac{4\alpha}{3} \int^{\frac{\pi}{2}}_{0}(R^2\cos^2\theta)^{1.5} \cdot R\cos \theta d\theta=\frac{4\alpha R^4}{3}\int^{\frac{\pi}{2}}_{0}\cos ^{4} \theta d\theta
$$
$$
=\frac{4\alpha R^{4}}{3}\cdot \frac{3\pi}{16}
$$
$$
Q=\frac{\alpha \pi R^{4}}{4}
$$
---
## b.
$R$ is simply $r$ going from $0$ to $R$, and $\theta$ going from $0$ to $2\pi$.
$$
\begin{cases}
\sigma=\alpha y^2=\alpha(r\sin \theta)^{2}  \\
dxdy=r dr d\theta
\end{cases}
$$
$$
Q = \int_{0}^{2\pi} \int_{0}^{R} (\alpha r^2 \sin^2\theta) \cdot r \,dr \,d\theta
$$
$$
Q = \int_{0}^{2\pi} \int_{0}^{R} \alpha r^3 \sin^2\theta \,dr \,d\theta
$$
$$
\int_{0}^{R} \alpha r^3 \sin^2\theta \,dr = \alpha \sin^2\theta \left[ \frac{r^4}{4} \right]_{0}^{R} = \frac{\alpha R^4}{4} \sin^2\theta
$$
$$
Q = \int_{0}^{2\pi} \frac{\alpha R^4}{4} \sin^2\theta \,d\theta
$$
To integrate $\sin^2\theta$, we use the half-angle identity: $\sin^2\theta = \frac{1 - \cos(2\theta)}{2}$.
$$
Q = \frac{\alpha R^4}{4} \int_{0}^{2\pi} \frac{1 - \cos(2\theta)}{2} \,d\theta
$$

$$
Q = \frac{\alpha R^4}{8} \left[ \theta - \frac{\sin(2\theta)}{2} \right]_{0}^{2\pi}
$$
$$
Q = \frac{\alpha R^4}{8} \left( (2\pi - 0) - (0 - 0) \right)
$$

$$
Q = \frac{\alpha \pi R^4}{4}
$$
---
# 4.
![[Pasted image 20260330165110.png]]
## a.
![[Pasted image 20260330175657.png]]
$$
U_{total}=U_{1,2}+U_{2,3}+U_{3,1}
$$
$$
l=r_{1,2}=r_{2,3}=r_{3,1}=1
$$
$$
U_{total}=k\left( \frac{q_{1}q_{2}}{l}+\frac{q_{2}q_{3}}{l}+\frac{q_{3}q_{1}}{l}
 \right)
$$
$$
U_{total}=k\left(-12 \times 10^{-12} \right) =-0.108 \space \text{Joules}
$$
---

## b.
![[Pasted image 20260330175723.png]]
$$
\Delta U=q_{4} \cdot V_{center}
$$
$$
V_{center}=\frac{k}{r}(q_{1}+q_{2}+q_{3})=45\sqrt{ 3 }\times 10^{3}
$$
$$
\Delta U=(5\times 10^{-6})\cdot(45\sqrt{ 3 }\times 10^{3})=225\sqrt{ 3 }\times 10^{-3} 
$$
$$
\Delta U \approx 0.3897 \space \text{Joules}
$$
---
# 5.
![[Pasted image 20260330180433.png]]
![[Pasted image 20260330180701.png]]

$$\vec{F}_{i} = k \frac{q_i \cdot q_t}{|\vec{r}_{it}|^3} \vec{r}_{it}$$

 Force from Charge 1 ($q_1 = q$)

- **Position:** $\vec{r}_1 = (3, 4, 1)$
- **Displacement Vector:** $\vec{r}_{1t} = (0-3, 0-4, 1-1) = (-3, -4, 0)$
- **Distance:** $|\vec{r}_{1t}| = \sqrt{(-3)^2 + (-4)^2 + 0^2} = \sqrt{9 + 16} = 5$
- **Force Vector ($\vec{F}_1$):**
$$\vec{F}_1 = k \frac{(q)(-4q)}{5^3} (-3, -4, 0)$$
$$\vec{F}_1 = k \frac{-4q^2}{125} (-3, -4, 0)$$
$$\vec{F}_1 = k q^2 \left( \frac{12}{125}, \frac{16}{125}, 0 \right) = k q^2 (0.096, 0.128, 0)$$

Force from Charge 2 ($q_2 = 2q$)

- **Position:** $\vec{r}_2 = (4, 3, -11)$
- **Displacement Vector:** $\vec{r}_{2t} = (0-4, 0-3, 1-(-11)) = (-4, -3, 12)$
- **Distance:** $|\vec{r}_{2t}| = \sqrt{(-4)^2 + (-3)^2 + 12^2} = \sqrt{16 + 9 + 144} = \sqrt{169} = 13$
- **Force Vector ($\vec{F}_2$):**
- $$\vec{F}_2 = k \frac{(2q)(-4q)}{13^3} (-4, -3, 12)$$

$$\vec{F}_2 = k \frac{-8q^2}{2197} (-4, -3, 12)$$
$$\vec{F}_2 = k q^2 \left( \frac{32}{2197}, \frac{24}{2197}, \frac{-96}{2197} \right) \approx k q^2 (0.0146, 0.0109, -0.0437)$$

Force from Charge 3 ($q_3 = 3q$)

- **Position:** $\vec{r}_3 = (0, 0, 5)$
- **Displacement Vector:** $\vec{r}_{3t} = (0-0, 0-0, 1-5) = (0, 0, -4)$
- **Distance:** $|\vec{r}_{3t}| = \sqrt{0^2 + 0^2 + (-4)^2} = \sqrt{16} = 4$
- **Force Vector ($\vec{F}_3$):**
$$\vec{F}_3 = k \frac{(3q)(-4q)}{4^3} (0, 0, -4)$$

$$\vec{F}_3 = k \frac{-12q^2}{64} (0, 0, -4)$$

$$\vec{F}_3 = k q^2 \left( 0, 0, \frac{48}{64} \right) = k q^2 \left( 0, 0, \frac{3}{4} \right) = k q^2 (0, 0, 0.75)$$


Total Force ($\vec{F}_{total}$)

$$\vec{F}_{total} = \vec{F}_1 + \vec{F}_2 + \vec{F}_3$$

$$F_x = k q^2 \left( \frac{12}{125} + \frac{32}{2197} \right)$$

$$F_y = k q^2 \left( \frac{16}{125} + \frac{24}{2197} \right)$$

$$F_z = k q^2 \left( 0 - \frac{96}{2197} + \frac{3}{4} \right)$$

- **X-component:** $0.096 + 0.0146 + 0 \approx \mathbf{0.1106 \, k q^2}$
- **Y-component:** $0.128 + 0.0109 + 0 \approx \mathbf{0.1389 \, k q^2}$
- **Z-component:** $0 - 0.0437 + 0.75 \approx \mathbf{0.7063 \, k q^2}$

The total force vector exerted on the $-4q$ charge is approximately:

$$\vec{F}_{total} \approx k q^2 (0.1106 \hat{i} + 0.1389 \hat{j} + 0.7063 \hat{k})$$