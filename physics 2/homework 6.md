# 1.

Given a square parallel-plate capacitor with area $A$ and a gap (between the plates) $d_0$. The capacitor was deformed such that a small angle was created between its plates, meaning one side of the top plate was raised by a distance $b$ where $b \ll d_0, \sqrt{A}$. Calculate the first-order correction to the capacitance of the capacitor as a result of the deformation. (Assume that the field lines are still perpendicular to both plates and neglect edge effects).


$$L = \sqrt{A}$$

$$dA = L dx$$

$$dC = \frac{\epsilon_0 dA}{d(x)} = \frac{\epsilon_0 L}{d_0 + \frac{b}{L}x} dx$$

$$C = \int_{0}^{L} \frac{\epsilon_0 L}{d_0 + \frac{b}{L}x} dx = \epsilon_0 L \int_{0}^{L} \frac{1}{d_0 + \frac{b}{L}x} dx$$

$$C = \frac{\epsilon_0 L^2}{b} \left[ \ln\left(d_0 + \frac{b}{L}x\right) \right]_{0}^{L} = \frac{\epsilon_0 L^2}{b} (\ln(d_0 + b) - \ln(d_0))$$

$$C = \frac{\epsilon_0 A}{b} \ln\left(1 - \frac{b}{d_0}\right)$$

Using the Taylor expansion:

$$\ln(1+u) \approx u - \frac{u^2}{2} + \dots$$

$$\ln\left(1+\frac{b}{d_0}\right) \approx \frac{b}{d_0} - \frac{1}{2}\left(\frac{b}{d_0}\right)^2$$

$$C \approx \frac{\epsilon_0 A}{b} \left( \frac{b}{d_0} - \frac{b^2}{2d_0^2} \right)$$

$$C \approx \frac{\epsilon_0 A}{d_0} - \frac{\epsilon_0 A b}{2d_0^2}$$

---
# 2.

A network of identical capacitors, each with capacitance $C$, are arranged in a "semi-infinite" network as described in the drawing. Find the equivalent capacitance between point A and point B. Hint: Use points D and E.

Because the network is infinite, the equivalent capacitance of the entire network ($C_{eq}$) is the same as the equivalent capacitance of the portion starting at points D and E. Therefore, we can model the circuit as a series connection of two capacitors $C$ (the top and bottom branches) with a parallel combination of $C$ and $C_{eq}$.

$$\frac{1}{C_{eq}} = \frac{1}{C} + \frac{1}{C} + \frac{1}{C + C_{eq}}$$

$$\frac{1}{C_{eq}} = \frac{2}{C} + \frac{1}{C + C_{eq}}$$

$$\frac{1}{C_{eq}} = \frac{2(C + C_{eq}) + C}{C(C + C_{eq})} = \frac{3C + 2C_{eq}}{C^2 + CC_{eq}}$$

Cross-multiplying and rearranging gives a quadratic equation:

$$2C_{eq}^2 + 2CC_{eq} - C^2 = 0$$

Solving for the positive root of $C_{eq}$:

$$C_{eq} = \frac{\sqrt{3}-1}{2}C$$

---
# 3.

$n$ conducting plates, each with an identical cross-sectional area $A$, are arranged at a distance $d$ from each other. The plates are connected into two groups as described in the diagram. What is the capacitance of the system?


Every pair of adjacent plates forms a basic parallel-plate capacitor with the standard capacitance:

$$C_0 = \frac{\epsilon_0 A}{d}$$

Because there are $n$ plates connected in an alternating pattern to the two terminals, they create $n-1$ identical capacitors that are all connected in parallel.

For capacitors in parallel, the total capacitance is simply the sum of the individual capacitances:

$$C_{total} = C_1 + C_2 + \dots + C_{n-1}$$

$$C_{total} = (n-1) \cdot C_0$$

$$C_{total} = (n-1) \frac{\epsilon_0 A}{d}$$

---
# 4.

The capacitance of a parallel-plate capacitor in a vacuum is $C_0$. Half of it is filled with a dielectric material $\epsilon_r$ in two different ways (see drawings). What is the new capacitance for each way?


For the initial vacuum capacitor:

$$C_0 = \frac{\epsilon_0 A}{d}$$

**Configuration 1: Dielectric fills half the distance ($d/2$)** This arrangement acts like two capacitors connected in series.

- $C_1$ (vacuum half): $C_1 = \frac{\epsilon_0 A}{d/2} = 2\frac{\epsilon_0 A}{d} = 2C_0$
    
- $C_2$ (dielectric half): $C_2 = \frac{\epsilon_r \epsilon_0 A}{d/2} = 2\epsilon_r\frac{\epsilon_0 A}{d} = 2\epsilon_r C_0$
    

For capacitors in series:

$$\frac{1}{C_{tot}} = \frac{1}{C_1} + \frac{1}{C_2}$$

$$\frac{1}{C_{tot}} = \frac{1}{2C_0} + \frac{1}{2\epsilon_r C_0} = \frac{\epsilon_r + 1}{2\epsilon_r C_0}$$

$$C_{tot} = \frac{2\epsilon_r C_0}{\epsilon_r + 1}$$

**Configuration 2: Dielectric fills half the area ($A/2$)** This arrangement acts like two capacitors connected in parallel.

- $C_1$ (vacuum half): $C_1 = \frac{\epsilon_0 (A/2)}{d} = \frac{1}{2} C_0$
    
- $C_2$ (dielectric half): $C_2 = \frac{\epsilon_r \epsilon_0 (A/2)}{d} = \frac{\epsilon_r}{2} C_0$
    

For capacitors in parallel:

$$C_{tot} = C_1 + C_2$$

$$C_{tot} = \frac{1}{2}C_0 + \frac{\epsilon_r}{2}C_0$$

$$C_{tot} = \frac{C_0}{2}(1 + \epsilon_r)$$

---
# 5.

Given two conducting shells. One shell is charged with a charge $Q$ and has an inner radius $a$, and the second shell is charged with a charge $-Q$ and has an outer radius $c$.

The space between the inner radius $a$ and radius $b$ (where $b < c$) is filled with a dielectric material having a constant $\kappa_1$, and the rest of the space between the shells is filled with a dielectric $\kappa_2$ as described in the drawing.

## a. Find the capacitance of the system.

First, the electric field in a dielectric is:

$$E = \frac{Q}{4\pi\epsilon_0\epsilon_r r^2}$$

Calculating the potential difference ($\Delta V$) between the inner and outer shells:

$$\Delta V = \frac{Q}{4\pi\epsilon_0\kappa_1}\left(\frac{1}{a} - \frac{1}{b}\right) + \frac{Q}{4\pi\epsilon_0\kappa_2}\left(\frac{1}{b} - \frac{1}{c}\right)$$

Since $C = \frac{Q}{\Delta V}$:

$$C = \frac{4\pi\epsilon_0}{\frac{1}{\kappa_1}\left(\frac{1}{a} - \frac{1}{b}\right) + \frac{1}{\kappa_2}\left(\frac{1}{b} - \frac{1}{c}\right)}$$

## b. Show that when taking $\kappa_1 \to 1$ and $\kappa_2 \to 1$ we get the capacitance of a standard spherical capacitor.

Substituting $\kappa_1 = 1$ and $\kappa_2 = 1$ into the capacitance formula we just found:

$$C = \frac{4\pi\epsilon_0}{1 \cdot \left(\frac{1}{a} - \frac{1}{b}\right) + 1 \cdot \left(\frac{1}{b} - \frac{1}{c}\right)}$$

$$C = \frac{4\pi\epsilon_0}{\frac{1}{a} - \frac{1}{b} + \frac{1}{b} - \frac{1}{c}}$$

The $\frac{1}{b}$ terms cancel out, leaving:

$$C = \frac{4\pi\epsilon_0}{\frac{1}{a} - \frac{1}{c}}$$

This perfectly matches the known formula for the capacitance of a standard spherical capacitor in a vacuum.