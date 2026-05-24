### Question 1

**Solve the following exact ODEs:**

**1.1** $2r\sin(2\theta)dr + 2r^2\cos(2\theta)d\theta = 0$

**Solution:**

Check if $P_\theta = Q_r$ (Note: the original text uses $P_y = Q_x$, but the variables here are $r$ and $\theta$):

$P_\theta = 4r\cos(2\theta)$

$Q_r = 4r\cos(2\theta)$

$P_\theta = Q_r$, and indeed the ODE is exact!

Choose which integral to do:

$$F(r, \theta) = \int Q(r, \theta) d\theta + c(r) = \int 2r^2\cos(2\theta) d\theta + c(r) = r^2\sin(2\theta) + c(r)$$

To find $c(r)$, we differentiate the obtained expression with respect to $r$ and compare it to $P$:

$$2r\sin(2\theta) + c'(r) = 2r\sin(2\theta) \implies c'(r) = 0 \implies c(r) = \text{const}$$

$$F(r, \theta) = r^2\sin(2\theta) + c$$

$$r^2\sin(2\theta) = c \implies 2\theta = \arcsin\left(\frac{c}{r^2}\right) \implies \theta = \frac{1}{2}\arcsin\left(\frac{c}{r^2}\right)$$

**1.2** $3x^2y^2dx + 2x^3ydy = 0$

**Solution:**

$P = 3x^2y^2$, $Q = 2x^3y$

Check if $P_y = Q_x$:

$P_y = 6x^2y$

$Q_x = 6x^2y$

$P_y = Q_x$, and indeed the ODE is exact!

Choose which integral to do:

$$F(x, y) = \int P(x, y) dx + c(y) = \int 3x^2y^2 dx + c(y) = x^3y^2 + c(y)$$

To find $c(y)$, we differentiate the obtained expression with respect to $y$ and compare it to $Q$:

$$2x^3y + c'(y) = 2x^3y \implies c'(y) = 0 \implies c(y) = \text{const}$$

In total, the solution is:

$$F(x, y) = x^3y^2 + k = c$$

$$x^3y^2 = c \implies y^2 = \frac{c}{x^3} \implies y_{1,2} = \pm\sqrt{\frac{c}{x^3}}$$

**1.3** $2xe^{x^2-y^2}dx - 2ye^{x^2-y^2}dy = 0$

**Solution:**

Check if $P_y = Q_x$:

$P_y = 2x \cdot (-2y)e^{x^2-y^2} = -4xye^{x^2-y^2}$

$Q_x = -2y \cdot 2xe^{x^2-y^2} = -4xye^{x^2-y^2}$

$P_y = Q_x$, yes, the equation is exact!

Choose which equation to fulfill:

$$F(x, y) = \int P(x, y) dx + c(y) = \int 2xe^{x^2-y^2} dx = e^{x^2-y^2} + c(y)$$

To find $c(y)$, we differentiate with respect to $y$:

$$-2ye^{x^2-y^2} + c'(y) = -2ye^{x^2-y^2} \implies c'(y) = 0$$

$$\int c'(y) dy = 0 \implies c(y) = \text{const}$$

$$F(x, y) = e^{x^2-y^2} + c = 0$$

$$x^2 - y^2 = c \implies y^2 = x^2 + c \implies y_{1,2} = \pm\sqrt{x^2 + c}$$

### Question 2

**Convert the following expressions to the form of an exact ODE and solve them:**

**2.1** $y' = \frac{-y\sin(x) + x^2}{y - \cos(x)}$

**Solution:**

$$y' = \frac{dy}{dx} = \frac{-y\sin(x) + x^2}{y - \cos(x)}$$

$$(y - \cos(x))dy = (-y\sin(x) + x^2)dx$$

$$(y\sin(x) - x^2)dx + (y - \cos(x))dy = 0$$

Check if $P_y = Q_x$:

$P = y\sin(x) - x^2 \implies P_y = \sin(x)$

$Q = y - \cos(x) \implies Q_x = \sin(x)$

$P_y = Q_x$, yes, the equation is exact!

Choose which equation to fulfill:

$$F(x, y) = \int Q(x, y) dy + c(x) = \int (y - \cos(x)) dy = \frac{y^2}{2} - y\cos(x) + c(x)$$

To find $c(x)$, we differentiate with respect to $x$:

$$y\sin(x) + c'(x) = y\sin(x) - x^2$$

$$c'(x) = -x^2 \implies \int c'(x) dx = \int -x^2 dx \implies c(x) = -\frac{x^3}{3}$$

$$F(x, y) = \frac{y^2}{2} - y\cos(x) - \frac{x^3}{3} = c$$

Now we find $y$ (using the quadratic formula):

$$y^2 - 2y\cos(x) - \frac{2x^3}{3} - 2c = 0$$

$$y_{1,2} = \cos(x) \pm \sqrt{\cos^2(x) - \left(-\frac{2x^3}{3} - 2c\right)} = \cos(x) \pm \sqrt{\cos^2(x) + \frac{2x^3}{3} + c}$$

**2.2** $y' = \frac{y\cos(x) - x}{y - \sin(x)}$

**Solution:**

$$y' = \frac{dy}{dx} = \frac{y\cos(x) - x}{y - \sin(x)}$$

$$(y - \sin(x))dy = (y\cos(x) - x)dx$$

$$(y\cos(x) - x)dx + (\sin(x) - y)dy = 0$$



Check if $P_y = Q_x$:

$P_y = \cos(x)$

$Q_x = \cos(x)$

$P_y = Q_x$, yes, the ODE is exact!

Choose which integral to do:

$$F(x, y) = \int Q(x, y) dy + c(x) = \int (\sin(x) - y) dy = y\sin(x) - \frac{y^2}{2} + c(x)$$

To find $c(x)$, we differentiate the obtained expression with respect to $x$ and compare it to $P$:

$$y\cos(x) + c'(x) = y\cos(x) - x \implies c'(x) = -x$$

$$\int c'(x) dx = \int -x dx \implies c(x) = -\frac{x^2}{2}$$

In total we get:

$$F(x, y) = y\sin(x) - \frac{x^2}{2} - \frac{y^2}{2} = c$$

$$y^2 - 2y\sin(x) + x^2 + 2c = 0$$

$$y_{1,2} = \frac{2\sin(x) \pm \sqrt{4\sin^2(x) - 4(x^2 + 2c)}}{2} = \sin(x) \pm \sqrt{\sin^2(x) - x^2 - c}$$