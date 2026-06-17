## 1.
![[Pasted image 20260614162601.png]]

## a.
$$
\vec{J}=\sigma \cdot \vec{E}=\sigma_{0}\left( 1-\frac{r}{R} \right) \cdot E_{0}\hat{z}
$$

---
## b.
$$
I=\int \int \vec{J}\cdot d\vec{s} $$
$$= \sigma_{0}E_{0}\int ^{R}_{0}\int ^{2\pi}_{0}\left( 1-\frac{r}{R} \right)r d\theta dr \hat{z}\cdot \hat{z}=2\pi \sigma_{0}E_{0}\int^R_{0}r-\frac{r^{2}}{R}dr
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

---
# 2.
![[Pasted image 20260614163120.png]]
## a.
$$
R=\rho\frac{ L}{A}
$$

$$
dR = \rho \frac{dr}{L \cdot 2\pi r}
$$

$$R = \int dR = \frac{\rho}{L \cdot 2\pi} \cdot \int_{a}^{b} \frac{dr}{r} = \frac{\rho}{2\pi L} \ln{\frac{b}{a}}$$

---
## b.

$$I = \frac{V}{R} = \frac{V \cdot 2\pi L}{\rho \cdot \ln(b/a)}$$

---
## c.
$$\vec{j} = \frac{I}{2\pi r \cdot L} = \frac{V}{\rho \cdot \ln(b/a)} \cdot \frac{\hat{r}}{r}$$

---
## d.
$$
\vec{J}=\sigma \vec{E}
$$
$$
\vec{E}=\frac{\vec{J}}{\sigma}=\rho\vec{J}=\frac{V}{\ln(b/a)}\cdot \frac{\hat{r}}{r}
$$

---
# 3.
![[Pasted image 20260614163051.png]]
$$
dR=\frac{\frac{\rho_{0}z}{r}dz}{2\pi rdr} 
$$
$$
dR=\frac{\rho_{0} \frac{1}{2}L^2}{2\pi r^2dr} 
$$
$$
\frac{1}{dR}=\frac{4\pi}{\rho_{0}L^2}r^2dr
$$
$$
\frac{1}{R}=\frac{4\pi}{\rho_{0}L^2} \frac{a^3}{3}
$$
$$
R=\frac{3\rho_{0}L^2}{4\pi a^3}
$$
$$
I=\frac{V}{R}=\frac{4\pi Va^3}{3\rho_{0}L^2}
$$

---
# 4.
![[Pasted image 20260614163605.png]]
Let's calculate the voltage drop across resistor $R_3$:

$$\varphi_3 = R_3 \cdot I_3 = 4[\Omega] \cdot 6[A] \Rightarrow \varphi_3 = 24[V]$$

The voltage drop across resistor $R_2$ and the box is identical to the voltage drop across resistor $R_3$, now we can find the voltage drop across resistor $R_1$ which is:

$$\varphi_1 = \varphi_A - \varphi_B - \varphi_3 = 78[V] - 24[V] \Rightarrow \varphi_1 = 54[V]$$

And the current through resistor $R_1$ is:

$$I_1 = \frac{\varphi_1}{R_1} = \frac{54[V]}{7[\Omega]} \Rightarrow I_1 = \frac{54}{7}[A]$$

We found that the current through resistor $R_1$ is greater than the current through $R_3$! This means there is a splitting of the current at the junction between $R_2$ and $R_3$. The current flowing through the top branch ($R_2$ and the Box) is:

$$I_{top} = I_1 - I_3 = \frac{54}{7}[A] - \frac{42}{7}[A] \Rightarrow I_{top} = \frac{12}{7}[A]$$

Now we can find the voltage drop across resistor $R_2$:

$$\varphi_{R2} = R_2 \cdot I_{top} = 6[\Omega] \cdot \frac{12}{7}[A] \Rightarrow \varphi_{R2} = \frac{72}{7}[V]$$

The remaining voltage drop in that branch must be across the Box:

$$\varphi_{Box} = \varphi_3 - \varphi_{R2} = 24[V] - \frac{72}{7}[V] \Rightarrow \varphi_{Box} = \frac{96}{7}[V]$$

Finally, we can calculate the resistance of the Box using Ohm's Law:

$$R_{Box} = \frac{\varphi_{Box}}{I_{top}} = \frac{96/7[V]}{12/7[A]} \Rightarrow R_{Box} = 8[\Omega]$$

Since the component in the box has a constant, exact resistance of $8\Omega$, it acts as a standard resistor. Therefore, answer 'A' is correct.

---
# 5.
![[Pasted image 20260614163649.png]]

Because everything is connected in a single loop (series), this complex circuit behaves exactly like a simple circuit that has only one resistor and one capacitor.

First, smash the components together into single, equivalent values:

- **Total Resistance ($R_{eq}$):** Resistors in series just add together.
    
    $$R_{eq} = R_1 + R_2$$
    
- **Total Capacitance ($C_{eq}$):** Capacitors in series combine inversely.
    
    $$C_{eq} = \frac{C_1 C_2}{C_1 + C_2}$$
    


In a series circuit, the current is the same everywhere, and both capacitors will store the exact same amount of charge. Because we simplified the circuit in Step 1, we don't need to write a new differential equation; we can just plug $R_{eq}$ and $C_{eq}$ directly into the standard physics formulas for a charging capacitor:

- **Standard Charge Formula:** $Q(t) = V C_{eq} \left(1 - e^{-\frac{t}{R_{eq}C_{eq}}}\right)$
    
- **Standard Current Formula:** $I(t) = \frac{V}{R_{eq}} e^{-\frac{t}{R_{eq}C_{eq}}}$
    


Just substitute your $R_{eq}$ and $C_{eq}$ values back into those standard formulas to get your final, full equations:

**Charge on both capacitors:**

$$Q_1(t) = Q_2(t) = V \left( \frac{C_1 C_2}{C_1 + C_2} \right) \left[ 1 - \exp\left(-\frac{t}{(R_1 + R_2) \left(\frac{C_1 C_2}{C_1 + C_2}\right)}\right) \right]$$

**Current in the circuit:**

$$I(t) = \frac{V}{R_1 + R_2} \exp\left(-\frac{t}{(R_1 + R_2) \left(\frac{C_1 C_2}{C_1 + C_2}\right)}\right)$$

---
# 6.
![[Pasted image 20260614164905.png]]
## a.
- **When the switch is OPEN for a long time:**
    
    The right branch (with $R_2$) is disconnected. The circuit consists only of the voltage source $V_0$, resistor $R_1$, and capacitor $C$ in series. Since the capacitor acts as an open circuit, no current flows through $R_1$, meaning there is zero voltage drop across $R_1$.
    
    Therefore, the capacitor charges fully to the source voltage:
    
    $$V_c(\text{open}) = V_0$$
    
- **When the switch is CLOSED for a long time:**
    
    The capacitor acts as an open circuit, so no current flows down its specific branch. However, current _does_ flow in the outer loop from $V_0$ through $R_1$ and $R_2$ to ground. This forms a standard voltage divider. The capacitor is in parallel with $R_2$, so it measures the voltage drop across $R_2$:
    
    $$V_c(\text{closed}) = V_0 \left( \frac{R_2}{R_1 + R_2} \right)$$
    
---
## b.

The time constant of an RC circuit is given by $\tau = R_{eq}C$, where $R_{eq}$ is the Thevenin equivalent resistance seen from the perspective of the capacitor (with the voltage source shorted to ground).

- **Switch OPEN ($\tau_1$):**
    
    With the switch open, the $R_2$ branch is gone. From the capacitor's perspective (shorting $V_0$ to ground), it only "sees" $R_1$.
    
    $$\tau_1 = R_1 C$$
    
- **Switch CLOSED ($\tau_2$):**
    
    With the switch closed, short $V_0$ to ground to find the equivalent resistance. From the capacitor's perspective, it looks back and sees $R_1$ connected to ground on one side, and $R_2$ connected to ground on the other side. Therefore, $R_1$ and $R_2$ are in parallel.
    
    $$\tau_2 = \left( \frac{R_1 R_2}{R_1 + R_2} \right) C$$
    
---
## c.

Here, the switching period $T$ is **much shorter** than the time constants. This means the capacitor doesn't have time to fully charge or discharge before the switch changes state.
![[Pasted image 20260614175348.png]]

---
## d.


Here, the switching period $T$ is **much longer** than the time constants. This means the capacitor has plenty of time to reach its final steady-state voltage in every single cycle.

![[Pasted image 20260614175321.png]]


---
## e.

- **Scenario 1: $R_1 \ll R_2$ (or $R_2$ is very large)**
    
    If $R_2$ is huge compared to $R_1$, the closed-switch steady state becomes:
    
    $$V_c(\text{closed}) = V_0 \left( \frac{R_2}{R_1 + R_2} \right) \approx V_0 \left( \frac{R_2}{R_2} \right) = V_0$$
    
    **Explanation:** $R_2$ is essentially acting like an open circuit anyway because its resistance is so high. Closing the switch barely draws any current away from the capacitor. Therefore, the capacitor voltage will remain almost constantly at $V_0$ regardless of whether the switch is open or closed.
    
- **Scenario 2: $R_2 \ll R_1$ (or $R_2$ is very small)**
    
    If $R_2$ is tiny compared to $R_1$, the closed-switch steady state becomes:
    
    $$V_c(\text{closed}) = V_0 \left( \frac{R_2}{R_1 + R_2} \right) \approx V_0 \left( \frac{0}{R_1} \right) = 0$$
    
    **Explanation:** Closing the switch essentially creates a short circuit to ground across the capacitor. The capacitor will rapidly and completely drain all its charge through $R_2$, dropping the voltage to $0V$. When the switch opens, it charges back to $V_0$. The circuit acts like an aggressive on/off switch for the capacitor voltage.