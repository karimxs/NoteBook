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
\vec{E}=\frac{\vec{J}}{\sigma}=\rho\vec{J}=\frac{V}{\ln(a/b)}\cdot \frac{\hat{r}}{r}
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

$$\varphi_3 = R_3 \cdot I_3 = 6[\Omega] \cdot 6[A] \Rightarrow \varphi_3 = 36[V]$$

The voltage drop across resistor $R_2$ and the box is identical to the voltage drop across resistor $R_3$, now we can find the voltage drop across resistor $R_1$ which is:

$$\varphi_1 = \varphi_A - \varphi_B - \varphi_3 = 78[V] - 36[V] \Rightarrow \varphi_1 = 42[V]$$

And the current through resistor $R_1$ is:

$$I_1 = \frac{\varphi_1}{R_1} = \frac{42[V]}{7[\Omega]} \Rightarrow I_1 = 6[A]$$

We found that the current through resistor $R_1$ and $R_3$ is identical! This means there is no splitting of the current at the junction between $R_2$ and $R_3$, therefore the correct answer must be 'E'. The reason is that there must be an open circuit, and seemingly only option 'B' is an open circuit. However, the current that was measured, was measured immediately after the connection, and if there is a capacitor there, then there would still be current through the capacitor before it became an open circuit. Therefore, answer 'E' is correct.

---
# 5.
![[Pasted image 20260614163649.png]]

Because all the components in the circuit are connected in a single loop, this is a series circuit. We can combine the resistors and the capacitors into equivalent components to make the math easier:

- **Equivalent Resistance ($R_{eq}$):** For resistors in series, you just add them together.
    
    $$R_{eq} = R_1 + R_2$$
    
- **Equivalent Capacitance ($C_{eq}$):** For capacitors in series, the reciprocal of the equivalent capacitance is the sum of their reciprocals.
    
    $$\frac{1}{C_{eq}} = \frac{1}{C_1} + \frac{1}{C_2} \implies C_{eq} = \frac{C_1 C_2}{C_1 + C_2}$$
    

In a series circuit, the current $I(t)$ is the same everywhere at any given moment. Because both capacitors are in series and start with zero initial charge ($Q_1(0) = 0$ and $Q_2(0) = 0$), the exact same amount of charge $Q(t)$ will be deposited on both of them by the current.

- Therefore, $Q_1(t) = Q_2(t) = Q(t)$
    
- The relationship between current and charge is: $I(t) = \frac{dQ}{dt}$
    

### **3. Apply Kirchhoff's Voltage Law (KVL)**

According to KVL, the sum of all voltage drops around a closed loop must equal the voltage supplied by the source. Let's write the equation for the loop:

$$V - V_{R1} - V_{C1} - V_{R2} - V_{C2} = 0$$

Substitute the formulas for voltage across a resistor ($V_R = I \cdot R$) and a capacitor ($V_C = \frac{Q}{C}$):

$$V - I \cdot R_1 - \frac{Q}{C_1} - I \cdot R_2 - \frac{Q}{C_2} = 0$$

Now, factor out the current $I$ and charge $Q$:

$$V - I(R_1 + R_2) - Q\left(\frac{1}{C_1} + \frac{1}{C_2}\right) = 0$$

Substitute our equivalent terms and $I = \frac{dQ}{dt}$:

$$V - \frac{dQ}{dt} R_{eq} - \frac{Q}{C_{eq}} = 0$$

### **4. Solve for the Charge ($Q(t)$)**

Rearranging the KVL equation gives us a first-order linear differential equation:

$$R_{eq} \frac{dQ}{dt} + \frac{Q}{C_{eq}} = V$$

This is the standard differential equation for a charging RC circuit. Solving this with the initial condition $Q(0) = 0$ yields the standard charging formula:

$$Q(t) = V C_{eq} \left(1 - e^{-\frac{t}{R_{eq}C_{eq}}}\right)$$

Since $Q(t)$ is the charge on both capacitors, we have our first answer.

### **5. Solve for the Current ($I(t)$)**

To find the current, we simply take the derivative of the charge $Q(t)$ with respect to time $t$:

$$I(t) = \frac{d}{dt} \left[ V C_{eq} \left(1 - e^{-\frac{t}{R_{eq}C_{eq}}}\right) \right]$$

$$I(t) = V C_{eq} \cdot \left( -e^{-\frac{t}{R_{eq}C_{eq}}} \right) \cdot \left( -\frac{1}{R_{eq}C_{eq}} \right)$$

The $C_{eq}$ terms cancel out, leaving:

$$I(t) = \frac{V}{R_{eq}} e^{-\frac{t}{R_{eq}C_{eq}}}$$

### **Final Answer**

Here are the final expressions for the charge and current for $t > 0$, expressed in terms of the original circuit variables:

**Charge on the capacitors:**

$$Q_1(t) = Q_2(t) = V \left( \frac{C_1 C_2}{C_1 + C_2} \right) \left[ 1 - \exp\left(-\frac{t}{(R_1 + R_2) \left(\frac{C_1 C_2}{C_1 + C_2}\right)}\right) \right]$$

**Current in the circuit:**

$$I(t) = \frac{V}{R_1 + R_2} \exp\left(-\frac{t}{(R_1 + R_2) \left(\frac{C_1 C_2}{C_1 + C_2}\right)}\right)$$

---
# 6.
![[Pasted image 20260614164905.png]]
![[Pasted image 20260614164942.png]]
![[Pasted image 20260614164955.png]]
![[Pasted image 20260614165005.png]]
![[Pasted image 20260614165014.png]]
