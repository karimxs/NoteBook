
# 1.
![[Pasted image 20260621121843.png]]
## a.
$$
\begin{cases}
\vec{B}=B_{0} \\
\vec{E}=0 \\
F_{B}=\vec{E}\cdot q+qv \times \vec{B}
\end{cases}
$$
Since the velocity vector is perpendicular to the magnetic field vector we get:
$$
F_{B}=qvB_{0}
$$
According to Newton second law:
$$
F=m\cdot a
$$
$$
qvB_{0}=m \cdot \frac{v^{2}}{R}
$$
$$
R=\frac{mv}{qB_{0}}
$$

---
## b.
In the far distance - in order for the particle to move in a straight path, the net force acting on it must be equal to 0. Therefore,
$$
\sum F=Eq+qv\times B=0
$$
$$
q(E+v\times B)=0
$$
$$
E=-v\times B=B\times v=vB
$$
$$
v=\frac{E}{B}
$$
and we know from a that:
$$
v=\frac{RqB_{0}}{m}
$$
$$
\frac{E}{B}=\frac{RqB_{0}}{m}
$$
$$
m=\frac{RqB_{0}B}{E}
$$

---
# 2.
![[Pasted image 20260622111933.png]]
$$
|F|=|I||L||B|\sin(90)
$$
$$
F=ILB
$$
$$
W=F\cdot a=ILBa
$$
Calculation of the final kinetic energy: 
(Since the body rolls without slipping, therefore):
$$
E_{k}=\frac{1}{2}mv^{2}+\frac{1}{2}I_{m}\omega^{2}
$$
$$
\begin{cases}
I_{m}=\frac{mR^{2}}{2} \\
v=\omega R \Rightarrow \omega=\frac{v}{R}
\end{cases}
$$
$$
E_{k}=\frac{1}{2}\left( mv^{2}+\frac{mR^2}{2}\frac{v^{2}}{R^2} \right)
$$
$$
E_{k}=\frac{3}{4}mv^2
$$
$$
W=\Delta E_{k}=E_{p}-E_{i}
$$
$$
ILBa=\frac{3}{4}mv^{2}-0
$$
$$
v=\sqrt{ \frac{4ILBa}{3m} }
$$

---
# 3.
![[Pasted image 20260622115252.png]]
## a.

$$\oint \vec{B} \cdot d\vec{l} = \mu_0 I_{in}$$

**Inside the conductor ($r < R$):**

The left side of Ampere's Law is the line integral of the magnetic field along a circular loop of radius $r$:

$$\oint \vec{B} \cdot d\vec{l} = B \cdot 2\pi r$$

To find the right side, we calculate the current enclosed ($I_{in}$) by integrating the current density over the cross-sectional area of our loop (where $dS = 2\pi r dr$):

$$I_{in} = \iint \vec{J} \cdot d\vec{S} = \int_0^r (\alpha r)(2\pi r) dr$$

$$I_{in} = 2\pi \alpha \int_0^r r^2 dr$$

$$I_{in} = 2\pi \alpha \frac{r^3}{3}$$

$$B \cdot 2\pi r = \mu_0 \left(2\pi \alpha \frac{r^3}{3}\right)$$

$$\vec{B} = \frac{\mu_0 \alpha r^2}{3} \hat{\theta}$$

**Outside the conductor ($r > R$):**

The left side of Ampere's Law remains the same for our new loop of radius $r$:

$$\oint \vec{B} \cdot d\vec{l} = B \cdot 2\pi r$$

For the enclosed current, we must remember that current only flows up to the physical radius of the cylinder ($R$). There is no current between $R$ and our loop $r$, so we split the integral:

$$I_{in} = \int_0^R (\alpha r)(2\pi r) dr + \int_R^r 0 \cdot 2\pi r dr$$

$$I_{in} = 2\pi \alpha \frac{R^3}{3} + 0$$


$$B \cdot 2\pi r = \mu_0 \left(2\pi \alpha \frac{R^3}{3}\right)$$

$$\vec{B} = \frac{\alpha R^3 \mu_0}{3r} \hat{\theta}$$


Combining the two regions, the magnetic field in all space is:

$$\vec{B} = \begin{cases} \frac{\mu_0 \alpha r^2}{3} \hat{\theta} & : r < R \\ \frac{\alpha R^3 \mu_0}{3r} \hat{\theta} & : r > R \end{cases}$$

---
## b.
![[Pasted image 20260622115610.png]]

$$\vec{J} = \begin{cases} \alpha r & : a < r < R \\ 0 & : r < a \end{cases}$$

**Inside the hollow cavity ($r < a$):**

In this region, there is no current flowing because the space is empty.

$$I_{in} = \iint \vec{J} \cdot d\vec{S} = 0$$

$$B \cdot 2\pi r = 0$$

$$\vec{B} = 0$$

**Inside the conductor ($a < r < R$):**

For a loop within the material of the conductor, we integrate the current density starting from the inner edge $a$ up to our loop radius $r$.

$$I_{in} = \iint \vec{J} \cdot d\vec{S} = \int_a^r (\alpha r)(2\pi r) dr$$

$$I_{in} = 2\pi \alpha \int_a^r r^2 dr$$

$$I_{in} = 2\pi \alpha \left[ \frac{r^3}{3} \right]_a^r$$

$$I_{in} = \frac{2\pi \alpha}{3} (r^3 - a^3)$$


$$B \cdot 2\pi r = \mu_0 \left( \frac{2\pi \alpha}{3} (r^3 - a^3) \right)$$

$$\vec{B} = \frac{\mu_0 \alpha (r^3 - a^3)}{3r} \hat{\theta}$$

**Outside the conductor ($r > R$):**

For a loop outside the entire cylinder, we enclose all the current. We integrate from $0$ to $r$, but since current only exists between $a$ and $R$, the integral splits into three parts (with the empty spaces contributing $0$):

$$I_{in} = \int_0^a 0 \cdot 2\pi r dr + \int_a^R (\alpha r)(2\pi r) dr + \int_R^r 0 \cdot 2\pi r dr$$

$$I_{in} = 0 + 2\pi \alpha \int_a^R r^2 dr + 0$$

$$I_{in} = \frac{2\pi \alpha}{3} (R^3 - a^3)$$



$$B \cdot 2\pi r = \mu_0 \left( \frac{2\pi \alpha}{3} (R^3 - a^3) \right)$$


$$\vec{B} = \frac{\mu_0 \alpha (R^3 - a^3)}{3r} \hat{\theta}$$


Combining the results for all three regions gives the total piecewise function for the magnetic field:

$$\vec{B} = \begin{cases} 0 & : r < a \\ \frac{\alpha(r^3 - a^3)\mu_0}{3r} \hat{\theta} & : a < r < R \\ \frac{\alpha(R^3 - a^3)\mu_0}{3r} \hat{\theta} & : r > R \end{cases}$$

---
# 4.
![[Pasted image 20260622115812.png]]
## a.

$$B = \frac{\mu_0 I}{4\pi R} \theta$$

In this diagram, the arcs span an angle of exactly $\frac{\pi}{2}$ radians ($90^\circ$). Let's break the loop into four parts:

1. **Inner arc (radius $a$):** The current flows counter-clockwise. Using the right-hand rule, the magnetic field points **out of the page**.

$$B_{inner} = \frac{\mu_0 I}{4\pi a} \left(\frac{\pi}{2}\right) = \frac{\mu_0 I}{8a} \text{ (out)}$$

2. **Outer arc (radius $b$):** The current flows clockwise. Using the right-hand rule, the magnetic field points **into the page**.
    
    $$B_{outer} = \frac{\mu_0 I}{4\pi b} \left(\frac{\pi}{2}\right) = \frac{\mu_0 I}{8b} \text{ (in)}$$
    
3. **Two straight radial segments:** These segments point directly towards or away from point P. Since the angle between the current element $d\vec{l}$ and the position vector $\vec{r}$ is $0^\circ$ or $180^\circ$, their cross product is zero. Therefore, they contribute **nothing** to the magnetic field at P.
    
    $$B_{straight} = 0$$
    

To find the total magnetic field, we add the contributions, defining "out of the page" as the positive direction:

$$B_{total} = B_{inner} - B_{outer}$$

$$B_{total} = \frac{\mu_0 I}{8a} - \frac{\mu_0 I}{8b}$$

Factoring out the common terms:

$$\vec{B} = \frac{\mu_0 I}{8} \left( \frac{1}{a} - \frac{1}{b} \right) \text{ (out)}$$

---
## b.


1. **Top semi-infinite straight wire:** The wire stops directly above point P. The magnetic field from a semi-infinite wire at a distance $R$ from its end is half that of an infinite wire.
    
    $$B_{top\_straight} = \frac{1}{2} \left( \frac{\mu_0 I}{2\pi R} \right) = \frac{\mu_0 I}{4\pi R}$$
    
    Using the right-hand rule (thumb points left), the magnetic field at P (below the wire) points **into the page**.
    
2. **Bottom semi-infinite straight wire:** The wire starts directly below point P. Similarly, its contribution is:
    
    $$B_{bottom\_straight} = \frac{\mu_0 I}{4\pi R}$$
    
    Using the right-hand rule (thumb points right), the magnetic field at P (above the wire) also points **into the page**.
    
3. **Semi-circular arc (radius $R$):** The arc spans an angle of $\pi$ radians ($180^\circ$). The current flows counter-clockwise.
    
    $$B_{arc} = \frac{\mu_0 I}{4\pi R} (\pi) = \frac{\mu_0 I}{4R}$$
    
    Using the right-hand rule, the magnetic field points **into the page**.
    

To find the total magnetic field, we add all the contributions together, as they all point in the same direction (into the page):

$$B_{total} = B_{top\_straight} + B_{bottom\_straight} + B_{arc}$$

$$B_{total} = \frac{\mu_0 I}{4\pi R} + \frac{\mu_0 I}{4\pi R} + \frac{\mu_0 I}{4R}$$

$$B_{total} = \frac{2\mu_0 I}{4\pi R} + \frac{\mu_0 I}{4R}$$

Factoring out $\frac{\mu_0 I}{4R}$:

$$\vec{B} = \frac{\mu_0 I}{4R} \left( \frac{2}{\pi} + 1 \right) \text{ (into the page)}$$

Rearranging the terms inside the parentheses gives us:

$$\vec{B} = \frac{\mu_0 I}{4R} \left( 1 + \frac{2}{\pi} \right) \text{ (into the page)}$$
---
# 5.
![[Pasted image 20260622120213.png]]
