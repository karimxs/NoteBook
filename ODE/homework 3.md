### Question 1

**a.** $y' - 2y = 2xe^{2x}$

**Variation of Parameters** We want to find $y = y_h + y_p$

$$y_h' - 2y_h = 0$$

$$\frac{y_h'}{y_h} = 2$$

$$\int \frac{dy_h}{y_h} = \int 2 dx$$

$$\ln|y_h| [cite_start]= 2x + c(x)$$

$$y_h = c(x)e^{2x}$$

After finding $y_h$, we will look for $y_p$

$$(c(x)e^{2x})' - 2y = 2xe^{2x}$$

$$c'(x)e^{2x} + c(x)2e^{2x} - 2c(x)e^{2x} = 2xe^{2x}$$

We will simplify the expression

$$c'(x)e^{2x} = 2xe^{2x}$$

$$c'(x) = 2x$$

$$\int c'(x) dx = \int 2x dx$$

$$c(x) = x^2$$

We substitute and get $y_p = x^2e^{2x}$

$$y = y_p + y_h = (c + x^2)e^{2x}$$


**b.** $y\cos(x) + y'\sin(x) = \sin(2x)$

We will start by simplifying the expression to reach the form $y' + a(x)y = b(x)$, we will divide it by $\sin(x)$

$$y' + y\cot(x) = \frac{\sin(2x)}{\sin(x)} = \frac{2\sin(x)\cos(x)}{\sin(x)} = 2\cos(x)$$

** Variation of Parameters**

$$y_h' + y_h\cot(x) = 0$$

$$y_h' = -y_h\cot(x)$$

$$\int \frac{dy_h}{y_h} = -\int \cot(x) dx$$

We know that $\int \cot(x)dx = \ln|\sin(x)| + [cite_start]c$ We substitute the solution and get

$$\ln|y_h| = -\ln|\sin(x)| + [cite_start]c$$

$$y_h = e^{\ln|\frac{1}{\sin(x)}| + [cite_start]c} = \frac{c}{\sin(x)}$$

We will look for $y_p$

$$\left(\frac{c(x)}{\sin(x)}\right)' + y\cot(x) = 2\cos(x)$$

$$\frac{c'(x)\sin(x) - c(x)\cos(x)}{\sin^2(x)} + \frac{c(x)\cos(x)}{\sin^2(x)} = 2\cos(x)$$

$$c'(x) = 2\cos(x)\sin(x) = \sin(2x)$$

$$\int c'(x) dx = \int \sin(2x) dx$$

$$c(x) = -\frac{\cos(2x)}{2}$$

$$y_p = -\frac{\cos(2x)}{2\sin(x)}$$

And finally we get

$$y = y_p + y_h = \frac{c}{\sin(x)} - \frac{\cos(2x)}{2\sin(x)}$$


### Question 2

**a.** $y' + xy = xy^3$

We identify that this is a Bernoulli equation where $n = 3$ We substitute $z = y^{1-n} = y^{1-3} = y^{-2} = \frac{1}{y^2}$ And we get from the formula $z' + (1-3)xz = (1-3)x$

$$z' - 2zx = -2x$$

We got a linear equation, we will solve it using the direct formula

$$z = e^{-\int -2x dx}\left(c + \int -2xe^{\int -2xdx} dx\right)$$

$$z = e^{x^2}\left(c + \int -2xe^{-x^2} dx\right)$$

Notice that $f'(x)e^{f(x)} = -2xe^{-x^2}$ Therefore it is easy to see that $(e^{-x^2})' = -2xe^{-x^2}$ and therefore $\int -2xe^{-x^2} dx = e^{-x^2}$

$$z = e^{x^2}(c + e^{-x^2})$$

$$z = ce^{x^2} + 1$$

Substitute back $z = \frac{1}{y^2}$

$$\frac{1}{y^2} = ce^{x^2} + 1$$

$$y^2 = \frac{1}{ce^{x^2} + 1}$$

$$y = \sqrt{\frac{1}{ce^{x^2} + 1}}$$

**b.** $3xy - x^2y' = y^2e^x$

We will start by simplifying the exercise to reach an equation of the form $y' + a(x)y = b(x)y^n$

$$y' - \frac{3y}{x} = -\frac{y^2e^x}{x^2}$$


$$z = y^{1-2} = \frac{1}{y}$$

Substitute into the formula and get

$$z' - \frac{(1-2)3z}{x} = -\frac{(1-2)e^x}{x^2}$$

$$z' + \frac{3z}{x} = \frac{e^x}{x^2}$$

Substitute into the formula

$$z = e^{-\int \frac{3}{x} dx}\left(c + \int \frac{e^x}{x^2}e^{\int \frac{3}{x}dx} dx\right)$$

$$z = e^{-\ln|x^3|}\left(c + \int \frac{e^x}{x^2}e^{\ln|x^3|}dx\right)$$

$$z = \frac{1}{x^3}\left(c + \int \frac{e^x}{x^2} x^3 dx\right)$$

$$z = \frac{1}{x^3}\left(c + \int xe^x dx\right)$$

$$z = \frac{1}{x^3}(c + xe^x - e^x)$$

Substitute back

$$y = \frac{1}{z}$$

$$y = \frac{x^3}{c + xe^x - e^x}$$

### Question 3

A boat weighing 1000 kg sails upstream at a speed of 30 meters per second. Suddenly the engine stops. The coefficient of friction of the boat with the water is $\mu = 100$. The drag of the boat is $F_{drag} = 300$. **a.** Build a model describing the motion of the boat according to $v(t)$. **b.** Solve the ODE and find a particular solution describing the boat's speed $v(t)$. **c.** After how much time will the boat's speed be 5 meters per second?

**Solution:**

**a.** We will look at the formula $\Sigma F = ma$

$$1000v' = -300(v-2) - 100(v-2)^2$$

Note, the boat is decelerating and therefore we get a negative derivative by necessity. Because the boat sails against the direction of the stream we substitute $v-2$ because the speed of the stream affects the speed of the boat in relation to friction and drag. Note that the initial speed of the boat will be $v(0) = 30$ and this will be our initial condition later.

**b.** Note that this is not a Bernoulli equation but we can easily convert it to Bernoulli. We will start by simplifying the expression

$$v' = -0.3(v-2) - 0.1(v-2)^2$$

We will perform a "shift" of the function on the coordinate system Substitute $w(t) = v(t) - 2$ We will differentiate with respect to $t$ and get

$$w' = v'$$

Substitute into the equation and get a Bernoulli equation

$$w' = -0.3w - 0.1w^2$$

And now we can solve the equation according to the Bernoulli equation.

Substitute $z = w^{1-2} = \frac{1}{w}$ And substitute into the equation

$$z' + (1-2)0.3w = -(1-2)0.1$$

$$z' - 0.3z = 0.1$$

$$z = e^{-\int -0.3 dt}\left(c + \int 0.1e^{\int -0.3dt} dt\right)$$

$$z = e^{0.3t}\left(c + \int 0.1e^{-0.3t} dt\right)$$

$$z = e^{0.3t}\left(c - \frac{1}{3}e^{-0.3t}\right)$$

$$z = ce^{0.3t} - \frac{1}{3}$$

Substitute back and get $w = \frac{1}{z}$

$$w = \frac{1}{ce^{0.3t} - \frac{1}{3}}$$

And finally substitute back $w = v - 2 \implies v = w + 2$ And we get the particular solution $v = \frac{1}{ce^{0.3t} - \frac{1}{3}} + 2$

We will look for a particular solution

$$w(0) = 30 = \frac{1}{ce^{0} - \frac{1}{3}} + 2$$

$$28 = \frac{1}{c - \frac{1}{3}}$$

$$c - \frac{1}{3} = \frac{1}{28}$$

$$c = \frac{31}{84}$$

Substitute back and we get a function describing the boat's deceleration

$$v(t) = \frac{1}{\frac{31}{84}e^{0.3t} - \frac{1}{3}} + 2$$

**c.** We will look for some time $\tau$ Substitute $v(\tau) = 5 = \frac{1}{\frac{31}{84}e^{0.3\tau} - \frac{1}{3}} + 2$

$$3 = \frac{1}{\frac{31}{84}e^{0.3\tau} - \frac{1}{3}}$$

$$\frac{1}{3} = \frac{31}{84}e^{0.3\tau} - \frac{1}{3}$$

$$\frac{10}{3} = \frac{31}{84}e^{0.3\tau}$$

$$e^{0.3\tau} = \frac{56}{31}$$

$$0.3\tau = 0.5913$$

$$\tau = 1.9712$$

The boat will be at a speed of 5 meters per second after about 1.98 seconds.