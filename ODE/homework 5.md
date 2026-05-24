### Question 1

Find a solution to the ODE $3xy^2y' + 2y^3 = \cos(x^2)$ that satisfies $y(\sqrt{\pi}) = 1$.

**Solution:**

First, we will move to the differential notation of the ODE and rearrange the sides:

$$(2y^3 - \cos(x^2))dx + 3xy^2dy = 0$$

Let's check if it is exact:

$$P_y = 6y^2 \neq Q_x = 3y^2$$

The ODE is not exact, we will want to check if it can be made exact. Let's first check if the expression $\frac{P_y - Q_x}{Q}$ does not depend on $y$:

$$\frac{P_y - Q_x}{Q} = \frac{6y^2 - 3y^2}{3xy^2} = \frac{1}{x}$$

The expression does not depend on $y$, meaning there is an integrating factor $\mu(x)$, yay!

The integrating factor in this case is:

$$\mu(x) = e^{\int \frac{P_y - Q_x}{Q} dx} = e^{\int \frac{1}{x} dx} = e^{\ln|x|} = |x| = x$$

Let's multiply by the integrating factor and verify that we indeed got an exact ODE:

$$x(2y^3 - \cos(x^2))dx + 3x^2y^2dy = 0$$

$$P_y = 6xy^2 = Q_x$$

The ODE is indeed exact!

Therefore it remains to solve it according to our standard method for solving exact ODEs (reminder - formula sheet).

We will find $F$ by calculating the integral $F = \int Qdy + c(x)$:

$$F = \int 3x^2y^2dy + c(x) = x^2y^3 + c(x)$$

We will differentiate and equate to the second coefficient:

$$F_x = 2xy^3 + c'(x) = P = x(2y^3 - \cos(x^2))$$

$$c'(x) = -x\cos(x^2)$$

$$c(x) = -\int x\cos(x^2) dx = -\frac{\sin(x^2)}{2}$$

And in total:

$$F = x^2y^3 - \frac{\sin(x^2)}{2}$$

Therefore the solution is given implicitly by:

$$x^2y^3 - \frac{\sin(x^2)}{2} = c$$

Let's substitute the initial condition $y=1, x=\sqrt{\pi}$:

$$\pi - \frac{\sin(\pi)}{2} = c$$

$$c = \pi$$

Therefore:

$$x^2y^3 - \frac{\sin(x^2)}{2} = \pi$$

Now it remains to isolate $y$:

$$y^3 = \frac{\pi + \frac{\sin(x^2)}{2}}{x^2}$$

$$y^3 = \frac{2\pi + \sin(x^2)}{2x^2}$$

$$y = \sqrt[3]{\frac{2\pi + \sin(x^2)}{2x^2}}$$

And this is the final solution.

### Question 2

A ball with mass $m = 1 \text{ kg}$ is thrown upwards by Yuli, with an initial velocity of magnitude 20 meters per second.

The forces acting on the ball are the force of gravity which is equal to $m \cdot 10$ in magnitude, and the force of air resistance which is equal in magnitude to the square of the velocity $v^2(t)$.

Within how much time will the ball reach its maximum height? What is the maximum height the ball will reach?

(You can give an approximate answer to three decimal places).

**Solution:**

Let's denote the position of the ball at time $t$ as $y(t)$.

Let's assume that the positive direction of the $y$ axis is upwards (like the initial direction of motion of the ball), and that the ball started moving from a height of 0.

Meaning, we have the initial condition $y(0) = 0$.

Air resistance acts opposite to the direction of motion of the ball, and therefore it has a negative sign.

Let's substitute everything into Newton's second law $F = ma$:

$$-mg - v^2 = ma$$

Substitute $a = v', m = 1 \text{ kg}, mg = m \cdot 10 = 10$, and we get:

$$-10 - v^2 = v'$$

Let's switch to differential notation $v' = \frac{dv}{dt}$:

$$-10 - v^2 = \frac{dv}{dt}$$

$$-(10 + v^2)dt = dv$$

Let's separate the variables:

$$-dt = \frac{1}{10 + v^2} dv$$

And now we will integrate both sides, as is customary in solving a separable ODE:

$$-\int dt = \int \frac{1}{10 + v^2} dv$$

$$\int \frac{1}{10 + v^2} dv = \int \frac{1}{(\sqrt{10})^2 + v^2} dv = \frac{1}{\sqrt{10}}\arctan\left(\frac{v}{\sqrt{10}}\right) + C$$

And in total:

$$-t = \frac{1}{\sqrt{10}}\arctan\left(\frac{v}{\sqrt{10}}\right) + C$$

Now we want to isolate $v$:

$$-t + C = \frac{1}{\sqrt{10}}\arctan\left(\frac{v}{\sqrt{10}}\right)$$

$$\sqrt{10}(-t + C) = \arctan\left(\frac{v}{\sqrt{10}}\right)$$

$$-\sqrt{10}t + C = \arctan\left(\frac{v}{\sqrt{10}}\right)$$

$$\tan(-\sqrt{10}t + C) = \frac{v}{\sqrt{10}}$$

$$v(t) = \sqrt{10}\tan(-\sqrt{10}t + C)$$

Let's substitute the initial condition $v(0) = 20$:

$$20 = \sqrt{10}\tan(C)$$

$$\frac{20}{\sqrt{10}} = \tan(C)$$

$$\arctan\left(\frac{20}{\sqrt{10}}\right) = C$$

From this, we get that the velocity function is:

$$v(t) = \sqrt{10}\tan\left(-\sqrt{10}t + \arctan\left(\frac{20}{\sqrt{10}}\right)\right)$$

The ball will reach its maximum height when the velocity function evaluates to zero, meaning:

$$0 = \sqrt{10}\tan\left(-\sqrt{10}t + \arctan\left(\frac{20}{\sqrt{10}}\right)\right)$$

$$\sqrt{10}t = \arctan\left(\frac{20}{\sqrt{10}}\right)$$

$$t = \frac{1}{\sqrt{10}}\arctan\left(\frac{20}{\sqrt{10}}\right) \approx 0.447 \text{ sec}$$

The ball will reach its maximum height within $0.447 \text{ sec}$.

Now it remains to calculate what the maximum height the ball will reach is. To do this, we want to find the function $y(t)$, and to discover what the maximum height is, we will substitute $t = \frac{1}{\sqrt{10}}\arctan\left(\frac{20}{\sqrt{10}}\right)$.

Recall that the velocity function is:

$$v(t) = \sqrt{10}\tan\left(-\sqrt{10}t + \arctan\left(\frac{20}{\sqrt{10}}\right)\right)$$

Because $v = y'$, we get:

$$y'(t) = \sqrt{10}\tan\left(-\sqrt{10}t + \arctan\left(\frac{20}{\sqrt{10}}\right)\right)$$

And to find $y(t)$ we will integrate both sides:

$$y(t) = \int \sqrt{10}\tan\left(-\sqrt{10}t + \arctan\left(\frac{20}{\sqrt{10}}\right)\right) dt$$

We will substitute:

$$u = -\sqrt{10}t + \arctan\left(\frac{20}{\sqrt{10}}\right)$$

$$du = -\sqrt{10}dt$$

Therefore:

$$y(t) = \int -\tan(u)du = \int -\frac{\sin(u)}{\cos(u)} du = \ln|\cos(u)| + c$$

Let's return to the variable $t$:

$$y(t) = \ln\left|\cos\left(-\sqrt{10}t + \arctan\left(\frac{20}{\sqrt{10}}\right)\right)\right| + c$$

Let's substitute the initial condition $y(0) = 0$:

$$0 = \ln\left|\cos\left(\arctan\left(\frac{20}{\sqrt{10}}\right)\right)\right| + c$$

$$c = -\ln\left|\cos\left(\arctan\left(\frac{20}{\sqrt{10}}\right)\right)\right|$$

And in total we get that the position function is:

$$y(t) = \ln\left|\cos\left(-\sqrt{10}t + \arctan\left(\frac{20}{\sqrt{10}}\right)\right)\right| - \ln\left|\cos\left(\arctan\left(\frac{20}{\sqrt{10}}\right)\right)\right|$$

To discover what the maximum height is, we will substitute $t = \frac{1}{\sqrt{10}}\arctan\left(\frac{20}{\sqrt{10}}\right)$:

$$y\left(\frac{1}{\sqrt{10}}\arctan\left(\frac{20}{\sqrt{10}}\right)\right) = \ln|\cos(0)| - \ln\left|\cos\left(\arctan\left(\frac{20}{\sqrt{10}}\right)\right)\right| \approx 1.857$$

### Question 3

Find a solution to the ODE $y' = y(\sin(x)y^2 - 1)$ that satisfies $y(0) = 1$.

**Solution:**

Let's start by rearranging the ODE:

$$y' = \sin(x)y^3 - y$$

Note that this is a Bernoulli ODE:

$$y' + y = \sin(x)y^3$$

$$a(x) = 1, \quad b(x) = \sin(x), \quad n = 3$$

We substitute $z = y^{1-n} = y^{-2}$ and get the ODE $z' - 2z = -2\sin(x)$

Which is of course a first-order linear ODE, where:

$$a(x) = -2, \quad A(x) = -2x, \quad b(x) = -2\sin(x)$$

Therefore the solution is given by the formula:

$$z = e^{-\int a(x)dx} \left(C + \int b(x)e^{\int a(x)dx}dx\right)$$

$$z = e^{2x} \left(C + \int -2\sin(x)e^{-2x}dx\right)$$

Let's calculate the integral on the side using integration by parts:

$$\int -2\sin(x)e^{-2x}dx = \sin(x)e^{-2x} - \int \cos(x)e^{-2x}dx$$

$$\int \cos(x)e^{-2x}dx = -\frac{1}{2}\cos(x)e^{-2x} - \frac{1}{2}\int \sin(x)e^{-2x}dx$$

$$2\int \sin(x)e^{-2x}dx = -\sin(x)e^{-2x} - \frac{1}{2}\cos(x)e^{-2x} - \frac{1}{2}\int \sin(x)e^{-2x}dx$$

$$\frac{5}{2}\int \sin(x)e^{-2x}dx = -\sin(x)e^{-2x} - \frac{1}{2}\cos(x)e^{-2x}$$

$$\int \sin(x)e^{-2x}dx = -e^{-2x}\left(\frac{2}{5}\sin(x) + \frac{1}{5}\cos(x)\right)$$

From here:

$$z = e^{2x}\left(C - 2\int \sin(x)e^{-2x}dx\right)$$

$$z = e^{2x}\left(C + 2e^{-2x}\left(\frac{2}{5}\sin(x) + \frac{1}{5}\cos(x)\right)\right)$$

$$z = C e^{2x} + \frac{4}{5}\sin(x) + \frac{2}{5}\cos(x)$$

Now we want to return to the variable $y$:

$z = y^{-2}$ therefore $y = \frac{1}{\sqrt{z}}$

$$y = \frac{1}{\sqrt{C e^{2x} + \frac{4}{5}\sin(x) + \frac{2}{5}\cos(x)}}$$

Let's substitute the initial condition $y(0) = 1$:

$$1 = \frac{1}{\sqrt{C + \frac{2}{5}}}$$

$$C = \frac{3}{5}$$

And the total solution to the ODE is:

$$y = \frac{1}{\sqrt{\frac{3}{5}e^{2x} + \frac{4}{5}\sin(x) + \frac{2}{5}\cos(x)}}$$

### Question 4

Find a solution to the ODE $xy' = x \cdot e^{\frac{y}{x}} + y$ that satisfies $y(1) = 3$.

**Solution:**

Note that this is a homogeneous ODE of the form $y' = g(\frac{y}{x})$.

We will expand (divide by $x$) until we reach the desired equation:

$$y' = e^{\frac{y}{x}} + \frac{y}{x}$$

Substitute $z = \frac{y}{x}$.

And we will use the formula sheet:

$$y' = e^z + z$$

$$g(z) = e^z + z$$

$$\int \frac{1}{g(z) - z} dz = \ln|x| + C$$

We substitute and get:

$$\int \frac{1}{e^z + z - z} dz = \int \frac{1}{e^z} dz = \int e^{-z} dz = -e^{-z}$$

Therefore in total:

$$-e^{-z} = \ln|x| + C$$

$$e^{-z} = -\ln|x| + C$$

$$-z = \ln(-\ln|x| + C)$$

$$z = -\ln(-\ln|x| + C)$$

We will return to the variable $y$ by substituting $y = xz$:

$$y = -x \cdot \ln(-\ln|x| + C)$$

Let's substitute the initial condition $y(1) = 3$:

$$-1 \cdot \ln(-\ln|1| + C) = 3$$

$$-\ln(C) = 3$$

$$\ln(C) = -3$$

$$C = e^{-3}$$

From here we get the final solution:

$$y = -x \cdot \ln(-\ln|x| + e^{-3})$$