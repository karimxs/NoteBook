# 1.
![[Pasted image 20260519153217.png]]
A. $(y'')^4 + 5xy = e^{3x}$

- **Order: 2** (The highest derivative is the second derivative, $y''$)


**B.** $x^2y' - xy = 2x$

- **Order: 1** (The highest derivative is the first derivative, $y'$)


**C.** $xy' + y''' = (x-1)y'' + x$

- **Order: 3** (The highest derivative is the third derivative, $y'''$)
---
# 2.
![[Pasted image 20260519154233.png]]
**A.**

$$yy' = x$$

Replace $y'$ with $\frac{dy}{dx}$.

$$y \frac{dy}{dx} = x$$

Multiply both sides by $dx$.

$$y \, dy = x \, dx$$

Rearrange the terms to one side.

$$x \, dx - y \, dy = 0$$

---

**B.**

$$x^2e^{xy}y' = x\sin(2x) - xye^{xy}$$

Replace $y'$ with $\frac{dy}{dx}$.

$$x^2e^{xy}\frac{dy}{dx} = x\sin(2x) - xye^{xy}$$

Multiply both sides by $dx$.

$$x^2e^{xy} \, dy = (x\sin(2x) - xye^{xy}) \, dx$$

Rearrange the terms to one side (subtracting the left side from the right).

$$(x\sin(2x) - xye^{xy}) \, dx - x^2e^{xy} \, dy = 0$$
---
# 3.
![[Pasted image 20260519160237.png]]
**A.**

$$dy = ydx$$

 Divide both sides by $dx$ to group the differentials.

$$\frac{dy}{dx} = y$$

 Replace $\frac{dy}{dx}$ with $y'$.

$$y' = y$$

---

**B.**

$$\frac{1}{y^3}dy = \frac{x}{\sqrt{1+x^2}}dx$$

 Divide both sides by $dx$ to isolate $\frac{dy}{dx}$ on the left side.

$$\frac{1}{y^3} \frac{dy}{dx} = \frac{x}{\sqrt{1+x^2}}$$

 Replace $\frac{dy}{dx}$ with $y'$.

$$\frac{1}{y^3} y' = \frac{x}{\sqrt{1+x^2}}$$

---
# 4.
![[Pasted image 20260519160418.png]]
**A.**

$$y^2 = x^2 + c$$

 If we differentiate this implicitly, we get $2yy' = 2x$, which simplifies to the ODE $yy' = x$. Integrating that ODE yields exactly $y^2 = x^2 + c$. The constant $c$ is a simple, arbitrary real number with no algebraic restrictions placed upon it.

**B.**

$$\ln|y| = 2x + c$$

 Differentiating this gives $\frac{1}{y}y' = 2$, which is the ODE $y' = 2y$. The constant $c$ can be any real number, so this implicit equation successfully represents the family of solutions.


**C.**

$$y = \cos(x) + e^c$$

 If we differentiate this equation, the constant term $e^c$ disappears, leaving the ODE $y' = -\sin(x)$.

To find the true general solution of this ODE, we integrate: $\int -\sin(x) dx = \cos(x) + C$, where $C$ can be _any_ real number (positive, negative, or zero).

However, in the given expression, the term $e^c$ is strictly positive ($e^c > 0$). It is impossible for $e^c$ to represent a negative constant or zero. Because it restricts the family of curves, it is not a complete general solution.

 **Conclusion:** **No**, it is not a valid general solution in its current form.

 **Simplified Form:** We fix this by replacing the restricted term $e^c$ with a standard, unrestricted constant $C$. The simplified valid solution is:

$$y = \cos(x) + C$$