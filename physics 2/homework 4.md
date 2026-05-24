Here are the translated questions and their step-by-step solutions in English, based on the provided document.

### **Question 1.1**

Given a spherically symmetric electric potential depending on the distance from the origin:


$$\phi(r)=\begin{cases}\alpha\cdot(R-r)&,r<R\\ 0&,r\ge R\end{cases}$$

where $\alpha$ is a positive constant.

a. Calculate the electric field vector in all space:
The electric field is given by the negative gradient of the potential, $\vec{E} = -\vec{\nabla}\phi$.

* For $r < R$: $\vec{E} = -\frac{\partial}{\partial r}(\alpha(R-r))\hat{r} = \alpha\hat{r}$.


* For $r \ge R$: $\vec{E} = -\frac{\partial}{\partial r}(0)\hat{r} = 0$.



b. Calculate the volumetric charge density in the region $r < R$:
Using Gauss's law in differential form, $\vec{\nabla} \cdot \vec{E} = \frac{\rho}{\epsilon_0}$.
In spherical coordinates:


$$\rho = \epsilon_0 \frac{1}{r^2}\frac{\partial}{\partial r}(r^2 E_r) = \epsilon_0 \frac{1}{r^2}\frac{\partial}{\partial r}(r^2 \alpha) = \frac{2\alpha\epsilon_0}{r}$$

.

c. Calculate the surface charge density on the sphere's boundary at radius $R$:
The surface charge density $\sigma$ is determined by the discontinuity in the electric field across the boundary:
$E_{r}(R^+) - E_{r}(R^-) = \frac{\sigma}{\epsilon_0}$.
$0 - \alpha = \frac{\sigma}{\epsilon_0} \implies \sigma = -\alpha\epsilon_0$.

d. What is the electrostatic energy of the system? The electrostatic energy $U$ is the integral of the energy density over all space:


$$U = \frac{\epsilon_0}{2} \int E^2 dV = \frac{\epsilon_0}{2} \int_0^R \alpha^2 (4\pi r^2) dr = \frac{\epsilon_0}{2} 4\pi\alpha^2 \left[\frac{r^3}{3}\right]_0^R = \frac{2\pi\epsilon_0\alpha^2 R^3}{3}$$

.

---

### **Question 1.2**

For the following potentials, calculate the electric field and charge density at every point in space:

a. $\varphi(x,y,z) = ax^3z + b\ln(y)$ in Cartesian coordinates ($a,b$ are constants):

* 
**Electric Field:** $\vec{E} = -\vec{\nabla}\varphi = -3ax^2z\hat{x} - \frac{b}{y}\hat{y} - ax^3\hat{z}$.


* 
**Charge Density:** $\rho = \epsilon_0 \vec{\nabla} \cdot \vec{E} = -\epsilon_0 \left(\frac{\partial E_x}{\partial x} + \frac{\partial E_y}{\partial y} + \frac{\partial E_z}{\partial z}\right) = \epsilon_0\left(\frac{b}{y^2} - 6axz\right)$.



b. $\varphi(r,\theta,z) = cr^2z\cos(\theta)$ in cylindrical coordinates ($c$ is constant):

* 
**Electric Field:** $\vec{E} = -\vec{\nabla}\varphi = -2crz\cos(\theta)\hat{r} + crz\sin(\theta)\hat{\theta} - cr^2\cos(\theta)\hat{z}$.


* 
**Charge Density:** $\rho = \epsilon_0 \vec{\nabla} \cdot \vec{E} = \epsilon_0 \left(\frac{1}{r}\frac{\partial}{\partial r}(r E_r) + \frac{1}{r}\frac{\partial E_\theta}{\partial \theta} + \frac{\partial E_z}{\partial z}\right)$.



$$\rho = -\epsilon_0 (4cz\cos(\theta) - cz\cos(\theta) + 0) = -3\epsilon_0 cz\cos(\theta)$$


.



c. $\varphi(r,\theta,\phi) = \frac{k}{r}$ in spherical coordinates ($k$ is constant). Did you get a logical result? If not, try to think why. 

* 
**Electric Field:** $\vec{E} = -\vec{\nabla}\varphi = \frac{k}{r^2}\hat{r}$.


* **Charge Density:** $\rho = \epsilon_0 \vec{\nabla} \cdot \vec{E}$. Using the divergence of $\frac{\hat{r}}{r^2}$ yields a Dirac delta function: $\rho = 4\pi\epsilon_0 k \delta^3(\vec{r})$.


* 
**Logical Result:** Yes, this is logical. This potential corresponds to a point charge of $q = 4\pi\epsilon_0 k$ located at the origin. If calculated without considering the singularity at the origin, you might mistakenly find the charge density to be zero everywhere, missing the point charge.



---

### **Question 1.3**

Given an inverted hollow cone shell with uniform surface charge density $\sigma$, height $h$, and radius $h$. Find the potential difference between the apex of the cone (point a) and the center of the cone's base (point b).

Placing the apex at the origin, the surface slant angle is 45 degrees (since radius equals height). The surface element is $ds = r d\theta dl = z \sqrt{2} dz d\theta$.

* 
**Potential at apex (a):** The distance from any surface element to the apex is $r_a = \sqrt{2}z$.



$$V_a = \int \frac{k dq}{r_a} = \int_0^{2\pi} \int_0^h \frac{k \sigma (z \sqrt{2} dz d\theta)}{\sqrt{2}z} = 2\pi k \sigma \int_0^h dz = 2\pi k \sigma h = \frac{\sigma h}{2\epsilon_0}$$


.


* 
**Potential at base center (b):** The distance to $z=h$ is $r_b = \sqrt{z^2 + (h-z)^2}$.



$$V_b = \int_0^{2\pi} \int_0^h \frac{k \sigma (z \sqrt{2} dz d\theta)}{\sqrt{z^2 + (h-z)^2}} = 2\pi k \sigma \sqrt{2} \int_0^h \frac{z dz}{\sqrt{2z^2 - 2hz + h^2}}$$


.
Solving the integral yields $V_b = 2\pi k \sigma h \ln(\sqrt{2}+1) = \frac{\sigma h}{2\epsilon_0}\ln(\sqrt{2}+1)$.


* 
**Potential Difference:** 
$$\Delta V = V_a - V_b = \frac{\sigma h}{2\epsilon_0} (1 - \ln(\sqrt{2}+1))$$


.



---

### **Question 1.4**

Given a solid sphere of radius $R$ with volumetric charge density $\rho = \rho_0 r^2$.

a. Find the potential on the boundary of the sphere (reference at infinity). First, find the total charge $Q = \int_0^R \rho_0 r^2 (4\pi r^2) dr = \frac{4\pi\rho_0 R^5}{5}$.
The potential on the surface acts like a point charge: $V(R) = \frac{kQ}{R} = \frac{\rho_0 R^4}{5\epsilon_0}$.

b. Find the potential at the center of the sphere (reference at infinity). The internal field using Gauss's law is $E(r) = \frac{1}{4\pi\epsilon_0 r^2} \int_0^r \rho_0 r'^2 (4\pi r'^2) dr' = \frac{\rho_0 r^3}{5\epsilon_0}$.


$$V(0) = V(R) + \int_0^R E(r) dr = \frac{\rho_0 R^4}{5\epsilon_0} + \frac{\rho_0 R^4}{20\epsilon_0} = \frac{\rho_0 R^4}{4\epsilon_0}$$

.

c. What is the potential difference between $r=2R$ and $r=3R$? Outside the sphere, $V(r) = \frac{kQ}{r}$.

* 
$V(2R) = \frac{\rho_0 R^4}{10\epsilon_0}$.


* 
$V(3R) = \frac{\rho_0 R^4}{15\epsilon_0}$.


* Difference: $V(2R) - V(3R) = \frac{\rho_0 R^4}{30\epsilon_0}$.



d. Now we set the reference point at $\tau = \frac{\sqrt{\pi}}{\ln(aR)}$. What is the potential difference between $r=3R$ and $r=2R$? The potential difference between two physical points is strictly independent of the chosen reference point. Therefore, the difference remains unchanged: $\frac{\rho_0 R^4}{30\epsilon_0}$.

---

### **Question 1.5**

A rod of length $L$ carrying charge $Q$ is laid along the x-axis from $x=0$ to $x=L$. Calculate the electric potential at a distance $d$ from the edge ($x=-d$), assuming reference is at infinity.

a. Uniform charge density:
The charge density is $\lambda = \frac{Q}{L}$.


$$V = \int_0^L \frac{k\lambda dx}{x - (-d)} = k\lambda \int_0^L \frac{dx}{x+d} = k\lambda \ln\left(\frac{L+d}{d}\right) = \frac{Q}{4\pi\epsilon_0 L} \ln\left(1 + \frac{L}{d}\right)$$

.

b. Charge density $\lambda = ax$:


$$V = \int_0^L \frac{k(ax) dx}{x+d} = ka \int_0^L \left(1 - \frac{d}{x+d}\right) dx = ka \left[L - d\ln\left(1 + \frac{L}{d}\right)\right]$$

.

---

### **Question 1.6**

Given a hollow disk (annulus) with inner radius $a$ and outer radius $b$, uniformly charged with surface density $\sigma$.

a. Find the electric field at height $z$ above the disk. By integrating ring elements, the symmetry cancels the radial components:


$$E_z = \int_a^b \frac{k (2\pi r \sigma dr)}{r^2+z^2} \frac{z}{\sqrt{r^2+z^2}} = 2\pi k \sigma z \int_a^b \frac{r dr}{(r^2+z^2)^{3/2}} = \frac{\sigma z}{2\epsilon_0} \left(\frac{1}{\sqrt{a^2+z^2}} - \frac{1}{\sqrt{b^2+z^2}}\right)\hat{z}$$

.

b. Find the potential at height $z$ (reference at infinity). 

$$V(z) = \int_a^b \frac{k (2\pi r \sigma dr)}{\sqrt{r^2+z^2}} = 2\pi k \sigma \left[\sqrt{r^2+z^2}\right]_a^b = \frac{\sigma}{2\epsilon_0} \left(\sqrt{b^2+z^2} - \sqrt{a^2+z^2}\right)$$

.

c. Prove that $\vec{E} = -\vec{\nabla}V$. Taking the negative z-derivative of the potential from section b:


$$-\frac{\partial V}{\partial z} = -\frac{\sigma}{2\epsilon_0} \left(\frac{z}{\sqrt{b^2+z^2}} - \frac{z}{\sqrt{a^2+z^2}}\right) = \frac{\sigma z}{2\epsilon_0} \left(\frac{1}{\sqrt{a^2+z^2}} - \frac{1}{\sqrt{b^2+z^2}}\right)$$

. This perfectly matches the $E_z$ derived in section a.

d. Show the field and potential in the limit $a \to 0$. What is the meaning of this limit? 

* 
**Field:** $E_z = \frac{\sigma}{2\epsilon_0} \left(\frac{z}{|z|} - \frac{z}{\sqrt{b^2+z^2}}\right)$.


* 
**Potential:** $V(z) = \frac{\sigma}{2\epsilon_0} (\sqrt{b^2+z^2} - |z|)$.


* 
**Meaning:** This limit represents closing the inner hole, effectively transforming the annulus into a solid disk of radius $b$.



---

### **Question 2.1**

Given a system of two point charges of charge $q$ (an electric dipole). Draw the field lines and explain where the field magnitude is strong and weak. 

* 
**Field Lines:** The lines emerge from the positive charge and curve to terminate at the negative charge.


* 
**Magnitude:** The electric field is strongest in the region directly between the two charges because the field line density is highest there (the contributions from both charges point in the same direction and constructively add). The field is weaker further away from the center of the dipole where the lines spread outwards.



---

### **Question 2.2**

Given a rod of length $2l$ carrying charge density $\lambda = \lambda_0 y$. The rod is centered at $y=0$ (the origin). 

a. Find the dipole moment of the system. 

$$\vec{p} = \int \vec{r} dq = \int_{-l}^l (y\hat{y}) (\lambda_0 y dy) = \lambda_0 \hat{y} \left[\frac{y^3}{3}\right]_{-l}^l = \frac{2\lambda_0 l^3}{3} \hat{y}$$

.

b. Prove that even if the origin is placed at $(a,0)$, you get the same dipole moment. The total charge of the rod is $Q = \int_{-l}^l \lambda_0 y dy = 0$. It is a fundamental property of multipole expansions that for any system with a net charge of zero, the calculated dipole moment vector is strictly invariant to the choice of the coordinate origin.

---

### **Question 2.3**

Find the dipole moment of a spherical shell of radius $R$ carrying a surface charge density $\sigma = \sigma_0 \cos(\theta)$. 

By symmetry, the resulting dipole moment will align purely along the z-axis.


$$\vec{p} = \int \vec{r} dq = \int_0^{2\pi} \int_0^\pi (R\cos\theta\hat{z}) (\sigma_0 \cos\theta) (R^2 \sin\theta d\theta d\phi)$$

.


$$p_z = 2\pi R^3 \sigma_0 \int_0^\pi \cos^2\theta \sin\theta d\theta = 2\pi R^3 \sigma_0 \left[-\frac{\cos^3\theta}{3}\right]_0^\pi = 2\pi R^3 \sigma_0 \left(\frac{1}{3} - \left(-\frac{1}{3}\right)\right) = \frac{4\pi \sigma_0 R^3}{3}$$

.


$$\vec{p} = \frac{4\pi \sigma_0 R^3}{3} \hat{z}$$

.