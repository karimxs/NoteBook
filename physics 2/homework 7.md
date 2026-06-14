## 1.
![[Pasted image 20260614162601.png]]

## a.
$$
\vec{J}=\sigma \cdot \vec{E}=\sigma_{0}\left( 1-\frac{r}{R} \right) \cdot E_{0}\hat{z}
$$

---
## b.
$$
I=\int \int \vec{J}\cdot d\vec{s} $$$$= \sigma_{0}E_{0}\int ^{R}_{0}\int ^{2\pi}_{0}\left( 1-\frac{r}{R} \right)r d\theta dr \hat{z}\cdot \hat{z}=2\pi \sigma_{0}E_{0}\int^R_{0}r-\frac{r^{2}}{R}dr
$$
$$
\Rightarrow 2\pi E_{0}\sigma_{0} \left[ \frac{r^2}{2} -\frac{r^3}{3R} \right] |^{R}_{0} = 2\pi E_{0}\sigma_{0} \left( \frac{R^2}{2} -\frac{R^2}{3} \right)
$$
$$
=\frac{\pi E_{0}\sigma_{0}R^2}{3}
$$

---
## c.
$$R = \frac{1}{\sigma} \cdot \frac{L}{A} \rightarrow dR = \frac{1}{\sigma_0(1-\frac{r}{R})} \cdot \frac{L}{2\pi r dr}$$

$$\frac{1}{R_T} = \int_{0}^{R} \frac{1}{dR} = \int_{0}^{R} \frac{\sigma_0(1-\frac{r}{R}) \cdot 2\pi r dr}{L} = \frac{2\pi\sigma_0}{L} \int_{0}^{R} \left(r - \frac{r^2}{R}\right) dr =$$

$$\Rightarrow \frac{2\pi\sigma_0}{L} \left[ \frac{r^2}{2} - \frac{r^3}{3R} \right] \Bigg|_{0}^{R} = \frac{\pi\sigma_0 R^2}{3L}$$

$$R_T = \frac{3L}{\pi\sigma_0 R^2}$$

$$\left( V = I R = \frac{\cancel{3L}}{\cancel{\pi\sigma_0 R^2}} \cdot \frac{\cancel{\pi E_0 \sigma_0 R^2}}{\cancel{3}} = E_0 \cdot L  \right)$$

$$-V + I R_1 + V_{c_1} + I R_2 + V_{c_2} = 0$$

$$-V + I(R_1 + R_2) + V_{c_1} + V_{c_2} = 0$$

$$-V + \frac{\partial Q}{\partial t}(R_1 + R_2) + \frac{Q_1}{C_1} + \frac{Q_2}{C_2} = 0$$

$$-V + \frac{\partial Q}{\partial t} \overbrace{(R_1 + R_2)}^{R_T} + Q \overbrace{\left(\frac{1}{C_1} + \frac{1}{C_2}\right)}^{\frac{1}{C_T}} = 0$$

$$-V + \frac{\partial Q}{\partial t} R_T + \frac{Q}{C_T} = 0 \rightarrow \frac{\partial Q}{\partial t} = \frac{V}{R_T} - \frac{Q}{C_T}$$

$$R_T = R_1 + R_2, \quad \frac{1}{C_T} = \frac{1}{C_1} + \frac{1}{C_2} $$
![[Pasted image 20260614163408.png]]
![[Pasted image 20260614163422.png]]


---
# 2.
![[Pasted image 20260614163120.png]]
![[Pasted image 20260614163501.png]]![[Pasted image 20260614163517.png]]

---
# 3.
![[Pasted image 20260614163051.png]]
![[Pasted image 20260614164802.png]]


---
# 4.
![[Pasted image 20260614163605.png]]
![[Pasted image 20260614164719.png]]

---
# 5.
![[Pasted image 20260614163649.png]]


---
# 6.
![[Pasted image 20260614164905.png]]
![[Pasted image 20260614164942.png]]
![[Pasted image 20260614164955.png]]
![[Pasted image 20260614165005.png]]
![[Pasted image 20260614165014.png]]
