### **Question 1.1**

Given electric field and cube side length $a$:

$$ \vec{E}=x\hat{x}+xy\hat{y}+xyz\hat{z} $$

**A.** Divergence theorem:

$$ \Phi = \iiint \nabla \cdot \vec{E} \,dV $$

$$ \nabla \cdot \vec{E} = \frac{\partial E_x}{\partial x} + \frac{\partial E_y}{\partial y} + \frac{\partial E_z}{\partial z} = 1 + x + xy $$

Volume integral ($0 \le x, y, z \le a$):

$$ \Phi = \int_0^a \int_0^a \int_0^a (1 + x + xy) \,dx \,dy \,dz $$

$$ \int_0^a (1 + x + xy) \,dx = a + \frac{a^2}{2} + \frac{a^2 y}{2} $$

$$ \int_0^a \left( a + \frac{a^2}{2} + \frac{a^2 y}{2} \right) \,dy = a^2 + \frac{a^3}{2} + \frac{a^4}{4} $$

$$ \int_0^a \left( a^2 + \frac{a^3}{2} + \frac{a^4}{4} \right) \,dz = a^3 + \frac{a^4}{2} + \frac{a^5}{4} $$

For $a=2m$:

$$ \Phi = 2^3 + \frac{2^4}{2} + \frac{2^5}{4} = 24 \, \left[\frac{N \cdot m^2}{C}\right] $$

**B.** Gauss's Law:

$$ \Phi = \frac{Q_{in}}{\epsilon_0} $$

$$ Q_{in} = 24\epsilon_0 \, [C] $$

---

### **Question 1.2**

Point charge $q$ in spherical shell $r=1[m]$. Total flux:

$$ \Phi_{total} = \frac{q}{\epsilon_0} $$

For a shell cut in half, by symmetry:

$$ \Phi = \frac{q}{2\epsilon_0} $$

---

### **Question 2.1**

Solid cylinder field ($r < R$):

$$ \vec{E} = \frac{\rho r}{2\epsilon_0} \hat{r} $$

Solid cylinder field ($r > R$):

$$ \vec{E} = \frac{\rho R^2}{2\epsilon_0 r} \hat{r} $$

Superposition of solid cylinder ($\rho$) and hole ($-\rho$):

**B.** Center of large cylinder ($x=0$):

$$ \vec{E}_A = 0 + \frac{(-\rho) (R/4)}{2\epsilon_0} (-\hat{x}) = \frac{\rho R}{8\epsilon_0} \hat{x} $$

**C.** Center of hole ($x=R/4$):

$$ \vec{E}_B = \frac{\rho (R/4)}{2\epsilon_0} \hat{x} + 0 = \frac{\rho R}{8\epsilon_0} \hat{x} $$

**D.** Edge of cylinder ($x=R$):

$$ \vec{E}_C = \frac{\rho R}{2\epsilon_0} \hat{x} + \frac{(-\rho) (R/4)^2}{2\epsilon_0 (3R/4)} \hat{x} = \frac{11\rho R}{24\epsilon_0} \hat{x} $$

**E.** Point D ($x=2R$):

$$ \vec{E}_D = \frac{\rho R^2}{2\epsilon_0 (2R)} \hat{x} + \frac{(-\rho) (R/4)^2}{2\epsilon_0 (7R/4)} \hat{x} = \frac{13\rho R}{56\epsilon_0} \hat{x} $$

---

### **Question 2.2**

System of two spheres: $R_1$ with $\rho$, $R_2$ with $-\rho$. Distance between centers $d = R_1 + L + R_2$.

**A.** Center of small sphere:

$$ \vec{E} = \frac{1}{4\pi\epsilon_0} \frac{\frac{4}{3}\pi R_1^3 \rho}{(R_1 + L + R_2)^2} \hat{x} = \frac{\rho R_1^3}{3\epsilon_0 (R_1 + L + R_2)^2} \hat{x} $$

**B.** Point A (middle of $L$):

$$ \vec{E}_A = \frac{\rho R_1^3}{3\epsilon_0 (R_1 + L/2)^2} \hat{x} + \frac{\rho R_2^3}{3\epsilon_0 (R_2 + L/2)^2} \hat{x} $$

Spheres merged: $R_2 = R_1/2$. Overlap field:

$$ \vec{E}_{overlap} = \frac{\rho}{3\epsilon_0}\left(\frac{R_1}{2} \hat{x}\right) = \frac{\rho R_1}{6\epsilon_0}\hat{x} $$

**C.** Center of large sphere:

$$ \vec{E} = \frac{\rho R_1}{6\epsilon_0} \hat{x} $$

**D.** Point A (center of small sphere):

$$ \vec{E}_A = \frac{\rho R_1}{6\epsilon_0} \hat{x} $$

**E.** Point B $(0, R_1)$:

Large sphere field:

$$ \vec{E}_1 = \frac{\rho R_1}{3\epsilon_0} \hat{y} $$

Small sphere field (center at $R_1/2, 0$, distance $r' = \frac{\sqrt{5}}{2}R_1$):

$$ \vec{E}_2 = \frac{1}{4\pi\epsilon_0} \frac{-\frac{4}{3}\pi (R_1/2)^3 \rho}{(r')^3} \left(-\frac{R_1}{2}\hat{x} + R_1\hat{y}\right) = \frac{\rho R_1}{30\sqrt{5}\epsilon_0} \hat{x} - \frac{2\rho R_1}{30\sqrt{5}\epsilon_0} \hat{y} $$

Total Field:

$$ \vec{E}_B = \vec{E}_1 + \vec{E}_2 $$

---

### **Question 3**

Differential Gauss's Law in spherical coordinates:

$$ \rho = \epsilon_0 \nabla \cdot \vec{E} = \epsilon_0 \frac{1}{r^2} \frac{\partial}{\partial r} (r^2 E_r) $$

For $r < R$, $E_r = \frac{2}{5\epsilon_0}\sqrt{r}$:

$$ \frac{\partial}{\partial r} \left( r^2 \cdot \frac{2}{5\epsilon_0} r^{1/2} \right) = \frac{2}{5\epsilon_0} \cdot \frac{5}{2} r^{3/2} = \frac{1}{\epsilon_0} r^{3/2} $$

$$ \rho(r) = \epsilon_0 \frac{1}{r^2} \left( \frac{1}{\epsilon_0} r^{3/2} \right) = \frac{1}{\sqrt{r}} $$

For $r > R$:

$$ \rho(r) = 0 $$

---

### **Question 4**

Electron cloud charge $-e$:

$$ -e = \int_0^\infty 4\pi c r^2 e^{-\frac{2r}{a_0}} dr $$

Using integral limit $l \to \infty$:

$$ \int_0^\infty x^2 e^{-kx} dx = \frac{2}{k^3} = \frac{2}{(2/a_0)^3} = \frac{a_0^3}{4} $$

**A.** Constant C:

$$ -e = 4\pi c \left( \frac{a_0^3}{4} \right) \implies c = -\frac{e}{\pi a_0^3} $$

**B.** Electric Field (enclosed charge includes nucleus $+e$ and cloud):

$$ Q_{enc} = e + \int_0^r 4\pi c r'^2 e^{-\frac{2r'}{a_0}} dr' $$

Using hint integral:

$$ Q_{enc} = e \cdot e^{-\frac{2r}{a_0}} \left( 1 + \frac{2r}{a_0} + \frac{2r^2}{a_0^2} \right) $$

$$ \vec{E}(r) = \frac{e}{4\pi\epsilon_0 r^2} e^{-\frac{2r}{a_0}} \left( 1 + \frac{2r}{a_0} + \frac{2r^2}{a_0^2} \right) \hat{r} $$

**C.** Field at $r = a_0$:

$$ \vec{E}(a_0) = \frac{e}{4\pi\epsilon_0 a_0^2} e^{-2} (1 + 2 + 2) \hat{r} = \frac{5e}{4\pi\epsilon_0 a_0^2 e^2} \hat{r} $$