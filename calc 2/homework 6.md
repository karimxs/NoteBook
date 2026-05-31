
**1.**

$$\sum_{k=1}^{\infty}\frac{k^{2}}{3^{k}}x^{k}$$

To find the radius of convergence $R$, we use the Ratio Test on the coefficients $a_k = \frac{k^2}{3^k}$:

$$R = \lim_{k \to \infty} \left| \frac{a_k}{a_{k+1}} \right| = \lim_{k \to \infty} \frac{\frac{k^2}{3^k}}{\frac{(k+1)^2}{3^{k+1}}}$$

$$R = \lim_{k \to \infty} \frac{k^2 \cdot 3^{k+1}}{(k+1)^2 \cdot 3^k} = \lim_{k \to \infty} 3 \left( \frac{k}{k+1} \right)^2 = 3 \cdot 1 = 3$$

The radius of convergence is $R=3$. The open interval is $(-3, 3)$.

Testing endpoints:

For $x=3$: $\sum_{k=1}^{\infty} \frac{k^2}{3^k} 3^k = \sum_{k=1}^{\infty} k^2$. This diverges since $\lim_{k \to \infty} k^2 \neq 0$.

For $x=-3$: $\sum_{k=1}^{\infty} \frac{k^2}{3^k} (-3)^k = \sum_{k=1}^{\infty} (-1)^k k^2$. This also diverges.

Domain of convergence: $(-3, 3)$.

---
**2.**

$$\sum_{k=1}^{\infty}\frac{(x-1)^{k}}{k^{1/2}}$$

Using the Ratio Test on $a_k = \frac{1}{\sqrt{k}}$:

$$R = \lim_{k \to \infty} \left| \frac{a_k}{a_{k+1}} \right| = \lim_{k \to \infty} \frac{\sqrt{k+1}}{\sqrt{k}} = \lim_{k \to \infty} \sqrt{1 + \frac{1}{k}} = 1$$

The center is $x_0 = 1$. The open interval is $(1-1, 1+1) = (0, 2)$.

Testing endpoints:

For $x=2$: $\sum_{k=1}^{\infty} \frac{1^k}{\sqrt{k}} = \sum_{k=1}^{\infty} \frac{1}{k^{1/2}}$. This diverges (p-series with $p = \frac{1}{2} \le 1$).

For $x=0$: $\sum_{k=1}^{\infty} \frac{(-1)^k}{\sqrt{k}}$. This converges by the Alternating Series Test ($\frac{1}{\sqrt{k}}$ is decreasing and limits to $0$).

Domain of convergence: $[0, 2)$.

---
**3.**

$$\sum_{k=1}^{\infty}\frac{k!}{k^{k}}(x+2)^{k}$$

Using the Ratio Test on $a_k = \frac{k!}{k^k}$:

$$R = \lim_{k \to \infty} \left| \frac{a_k}{a_{k+1}} \right| = \lim_{k \to \infty} \frac{k!}{k^k} \cdot \frac{(k+1)^{k+1}}{(k+1)!}$$

$$R = \lim_{k \to \infty} \frac{(k+1)^{k+1}}{k^k (k+1)} = \lim_{k \to \infty} \frac{(k+1)^k}{k^k} = \lim_{k \to \infty} \left(1 + \frac{1}{k}\right)^k = e$$

The center is $x_0 = -2$. The radius of convergence is $R=e$.

Interval of convergence: $(-2-e, -2+e)$.

---
**4.**

$$\sum_{k=1}^{\infty}(-1)^{k}\frac{(x-3)^{k}}{k}$$

Using the Ratio Test on $a_k = \frac{(-1)^k}{k}$:

$$R = \lim_{k \to \infty} \left| \frac{a_k}{a_{k+1}} \right| = \lim_{k \to \infty} \frac{\frac{1}{k}}{\frac{1}{k+1}} = \lim_{k \to \infty} \frac{k+1}{k} = 1$$

The center is $x_0 = 3$. The open interval is $(3-1, 3+1) = (2, 4)$.

Testing endpoints:

For $x=4$: $\sum_{k=1}^{\infty} \frac{(-1)^k 1^k}{k} = \sum_{k=1}^{\infty} \frac{(-1)^k}{k}$. This converges by the Alternating Series Test.

For $x=2$: $\sum_{k=1}^{\infty} \frac{(-1)^k (-1)^k}{k} = \sum_{k=1}^{\infty} \frac{1}{k}$. This diverges (Harmonic series).

Domain of convergence: $(2, 4]$.

---
**5.**

$$f(x,y)=\frac{x^{2}y}{x^{2}+y^{2}}$$

To find the first partial derivatives for $(x,y) \neq (0,0)$, use the quotient rule:

$$\frac{\partial f}{\partial x} = \frac{(2xy)(x^2+y^2) - (x^2y)(2x)}{(x^2+y^2)^2}$$

$$\frac{\partial f}{\partial x} = \frac{2x^3y + 2xy^3 - 2x^3y}{(x^2+y^2)^2} = \frac{2xy^3}{(x^2+y^2)^2}$$

$$\frac{\partial f}{\partial y} = \frac{(x^2)(x^2+y^2) - (x^2y)(2y)}{(x^2+y^2)^2}$$

$$\frac{\partial f}{\partial y} = \frac{x^4+x^2y^2-2x^2y^2}{(x^2+y^2)^2} = \frac{x^4-x^2y^2}{(x^2+y^2)^2}$$

---
**6.**

$$f(x,y)=\frac{x^{3}}{x^{2}+y^{2}}$$

Assuming $f(0,0)=0$, we check if partial derivatives exist at $(0,0)$ using the limit definition:

$$\frac{\partial f}{\partial x}(0,0) = \lim_{h \to 0} \frac{f(h,0) - f(0,0)}{h} = \lim_{h \to 0} \frac{\frac{h^3}{h^2+0} - 0}{h} = \lim_{h \to 0} \frac{h}{h} = 1$$

$$\frac{\partial f}{\partial y}(0,0) = \lim_{h \to 0} \frac{f(0,h) - f(0,0)}{h} = \lim_{h \to 0} \frac{\frac{0}{0+h^2} - 0}{h} = \lim_{h \to 0} \frac{0}{h} = 0$$

Yes, both partial derivatives exist at $(0,0)$.

---
**7.**

$$f(x,y)=\frac{xy^{2}}{x^{2}+y^{2}}, \quad f(0,0)=0$$

Calculating $\frac{\partial f}{\partial x}(0,0)$ by definition:

$$\frac{\partial f}{\partial x}(0,0) = \lim_{h \to 0} \frac{f(h,0) - f(0,0)}{h} = \lim_{h \to 0} \frac{\frac{h \cdot 0^2}{h^2+0^2} - 0}{h} = \lim_{h \to 0} \frac{0}{h} = 0$$


---
**8.**

$$f(x,y)=\frac{x^{2}y}{x^{2}+y^{2}}$$

Check continuity at $(0,0)$ using the squeeze theorem:

$$0 \le \left| \frac{x^2y}{x^2+y^2} \right| = |y| \left( \frac{x^2}{x^2+y^2} \right)$$

Since $\frac{x^2}{x^2+y^2} \le 1$:

$$|y| \left( \frac{x^2}{x^2+y^2} \right) \le |y| \cdot 1 = |y|$$

$$\lim_{(x,y) \to (0,0)} |y| = 0$$

By the squeeze theorem, the limit is $0$. Assuming $f(0,0)=0$, the function is continuous at $(0,0)$.

---
**9.**

$$f(x,y)=\frac{xy}{x^{2}+y^{2}}, \quad f(0,0)=0$$

Check differentiability at $(0,0)$. First, we check if it is continuous:

Path $y=x$: $\lim_{x \to 0} \frac{x \cdot x}{x^2+x^2} = \frac{x^2}{2x^2} = \frac{1}{2}$.

Path $y=0$: $\lim_{x \to 0} \frac{x \cdot 0}{x^2+0} = 0$.

The limit does not exist, so $f(x,y)$ is not continuous at $(0,0)$. Since it is not continuous, it is **not differentiable** at $(0,0)$.

---
**10.**

**Is the existence of partial derivatives at a point sufficient for differentiability?**

No. A classic counterexample is the function from Question 9: $f(x,y) = \frac{xy}{x^2+y^2}$ (with $f(0,0)=0$).

Its partial derivatives at $(0,0)$ exist and are both equal to $0$ (since $f(x,0)=0$ and $f(0,y)=0$ for all $x,y$). However, the function is not even continuous at $(0,0)$, meaning it cannot be differentiable.


---
**11.**

$$f(x,y)=x^{2}+y^{2}, \quad x=t^{2}, \quad y=\sin t$$

Find $\frac{df}{dt}$:

$$\frac{df}{dt} = \frac{\partial f}{\partial x}\frac{dx}{dt} + \frac{\partial f}{\partial y}\frac{dy}{dt}$$

$$\frac{\partial f}{\partial x} = 2x, \quad \frac{dx}{dt} = 2t$$

$$\frac{\partial f}{\partial y} = 2y, \quad \frac{dy}{dt} = \cos t$$

Substituting everything:

$$\frac{df}{dt} = (2x)(2t) + (2y)(\cos t) = 2(t^2)(2t) + 2(\sin t)(\cos t)$$

$$\frac{df}{dt} = 4t^3 + 2\sin t \cos t = 4t^3 + \sin(2t)$$


---
**12.**

$$f(x,y)=x^{2}y, \quad x=r\cos s, \quad y=r\sin s$$

Find $\frac{\partial f}{\partial r}$ and $\frac{\partial f}{\partial s}$:

$$\frac{\partial f}{\partial r} = \frac{\partial f}{\partial x}\frac{\partial x}{\partial r} + \frac{\partial f}{\partial y}\frac{\partial y}{\partial r} = (2xy)(\cos s) + (x^2)(\sin s)$$

Substitute $x$ and $y$:

$$\frac{\partial f}{\partial r} = 2(r\cos s)(r\sin s)\cos s + (r\cos s)^2\sin s = 2r^2\cos^2s\sin s + r^2\cos^2s\sin s = 3r^2\cos^2s\sin s$$

$$\frac{\partial f}{\partial s} = \frac{\partial f}{\partial x}\frac{\partial x}{\partial s} + \frac{\partial f}{\partial y}\frac{\partial y}{\partial s} = (2xy)(-r\sin s) + (x^2)(r\cos s)$$

Substitute $x$ and $y$:

$$\frac{\partial f}{\partial s} = 2(r\cos s)(r\sin s)(-r\sin s) + (r\cos s)^2(r\cos s) = -2r^3\cos s\sin^2s + r^3\cos^3s$$


---
**13.**

$$f(x,y)=x^{2}+xy$$

Find directional derivative at point $P(1,2)$ in the direction $\vec{v} = (1,1)$.

Gradient: $\nabla f = (2x+y, x)$.

At $P(1,2)$: $\nabla f(1,2) = (2(1)+2, 1) = (4,1)$.

Direction vector normalized: $\hat{u} = \frac{\vec{v}}{|\vec{v}|} = \left( \frac{1}{\sqrt{2}}, \frac{1}{\sqrt{2}} \right)$.

Directional derivative $D_{\hat{u}}f = \nabla f \cdot \hat{u}$:

$$D_{\hat{u}}f = (4,1) \cdot \left( \frac{1}{\sqrt{2}}, \frac{1}{\sqrt{2}} \right) = \frac{4}{\sqrt{2}} + \frac{1}{\sqrt{2}} = \frac{5}{\sqrt{2}}$$

---
**14.**

$$f(x,y,z)=xyz$$

Find directional derivative at $P(2,-1,2)$ in the direction $\vec{v} = (1,1,1)$.

Gradient: $\nabla f = (yz, xz, xy)$.

At $P(2,-1,2)$: $\nabla f(2,-1,2) = ((-1)(2), (2)(2), (2)(-1)) = (-2, 4, -2)$.

Direction vector normalized: $\hat{u} = \left( \frac{1}{\sqrt{3}}, \frac{1}{\sqrt{3}}, \frac{1}{\sqrt{3}} \right)$.

Directional derivative $D_{\hat{u}}f = \nabla f \cdot \hat{u}$:

$$D_{\hat{u}}f = -2\left(\frac{1}{\sqrt{3}}\right) + 4\left(\frac{1}{\sqrt{3}}\right) - 2\left(\frac{1}{\sqrt{3}}\right) = \frac{-2+4-2}{\sqrt{3}} = 0$$

---
**15.**

$$f(x,y)=x^{2}+y^{2}$$

Find the direction where the directional derivative is maximal at $P(1,1)$.

The maximum directional derivative always occurs in the direction of the gradient evaluated at that point.

Gradient: $\nabla f = (2x, 2y)$.

At $P(1,1)$: $\nabla f(1,1) = (2,2)$.

The direction of maximum rate of change is $(2,2)$, or represented as the unit vector $\left( \frac{1}{\sqrt{2}}, \frac{1}{\sqrt{2}} \right)$.