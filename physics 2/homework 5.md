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
![[Pasted image 20260602151509.png]]

$$V_1 = V_2 = V_3$$

$$V_1 = \frac{kQ_1}{R_1}$$

$$\frac{kQ_1}{R_1} = \frac{kQ_2}{R_2} \Rightarrow Q_2 = \frac{R_2 Q_1}{R_1}$$

$$\frac{kQ_1}{R_1} = \frac{kQ_3}{R_3} \Rightarrow Q_3 = \frac{R_3 Q_1}{R_1}$$

$$Q_{total} = Q_1 + Q_2 + Q_3$$

$$Q_{total} = Q_1 + \frac{R_2 Q_1}{R_1} + \frac{R_3 Q_1}{R_1}$$

$$Q_{total} = \frac{Q_1 R_1 + R_2 Q_1 + R_3 Q_1}{R_1}$$
![[Pasted image 20260602151528.png]]

---
# 4.

Given the following system: An insulating sphere of radius $R_1$ charged with a spherically symmetric volume charge density $\rho(r)$:

$$\rho(r) = a \cdot r^3 \quad \text{(where } a > 0 \text{ for } 0 \le r \le R_1 \text{)}$$

And surrounding it is a thin conducting, grounded spherical shell of radius $R_2$ (where $R_2 > R_1$). The center of the shell is identical to the center of the sphere.

## a. What is the total charge of the insulating sphere?

$$Q_{in} = \frac{2\pi a R_1^6}{3}$$

---
## b. What is the total charge on the shell?

$$Q_{shell} = -Q_{in} = -\frac{2\pi a R_1^6}{3}$$

---
## c. What is the electric field at every point in space?

For $0 \le r \le R_1$:

$$E = \frac{a r^4}{6\epsilon_0}$$

For $R_1 < r < R_2$:

$$E = \frac{a R_1^6}{6\epsilon_0 r^2}$$

For $r \ge R_2$:

$$E = 0$$

---
## d. What is the potential energy of the system?

$$U = \frac{\pi a^2 R_1^{11}}{198\epsilon_0} + \frac{\pi a^2 R_1^{12}}{18\epsilon_0} \left(\frac{1}{R_1} - \frac{1}{R_2}\right)$$

---
## e. What is the work required to move a positive charge $q$ along the path $A \to C \to D \to E$ described in the drawing?

The electrostatic field is conservative, so the work depends only on the initial and final points ($A$ and $E$).

$$W_{A \to E} = q(V_E - V_A)$$

$$V_E = 0$$

$$V_A = \frac{a R_1^6}{6\epsilon_0} \left(\frac{1}{R_1} - \frac{1}{R_2}\right)$$

$$W = -q \frac{a R_1^6}{6\epsilon_0} \left(\frac{1}{R_1} - \frac{1}{R_2}\right)$$

---
# 5.

Given two conducting spheres far apart from each other. The radius of the first sphere is $2R$ and it is charged with a charge $3Q$. The radius of the second sphere is $R$ and it is charged with a charge $-Q$. The two spheres were connected by a thin, long conducting wire, and after the system stabilized, they were disconnected from each other.

## a.

Calculate the initial energy of the system (before connecting the spheres).

$$U_{initial} = \frac{11kQ^2}{4R}$$

---
## b.

Calculate the charge on each sphere after connecting them.

$$q_1' = \frac{4}{3}Q$$

$$q_2' = \frac{2}{3}Q$$

---
## c.

Calculate the final energy of the system.

$$U_{final} = \frac{2kQ^2}{3R}$$

---
## d.

Bonus: Under the conditions of the problem, the two spheres are isolated from their surroundings. How is it possible that the answers to sections a and c are different? Is this not a contradiction to the law of conservation of energy?

This is not a contradiction to the law of conservation of energy. The difference in electrostatic potential energy is dissipated as heat (due to the resistance of the wire) or as electromagnetic radiation while the charges are moving between the spheres to reach equilibrium.