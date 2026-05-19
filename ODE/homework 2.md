# 1.
![[Pasted image 20260519161247.png]]
**A.**

$$y' + y^2(x^2 + 2) - 16(x^2 + 2) = 0$$

- **Analysis:** We can factor out the common term $(x^2 + 2)$ to get $y' + (y^2 - 16)(x^2 + 2) = 0$, which can be rearranged to $y' = -(x^2 + 2)(y^2 - 16)$. Because we can write the right side as a product of a function of $x$ and a function of $y$, it can be separated.

- **Type: Separable**


**B.**

$$y' = \frac{x^2 + y^2}{xy}$$

- **Analysis:** If we substitute $tx$ and $ty$ for $x$ and $y$, we get $\frac{(tx)^2 + (ty)^2}{(tx)(ty)} = \frac{t^2(x^2 + y^2)}{t^2xy} = \frac{x^2 + y^2}{xy}$. Since the $t$ terms cancel out entirely (it is a homogeneous function of degree 0), the equation fits the definition.

- **Type: Homogeneous**


**C.**

$$y' + y = x$$

- **Analysis:** This equation is already in the standard form of a first-order linear ODE: $y' + p(x)y = q(x)$, where $p(x) = 1$ and $q(x) = x$.

- **Type: Linear**


**D.**

$$2xyy' = y^2 - 1$$

- **Analysis:** We can rearrange this to isolate $y'$ and separate the variables: $y' = \frac{y^2 - 1}{2xy}$, which can be rewritten as a product of $x$ and $y$ terms: $y' = \left(\frac{1}{2x}\right)\left(\frac{y^2 - 1}{y}\right)$.

- **Type: Separable**


**E.**

$$7y' = y$$

- **Analysis:** This equation actually fits into two categories. It can be written as $y' - \frac{1}{7}y = 0$ (which fits the standard **Linear** form) and it can also be easily separated into $\frac{1}{y}dy = \frac{1}{7}dx$.

- **Type: Separable and Linear**

---
# 2.
![[Pasted image 20260519161608.png]]
First, factor out the common term $2x$ on the right side:

$$y' = 2x(1 + y^2)$$

Next, replace $y'$ with $\frac{dy}{dx}$ and separate the $x$ and $y$ variables to opposite sides of the equation:

$$\frac{dy}{dx} = 2x(1 + y^2)$$

$$\frac{1}{1 + y^2} dy = 2x \, dx$$

Now, take the integral of both sides:

$$\int \frac{1}{1 + y^2} dy = \int 2x \, dx$$

The integral on the left is a standard inverse trigonometric identity, and the right side is a basic power rule integral:

$$\arctan(y) = x^2 + C$$



We are given the initial condition $y(0) = 0$. This means when $x = 0$, $y = 0$. Plug these values into our general solution:

$$\arctan(0) = (0)^2 + C$$

Since $\arctan(0) = 0$, we get:

$$0 = 0 + C \implies C = 0$$

Substitute $C = 0$ back into the equation:

$$\arctan(y) = x^2$$


To isolate $y$, take the tangent of both sides:

$$y = \tan(x^2)$$

This is your final, specific solution to the ODE.