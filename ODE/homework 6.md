### Question 1

Find a solution to the ODE $y'' = y'y$ that satisfies $y(0) = 1$. _(Note: Based on the provided solution, it appears there is an implicitly given additional initial condition of $y'(0) = 1$)._

**Solution:** Since the variable $x$ does not appear, we will reduce the order of the equation. We are looking for a function $p(y)$ such that for the solution it holds:

$$y' = p(y) \implies y'' = p'(y) \cdot y'$$

We will substitute this into the ODE and get:

$$p'(y) \cdot p(y) = p(y) \cdot y$$

And therefore:

$$p'(y) = y$$

From this we get:

$$p(y) = \frac{1}{2}y^2 + C$$

Therefore the solution satisfies the equation:

$$y' = p(y) = \frac{1}{2}y^2 + C$$

Now we will use the given data; substitute $x = 0$:

$$1 = \frac{1}{2} + C \implies C = \frac{1}{2}$$

Therefore we are looking for the solution of the equation:

$$y' = \frac{1}{2}(y^2 + 1)$$

This is a separable equation. We will perform separation of variables and get:

$$\frac{1}{y^2+1} dy = \frac{1}{2} dx$$

We will integrate:

$$\arctan(y) = \frac{1}{2}x + C$$

Again we will use the given data, substitute $x = 0$:

$$\arctan(1) = C \implies C = \frac{\pi}{4}$$

In total, the final solution is:

$$y = \tan\left(\frac{1}{2}x + \frac{\pi}{4}\right)$$

### Question 2

Let $P(t)$ denote the size of the bacteria population at time $t$. "The rate of change of the growth rate" is the second derivative: $P''(t)$. "The growth rate" is: $P'(t)$. Therefore according to the given data _(implicit in the original problem statement)_:

$$P'' = 4P' - 3P$$

We will move sides:

$$P'' - 4P' + 3P = 0$$

This is a 2nd order homogeneous linear ODE with constant coefficients. We will build a characteristic polynomial:

$$r^2 - 4r + 3 = 0$$

We factor:

$$(r - 1)(r - 3) = 0$$

And therefore:

$$r = 1, 3$$

From here the general solution is:

$$P(t) = C_1e^t + C_2e^{3t}$$

We will differentiate:

$$P'(t) = C_1e^t + 3C_2e^{3t}$$

Substitute the initial condition $P(0) = 100$:

$$C_1 + C_2 = 100$$

And also $P'(0) = 200$:

$$C_1 + 3C_2 = 200$$

Subtract the equations:

$$2C_2 = 100 \implies C_2 = 50$$

And from this:

$$C_1 = 50$$

Therefore the solution is:

$$P(t) = 50e^t + 50e^{3t}$$

### Question 3

Given the ODE: $y'' - 4y' + 4y = 0$.

**Solution:**

Write the characteristic polynomial:

$$r^2 - 4r + 4 = 0$$

Factor:

$$(r - 2)^2 = 0$$

Therefore there is a double root: $r = 2$. When there is a double root, the general solution is:

$$y = C_1e^{2x} + C_2xe^{2x}$$

Meaning:

$$y = (C_1 + C_2x)e^{2x}$$

### Question 4

Given the ODE: $y'' + 2y' + 5y = 0$.

**Solution:**

Write the characteristic polynomial:

$$r^2 + 2r + 5 = 0$$

According to the quadratic formula:

$$r = \frac{-2 \pm \sqrt{4 - 20}}{2} = \frac{-2 \pm \sqrt{-16}}{2} = \frac{-2 \pm 4i}{2}$$

And therefore:

$$r = -1 \pm 2i$$

When the roots are $r = \alpha \pm \beta i$, the general solution is:

$$y = e^{\alpha x}(C_1\cos(\beta x) + C_2\sin(\beta x))$$

Here: $\alpha = -1, \beta = 2$.

And therefore:

$$y = e^{-x}(C_1\cos(2x) + C_2\sin(2x))$$