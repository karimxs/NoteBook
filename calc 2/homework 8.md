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