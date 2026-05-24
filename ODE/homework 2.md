### Question 1

**a.** $y' + y^2(x^2 + 2) - 16(x^2 + 2) = 0$

**Solution:** We will rearrange the equation and take out common factors: $y' + (y^2 - 16)(x^2 + 2) = 0$ $y' = -(y^2 - 16)(x^2 + 2)$

We got an expression of the form $y' = f(x)g(y)$, and therefore the ODE is separable! We can switch to differential notation and get:

$$\frac{dy}{-(y^2 - 16)} = (x^2 + 2)dx$$

**b.** $y' = \frac{x^2+y^2}{x^2+xy}$

**Solution:** Let's check if the ODE is homogeneous. We will want to reach an ODE of the form $y' = g(\frac{y}{x})$. Let's rearrange a bit and get:

$$y' = \frac{1+(\frac{y}{x})^2}{1+\frac{y}{x}}$$

Meaning in this case we got $g(\frac{y}{x}) = \frac{1+(\frac{y}{x})^2}{1+\frac{y}{x}}$. Let's substitute $z = \frac{y}{x}$ and get: $g(z) = \frac{1+z^2}{1+z}$. Meaning this is indeed a homogeneous ODE. (To find a solution, it only remains to substitute into the formula sheet, and not to forget to find the solution to the original ODE, meaning to return to $y$).

**c.** $y' + y = x$

**Solution:** This is a first-order linear ODE, where $a(x) = 1, b(x) = x$. (Here too, to find a solution, it only remains to substitute into the formula sheet).

**d.** $2xyy' = y^2 - 1$

**Solution:** We will divide by $x(y^2-1)$ and get:

$$\frac{2yy'}{y^2 - 1} = \frac{1}{x}$$

Or in differential notation:

$$\frac{2y}{y^2 - 1} \frac{dy}{dx} = \frac{1}{x}$$

Meaning we got a separable ODE:

$$\frac{2y}{y^2 - 1} dy = \frac{1}{x} dx$$

**e.** $7y' = y$

**Solution:** We will switch to differential notation and get:

$$7 \frac{dy}{dx} = y$$

$$7dy = ydx$$

$$\frac{1}{y} dy = \frac{1}{7} dx$$

Meaning we got a separable ODE.

### Question 2

Find a solution to the ODE $y' = 2x + 2xy^2$ that satisfies the initial condition $y(0) = 0$.

**Solution:** First, we will rearrange the equation and take out common factors: $y' = 2x(1 + y^2)$

We got an expression of the form $y' = f(x)g(y)$ and therefore this is a separable ODE. We will switch to differential notation and get:

$$\frac{dy}{dx} = 2x(1 + y^2)$$

$$dy = 2x(1 + y^2)dx$$

Recall that the goal is to separate the variables, therefore we will divide by $(1 + y^2)$ and get:

$$\frac{1}{1 + y^2} dy = 2x dx$$

Now we will integrate both sides, each with respect to its variable:

$$\int \frac{1}{1 + y^2} dy = \int 2x dx$$

$$\arctan(y) = x^2 + c$$

We got the implicit equation. But let's not forget that the solution to an ODE is a function! Therefore we will want to isolate $y$:

$$y = \tan(x^2 + c)$$

Now we can substitute the initial condition:

$$y(0) = \tan(0 + c) = \tan(c) = 0$$

And therefore $c = 0$.

Hence, the solution to the ODE that satisfies the initial condition is:

$$y = \tan(x^2)$$

### Question 3

An apple with mass $m$, falls from a height of 10 meters. Assume that the only force acting on the apple is the force of gravity. How much time will it take for the apple to reach the ground? _Hint: Define a function $y(t)$ that measures the height of the apple at time $t$, calculate what the initial condition is, and into which ODE we must substitute the data._

**Solution:** An apple with mass $m$, falls from a height of 10 meters. The only force acting on the apple is the force of gravity, meaning the only force acting on the apple is $mg$. ($mg$ is relevant when time is measured in seconds, and distance is measured in meters). _Note: For convenience, it is recommended at this stage to refer to the mass of the apple as $m$._

Let's define: $y(t)$ is the function that measures the height of the apple at time $t$. Note that the apple falls from a height of 10 meters, meaning, at time $t = 0$ the height of the apple is 10 meters, we will substitute this into the function we defined and get: $y(0) = 10$ And this is our initial condition.

In addition, we are given that the apple _falls_, therefore we can deduce that its initial velocity is zero. Meaning we will get an additional initial condition: $y'(0) = 0$

Also, we will deduce that the height of the apple at the ground is 0 meters, and we will define the positive direction to be upwards. Let's substitute everything into the ODE: $F = ma$ Here $F = -mg$ because we defined the positive direction to be upwards! The force is trying to drag us downwards and therefore it receives the minus sign. Total: $-mg = ma$

Now we can cancel out $m$ and get: $-g = a$ (We see here that the mass does not affect it, since there is no air resistance). Recall that: $a = y''$, therefore: $y'' = -g$

Recall that we want to find how much time it will take for the apple to reach the ground, or in other words, we want to find the value of $t$ for which $y(t) = 0$. Therefore, we will want to integrate both sides twice, so that we can reach $y$ from $y''$. And let's not forget to add a constant after each integral: $y' = -gt + c$

Before we move to the next integral, let's check if we can substitute an initial condition. Indeed, the initial condition that can be substituted right now is: $y'(0) = 0$. We will substitute and get: $y'(0) = 0 + c = 0$ Meaning $c = 0$.

Now we will want to perform an additional integral, this time on the ODE: $y' = -gt$ And we will get:

$$y = -\frac{1}{2}gt^2 + c$$

Now we can substitute our second initial condition, meaning: $y(0) = 10$: $y(0) = c = 10$ Therefore:

$$y = -\frac{1}{2}gt^2 + 10$$

Recall that our goal is to find when the apple reaches the ground, meaning we want to find the value of $t$ for which $y(t) = 0$.

$$0 = -\frac{1}{2}gt^2 + 10$$

$$\frac{1}{2}gt^2 = 10$$

$$gt^2 = 20$$

$$t^2 = \frac{20}{g}$$

By taking the square root, we will only refer to the positive solution, since we are dealing with time.

$$t = \sqrt{\frac{20}{g}} \approx 1.42 \text{ sec}$$

### Question 4

Find a solution to the ODE $xy' = y + \frac{y}{\ln(\frac{y}{x})}$ that satisfies $y(1) = e^{-2}$.

**Solution:** First, we will want to rearrange the equation:

$$xy' = y + \frac{y}{\ln(\frac{y}{x})}$$

$$y' = \frac{y}{x} + \frac{\frac{y}{x}}{\ln(\frac{y}{x})}$$

Therefore, this is a homogeneous ODE, we reached an ODE of the form $y' = g(\frac{y}{x})$. Therefore, we will do as written in the formula sheet. Substitute $z = \frac{y}{x}$ And we get: $g(z) = z + \frac{z}{\ln(z)}$.

$$\int \frac{1}{g(z) - z} dz = \ln|x| + [cite_start]C$$

Let's substitute $g(z)$:

$$\int \frac{1}{z + \frac{z}{\ln(z)} - z} dz = \ln|x| + [cite_start]C$$

$$\int \frac{1}{\frac{z}{\ln(z)}} dz = \ln|x| + [cite_start]C$$

$$\int \frac{\ln(z)}{z} dz = \ln|x| + [cite_start]C$$

We want to find the integral for $z$, and for that we will use substitution: Let $t = \ln(z)$ $dt = \frac{1}{z} dz$

$$\int t dt = \frac{t^2}{2} + c = \frac{\ln^2(z)}{2} + c$$

In total we get:

$$\frac{\ln^2(z)}{2} = \ln|x| + [cite_start]C$$

To find the solution to the ODE, we will want to isolate $z$, and let's not forget to return to $y$ for the original ODE.

$$\ln^2(z) = 2\ln|x| + [cite_start]C$$

$$\ln(z) = \pm\sqrt{2\ln|x| + [cite_start]C}$$

$$z = e^{\pm\sqrt{2\ln|x| + [cite_start]C}}$$

Therefore $y = xz$ brings us to the solution for the original ODE:

$$y = x \cdot e^{\pm\sqrt{2\ln|x| + [cite_start]C}}$$

Now, we can substitute the initial condition and get:

$$y(1) = 1 \cdot e^{\pm\sqrt{2\ln|1| + [cite_start]C}} = e^{\pm\sqrt{C}}$$

Meaning we will get:

$$e^{-2} = e^{\pm\sqrt{C}}$$

$$-2 = \pm\sqrt{C}$$

Therefore, we will take the solution with the minus sign (because that is the one that will satisfy the initial condition!), together with $C = 4$. And the total solution is:

$$y = x \cdot e^{-\sqrt{2\ln|x| + [cite_start]4}}$$