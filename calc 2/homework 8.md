# A.
## 1.
![[Pasted image 20260621122941.png]]
It's true
$$u = xy$$

Now, substitute this into the original function to create a single-variable function:

$$g(u) = u + e^u$$

We need to find the maximum and minimum possible values of $u$ (which is $xy$) given our domain constraint $9x^2 + 4y^2 \leq 16$. We can use the **AM-GM Inequality** (Arithmetic Mean-Geometric Mean), which states that $a^2 + b^2 \geq 2|ab|$ for any real numbers $a$ and $b$.

Let $a = 3x$ and $b = 2y$:

$$(3x)^2 + (2y)^2 \geq 2|(3x)(2y)|$$

$$9x^2 + 4y^2 \geq 12|xy|$$

We know from the domain definition that $9x^2 + 4y^2 \leq 16$. Combining these gives:

$$12|xy| \leq 16$$

$$|xy| \leq \frac{16}{12}$$

$$|xy| \leq \frac{4}{3}$$

$$-\frac{4}{3} \leq u \leq \frac{4}{3}$$


Now we examine $g(u) = u + e^u$ on the interval $[-\frac{4}{3}, \frac{4}{3}]$. To find critical points, we take the derivative with respect to $u$:

$$g'(u) = 1 + e^u$$

Since $e^u > 0$ for all real numbers $u$, it must be true that:

$$g'(u) > 0$$

Because the derivative is always strictly positive, $g(u)$ is a **strictly increasing function** and has no critical points inside the interval. Therefore, its absolute maximum and minimum must occur at the endpoints of the interval.


- **Absolute Minimum:** Occurs at the lowest bound, $u = -\frac{4}{3}$.

$$f_{\text{min}} = -\frac{4}{3} + e^{-4/3}$$

- **Absolute Maximum:** Occurs at the highest bound, $u = \frac{4}{3}$.

$$f_{\text{max}} = \frac{4}{3} + e^{4/3}$$

---
## 2.
![[Pasted image 20260622103717.png]]
It's true.

$$f(x,y) = \frac{x}{y^2 - 9}$$

This is a rational function. It is continuous everywhere except where its denominator is equal to zero. Let's find those points of discontinuity:

$$y^2 - 9 = 0$$

$$y^2 = 9$$

$$y = 3 \text{ or } y = -3$$

Now, let's examine the given domain $D$:

$$9x^2 + 4y^2 = 16$$

This equation represents an ellipse. To see if the discontinuity points ($y = \pm 3$) fall within or on this domain, let's find the maximum and minimum possible values for $y$ on this ellipse. Since $9x^2 \geq 0$ for any real number $x$, we can write:

$$4y^2 = 16 - 9x^2$$

$$4y^2 \leq 16$$

$$y^2 \leq 4$$

$$-2 \leq y \leq 2$$

Because the maximum value for $y$ anywhere in our domain is $2$ and the minimum is $-2$, the domain never reaches the problematic lines $y = 3$ or $y = -3$.

Therefore, the denominator is never zero within the domain $D$, which means the function $f(x,y)$ is **continuous** on the entire domain $D$.

Finally, we apply our calculus theorems:

- The domain $D$ is an ellipse (specifically, its boundary due to the $=$ sign), which is a **closed and bounded** set (a compact set).

- The function $f(x,y)$ is **continuous** on this closed and bounded set.


According to the **Extreme Value Theorem** (Weierstrass Theorem), any continuous function defined on a closed and bounded set must attain both an absolute maximum and an absolute minimum.

---
# B.
![[Pasted image 20260622103912.png]]
$$f_x = \frac{\partial}{\partial x}(x^3 - 12xy + 8y^3) = 3x^2 - 12y$$

$$f_y = \frac{\partial}{\partial y}(x^3 - 12xy + 8y^3) = -12x + 24y^2$$


Set both partial derivatives to zero and solve the system of equations:

1. $3x^2 - 12y = 0$

2. $-12x + 24y^2 = 0$


From equation (1), solve for $y$:

$$3x^2 = 12y$$

$$y = \frac{x^2}{4}$$

Substitute this $y$ into equation (2):

$$-12x + 24\left(\frac{x^2}{4}\right)^2 = 0$$

$$-12x + 24\left(\frac{x^4}{16}\right) = 0$$

$$-12x + \frac{3}{2}x^4 = 0$$

Multiply by $\frac{2}{3}$ to simplify:

$$-8x + x^4 = 0$$

$$x(x^3 - 8) = 0$$

This gives two possible values for $x$:

- $x = 0$

- $x^3 = 8 \Rightarrow x = 2$


Now, find the corresponding $y$ values using $y = \frac{x^2}{4}$:

- If $x = 0$, then $y = \frac{0^2}{4} = 0$. This gives the point **$(0, 0)$**.

- If $x = 2$, then $y = \frac{2^2}{4} = 1$. This gives the point **$(2, 1)$**.


We have two critical points: **$(0, 0)$** and **$(2, 1)$**.


To classify these points, we use the Second Derivative Test, which requires the second-order partial derivatives:

- $$f_{xx} = \frac{\partial}{\partial x}(3x^2 - 12y) = 6x$$

- $$f_{yy} = \frac{\partial}{\partial y}(-12x + 24y^2) = 48y$$

- $$f_{xy} = \frac{\partial}{\partial y}(3x^2 - 12y) = -12$$



The formula for the discriminant is $D(x,y) = f_{xx}f_{yy} - (f_{xy})^2$.

$$D(x,y) = (6x)(48y) - (-12)^2$$

$$D(x,y) = 288xy - 144$$


Now we evaluate $D$ and $f_{xx}$ at each critical point.

**For the point $(0, 0)$:**

- $D(0,0) = 288(0)(0) - 144 = -144$

- Since $D < 0$, the Second Derivative Test tells us that **$(0, 0)$ is a saddle point**.


**For the point $(2, 1)$:**

- $D(2,1) = 288(2)(1) - 144 = 576 - 144 = 432$

- Since $D > 0$, we must look at the concavity given by $f_{xx}$ to determine if it's a minimum or maximum.

- $f_{xx}(2,1) = 6(2) = 12$

- Since $D > 0$ and $f_{xx} > 0$, the function is concave up at this point. Therefore, **$(2, 1)$ is a local minimum**.


### **Final Answer:**

- **Saddle Point:** $(0, 0)$

- **Local Minimum:** $(2, 1)$

- **Local Maximum:** None

---
# C.
![[Pasted image 20260622104255.png]]

$$f(x,y) = \frac{1}{2}x^2 + \frac{1}{2}y^2$$

Domain: $\frac{1}{2}x^2 + y^2 \leq 1$

Set the first partial derivatives to zero:

$$f_x = x = 0$$

$$f_y = y = 0$$

The only critical point is $(0,0)$.

Check if it is inside the domain: $\frac{1}{2}(0)^2 + (0)^2 = 0 \leq 1$. It is inside.

Evaluate the function at this point:

$$f(0,0) = 0$$


The boundary is the ellipse:

$$\frac{1}{2}x^2 + y^2 = 1$$

From this equation, we can isolate $\frac{1}{2}x^2$:

$$\frac{1}{2}x^2 = 1 - y^2$$

Substitute this into the original function to create a single-variable function $h(y)$:

$$h(y) = (1 - y^2) + \frac{1}{2}y^2$$

$$h(y) = 1 - \frac{1}{2}y^2$$

Since $\frac{1}{2}x^2 \geq 0$ for all real $x$, we must have $1 - y^2 \geq 0$. This gives the strict interval for $y$:

$$-1 \leq y \leq 1$$

Now, find the critical points of $h(y)$ on this interval:

$$h'(y) = -y = 0 \Rightarrow y = 0$$

Evaluate $h(y)$ at the critical point $y=0$ and the endpoints $y=1, y=-1$:

- If $y = 0$, then $h(0) = 1 - 0 = 1$.
    
    Find the corresponding $x$ values: $\frac{1}{2}x^2 = 1 \Rightarrow x^2 = 2 \Rightarrow x = \pm\sqrt{2}$.
    
    This gives the points $(\sqrt{2}, 0)$ and $(-\sqrt{2}, 0)$ with a function value of $1$.
    
- If $y = 1$, then $h(1) = 1 - \frac{1}{2}(1)^2 = \frac{1}{2}$.
    
    Find the corresponding $x$ value: $\frac{1}{2}x^2 = 1 - 1^2 = 0 \Rightarrow x = 0$.
    
    This gives the point $(0, 1)$ with a function value of $\frac{1}{2}$.
    
- If $y = -1$, then $h(-1) = 1 - \frac{1}{2}(-1)^2 = \frac{1}{2}$.
    
    Find the corresponding $x$ value: $\frac{1}{2}x^2 = 1 - (-1)^2 = 0 \Rightarrow x = 0$.
    
    This gives the point $(0, -1)$ with a function value of $\frac{1}{2}$.
    


- Interior point: $f(0,0) = 0$
    
- Boundary points at $y=0$: $f(\pm\sqrt{2}, 0) = 1$
    
- Boundary points at $y=\pm1$: $f(0, \pm 1) = \frac{1}{2}$
    

**Final Answer:**

Absolute Minimum: $0$ at $(0, 0)$

Absolute Maximum: $1$ at $(\sqrt{2}, 0)$ and $(-\sqrt{2}, 0)$

---
# D.
![[Pasted image 20260622104411.png]]

$$\frac{x}{2} + \frac{y}{3} = 1$$

$$\frac{x}{2} = 1 - \frac{y}{3}$$

$$x = 2 - \frac{2}{3}y$$

Replace $x$ in the original function to create a single-variable function $h(y)$:

$$h(y) = \left(2 - \frac{2}{3}y\right)^2 + y^2$$

$$h(y) = \left(4 - \frac{8}{3}y + \frac{4}{9}y^2\right) + y^2$$

$$h(y) = \frac{13}{9}y^2 - \frac{8}{3}y + 4$$

Take the derivative with respect to $y$ and set it to zero to find the minimum:

$$h'(y) = \frac{26}{9}y - \frac{8}{3} = 0$$

$$\frac{26}{9}y = \frac{8}{3}$$

$$y = \frac{8}{3} \cdot \frac{9}{26}$$

$$y = \frac{72}{78}$$

$$y = \frac{12}{13}$$

Plug $y$ back into our isolated equation for $x$:

$$x = 2 - \frac{2}{3}\left(\frac{12}{13}\right)$$

$$x = 2 - \frac{24}{39}$$

$$x = 2 - \frac{8}{13}$$

$$x = \frac{26}{13} - \frac{8}{13}$$

$$x = \frac{18}{13}$$

Because the constraint represents an infinite line, and $x^2 + y^2$ goes to infinity as $x$ and $y$ get larger, the single critical point we found must be the absolute minimum.

The minimum point is **$(\frac{18}{13}, \frac{12}{13})$**.

---
# E.
![[Pasted image 20260622104904.png]]
We are restricted to the line $x + y = 1$. To make this easier, we can solve for $y$:

$$y = 1 - x$$


Now we take our main function $z = x^2 + y^2$ and replace the $y$ with what we just found. This gives us a new function (let's call it $h(x)$) that only has one variable:

$$h(x) = x^2 + (1 - x)^2$$


$$h(x) = x^2 + (1 - 2x + x^2)$$

$$h(x) = 2x^2 - 2x + 1$$


To find where this function hits its minimum or maximum, we take the derivative with respect to $x$ and set it to zero:

$$h'(x) = 4x - 2 = 0$$

$$4x = 2$$

$$x = \frac{1}{2}$$


Now that we have $x$, we plug it back into our constraint equation ($y = 1 - x$) to find $y$:

$$y = 1 - \frac{1}{2}$$

$$y = \frac{1}{2}$$

Because the function $h(x)$ is an upward-facing parabola (its second derivative $h''(x) = 4$ is positive), this critical point is an absolute minimum.

Therefore, the minimum point is **$(\frac{1}{2}, \frac{1}{2})$**.