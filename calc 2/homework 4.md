### **Question 1**

**Explanation:** To prove uniform convergence, we can use the **Weierstrass M-test**. We need to find the maximum value of the function $f_k(x) = x^k(1-x)^k$ on the interval $[0,1]$ and show that the sum of these maximums converges.

$$f_k(x) = x^k(1-x)^k$$

We find the maximum by setting the derivative to zero:

$$f'_k(x) = kx^{k-1}(1-x)^{k-1}(1-2x) = 0 \implies x = \frac{1}{2}$$

Substituting $x = 1/2$ back into the function gives us the upper bound $M_k$:

$$\max_{x \in [0,1]} |f_k(x)| = f_k\left(\frac{1}{2}\right) = \frac{1}{4^k}$$

Because $\sum \frac{1}{4^k}$ is a convergent geometric series, the Weierstrass M-test guarantees uniform convergence:

$$\sum_{k=1}^{\infty} \frac{1}{4^k} < \infty \implies \sum_{k=1}^{\infty} x^k(1-x)^k \text{ converges uniformly on } [0,1]$$

### **Question 2**

**Explanation:** This is another direct application of the **Weierstrass M-test**. We bound the trigonometric function to find our $M_k$.

Since the cosine function is bounded by 1 for all real numbers:

$$\forall x \in \mathbb{R}, \quad |a_k \cos(kx)| \le |a_k| \cdot 1 = |a_k|$$

We are given that the series $\sum a_k$ converges absolutely, which means $\sum |a_k|$ converges. Therefore, the series converges uniformly:

$$\sum_{k=1}^{\infty} |a_k| < \infty \implies \sum_{k=1}^{\infty} a_k \cos(kx) \text{ converges uniformly on } \mathbb{R}$$

### **Question 3**

**Explanation:** Power series can be **integrated term-by-term** strictly within their interval of convergence. We start with the known geometric series expansion for $\frac{1}{1+x}$ and integrate both sides.

$$\frac{1}{1+x} = \sum_{k=0}^{\infty} (-1)^k x^k \quad \text{for } |x| < 1$$

Integrate both sides from $0$ to $t$:

$$\int_{0}^{t} \frac{1}{1+x} dx = \sum_{k=0}^{\infty} \int_{0}^{t} (-1)^k x^k dx$$

Evaluating the integrals yields the Taylor series for the natural logarithm:

$$\ln(1+t) = \sum_{k=0}^{\infty} \frac{(-1)^k t^{k+1}}{k+1} = \sum_{k=1}^{\infty} \frac{(-1)^{k+1} t^k}{k}$$

### **Question 4**

**Explanation:** Power series can also be **differentiated term-by-term**. To evaluate the specific numerical series, we first find the sum function for $\sum kx^k$ by taking the derivative of the standard geometric series, and then we evaluate it at $x = 1/3$.

$$f(x) = \sum_{k=1}^{\infty} kx^k = x \sum_{k=1}^{\infty} kx^{k-1} = x \frac{d}{dx} \sum_{k=0}^{\infty} x^k$$

$$f(x) = x \frac{d}{dx} \left( \frac{1}{1-x} \right) = \frac{x}{(1-x)^2}$$

Substitute $x = 1/3$ into our resulting closed-form formula:

$$\sum_{k=1}^{\infty} \frac{k}{3^k} = f\left(\frac{1}{3}\right) = \frac{1/3}{(1-1/3)^2} = \frac{3}{4}$$

### **Question 5**

**1. Interval $[0,1]$:**

**Explanation:** Uniform convergence requires pointwise convergence everywhere in the interval. If we check the right endpoint ($x=1$), the series becomes the harmonic series, which diverges. Since it fails to converge at a point in the interval, it cannot converge uniformly.

At $x=1$, $\sum_{k=1}^{\infty} \frac{1^k}{k}$ diverges.

**2. Interval $[0,a], \ 0 < a < 1$:**

**Explanation:** On this restricted interval, the maximum value of $x$ is $a$. We can use the **Weierstrass M-test** by bounding the general term with $a^k$.

$$\forall x \in [0,a], \quad \left| \frac{x^k}{k} \right| \le \frac{a^k}{k} \le a^k$$

Since $0 < a < 1$, $\sum a^k$ is a convergent geometric series:

$$\sum_{k=1}^{\infty} a^k < \infty \implies \sum_{k=1}^{\infty} \frac{x^k}{k} \text{ converges uniformly on } [0,a]$$

### **Question 6**

**Explanation:** A necessary condition for uniform convergence is that the supremum of the general term must approach $0$ as $k \to \infty$. By evaluating the general term at $x=k$, we can show that the supremum does not shrink to zero.

We analyze the limit of the supremum of the general term $f_k(x)$:

$$\lim_{k \to \infty} \sup_{x \in \mathbb{R}} \left| \frac{x^2}{k^2+x^2} \right| \ge \lim_{k \to \infty} \left| \frac{k^2}{k^2+k^2} \right| = \frac{1}{2} \neq 0$$

Because the general term does not uniformly vanish, the series fails the basic divergence test for uniform convergence and does not converge uniformly on $\mathbb{R}$.

### **Question 7**

**Explanation:** Similar to Question 3, we use **term-by-term integration** of the standard geometric series.

Start with the given geometric series:

$$\sum_{k=0}^{\infty} x^k = \frac{1}{1-x} \quad \text{for } |x| < 1$$

Integrate both sides from $0$ to $t$:

$$\int_{0}^{t} \sum_{k=0}^{\infty} x^k dx = \int_{0}^{t} \frac{1}{1-x} dx$$

Evaluating the integrals provides the required sum:

$$\sum_{k=0}^{\infty} \frac{t^{k+1}}{k+1} = -\ln(1-t)$$

### **Question 8**

**Explanation:** We rewrite the term to look like $\sum k u^k$, allowing us to use the formula derived in Question 4. By applying **term-by-term differentiation** on a substituted variable, we find the closed-form sum.

First, recall the formula derived by differentiating the geometric series for a variable $u$:

$$\sum_{k=1}^{\infty} k u^k = u \frac{d}{du} \left( \frac{1}{1-u} \right) = \frac{u}{(1-u)^2}$$

Let $u = x/2$. We substitute this into our original series to find the sum:

$$\sum_{k=1}^{\infty} \frac{kx^k}{2^k} = \sum_{k=1}^{\infty} k \left(\frac{x}{2}\right)^k = \frac{x/2}{(1 - x/2)^2}$$

Multiply the numerator and denominator by $4$ to simplify the fraction:

$$\frac{x/2}{(1 - x/2)^2} = \frac{2x}{(2-x)^2}$$