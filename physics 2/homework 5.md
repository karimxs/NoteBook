# 1.
A conducting sphere of radius $R$ is charged with a charge $Q$ and is surrounded by a neutral conducting spherical shell (with no initial charges) having an inner radius $a$ and an outer radius $b$ (where $R < a < b$).
![[Pasted image 20260602145545.png]]
## a. 
Find the surface charge densities $\sigma_a, \sigma_b, \sigma_R$.


$$\sigma_R = \frac{Q}{4\pi R^2}$$

$$\sigma_a = \frac{-Q}{4\pi a^2}$$

$$\sigma_b = \frac{Q}{4\pi b^2}$$

---
## b.
Find the potential at the center of the sphere (reference point at infinity).


$$V_O = \frac{kQ}{R} - \frac{kQ}{a} + \frac{kQ}{b} = kQ\left(\frac{1}{R} - \frac{1}{a} + \frac{1}{b}\right)$$

---
## c.

What is the electric field on the outer shell ($r = b$) and also on the inner shell ($r = a$)?

$$E_b = \frac{kQ}{b^2}$$

$$E_a = \frac{kQ}{a^2}$$

---
## d. 
The outer shell is grounded to the earth with a conductor. How will the answers to sections a and b change?

**Changes to section a:**

$\sigma_R$ and $\sigma_a$ remain unchanged, but the charge on the outer surface becomes zero.

$$\sigma_R = \frac{Q}{4\pi R^2}$$

$$\sigma_a = \frac{-Q}{4\pi a^2}$$

$$\sigma_b = 0$$

**Changes to section b:**

The new potential at the center of the sphere is:

$$V_O = kQ\left(\frac{1}{R} - \frac{1}{a}\right)$$

---
# 2.

Given an uncharged conducting sphere of radius $R$ with two holes hollowed out of it, one of radius $a$ and the second of radius $b$, as shown in the figure:

A charge is placed at the center of each hole, $q_a$ at the center of the hole with radius $a$ and $q_b$ at the center of the hole with radius $b$.
![[Pasted image 20260602150734.png]]
## a. Find the surface charge density of the conductor $\sigma_a, \sigma_b, \sigma_R$.

$$\sigma_a = \frac{-q_a}{4\pi a^2}$$

$$\sigma_b = \frac{-q_b}{4\pi b^2}$$

$$\sigma_R = \frac{q_a + q_b}{4\pi R^2}$$

---
## b. What is the electric field outside the conducting sphere?

$$E = \frac{k(q_a + q_b)}{r^2}$$

---
## c. What is the net force acting on the charges $q_a, q_b$?

$$F_a = 0$$

$$F_b = 0$$

---
![[Pasted image 20260602150843.png]]
## d. Assuming a charge $q_c$ is brought near the conductor but not into it, what will change in sections a-c?

- **Section a:** $\sigma_a$ and $\sigma_b$ will not change. $\sigma_R$ will change (the charge distribution on the outer surface will no longer be uniform, though the total charge remains the same).
    
- **Section b:** The electric field outside the sphere will change (it will now be influenced by $q_c$ and the non-uniform distribution of $\sigma_R$).
    
- **Section c:** The net force on $q_a$ and $q_b$ will not change (it remains $0$ due to the electrostatic shielding of the conductor).

---
![[Pasted image 20260602150938.png]]
## e. If the spherical shell of the conductor is grounded with respect to infinity (without the charge from section d), how will the answers in sections a-c change?

- **Section a:** $\sigma_a$ and $\sigma_b$ will not change. $\sigma_R$ will change to $0$.
    
- **Section b:** The electric field outside the sphere will change to $0$.
    
- **Section c:** The net force on $q_a$ and $q_b$ will not change (it remains $0$).

---
# 3.
Given three conducting spheres of radius $R_1, R_2, R_3$. The spheres are connected to each other by long, thin conducting wires, and the spheres are very far apart from each other. It is known that the first sphere is charged with a charge $Q_1$. Calculate the total charge $Q$ on the three spheres.

$$V_1 = V_2 = V_3$$

$$V_1 = \frac{kQ_1}{R_1}$$

$$\frac{kQ_1}{R_1} = \frac{kQ_2}{R_2} \Rightarrow Q_2 = \frac{R_2 Q_1}{R_1}$$

$$\frac{kQ_1}{R_1} = \frac{kQ_3}{R_3} \Rightarrow Q_3 = \frac{R_3 Q_1}{R_1}$$

$$Q_{total} = Q_1 + Q_2 + Q_3$$

$$Q_{total} = Q_1 + \frac{R_2 Q_1}{R_1} + \frac{R_3 Q_1}{R_1}$$

$$Q_{total} = \frac{Q_1 R_1 + R_2 Q_1 + R_3 Q_1}{R_1}$$

---
