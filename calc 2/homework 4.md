### **Question 1 Solution**

**The Problem:** Use the Weierstrass M-test to prove that the series

$$\sum_{k=1}^{\infty}x^{k}(1-x)^{k}$$

converges uniformly on the interval $[0,1]$.

**Proof:**

1. **Define the function sequence:**
    
    Let $f_k(x) = x^k(1-x)^k$. We can rewrite this algebraically as:
    
    $$f_k(x) = [x(1-x)]^k$$
    
2. **Find the maximum of the inner function:**
    
    To apply the Weierstrass M-test, we need to find a sequence of positive constants $M_k$ such that $|f_k(x)| \le M_k$ for all $x$ in the interval $[0,1]$, and where the sum $\sum M_k$ converges.
    
    Let's maximize the base of the exponent, $g(x) = x(1-x) = x - x^2$, on the interval $[0,1]$.
    
    To find the critical points, we take the derivative of $g(x)$ and set it to zero:
    
    $$g'(x) = 1 - 2x = 0$$
    
    $$2x = 1$$
    
    $$x = \frac{1}{2}$$
    
3. **Evaluate the maximum value:**
    
    Now, we evaluate $g(x)$ at the critical point and at the boundaries of the interval $[0,1]$ to find the absolute maximum:
    
    - **At $x = 0$:** $g(0) = 0(1-0) = 0$
        
    - **At $x = 1$:** $g(1) = 1(1-1) = 0$
        
    - **At $x = \frac{1}{2}$:** $g\left(\frac{1}{2}\right) = \frac{1}{2}\left(1 - \frac{1}{2}\right) = \frac{1}{4}$
        
    
    The maximum value of $x(1-x)$ on the interval $[0,1]$ is $\frac{1}{4}$.
    
4. **Establish the bound $M_k$:**
    
    Since $0 \le x(1-x) \le \frac{1}{4}$ for all $x \in [0,1]$, we can bound our original function sequence:
    
    $$|f_k(x)| = |x(1-x)|^k \le \left(\frac{1}{4}\right)^k$$
    
    Let $M_k = \left(\frac{1}{4}\right)^k$.
    
5. **Check the convergence of $\sum M_k$:**
    
    We now analyze the numerical series $\sum_{k=1}^{\infty} M_k$:
    
    $$\sum_{k=1}^{\infty} \left(\frac{1}{4}\right)^k$$
    
    This is a standard geometric series with a common ratio $r = \frac{1}{4}$.
    
    Because $|r| < 1$, the geometric series converges.
    

**Conclusion:**

Since $|f_k(x)| \le M_k$ for all $x \in [0,1]$ and the constant series $\sum_{k=1}^{\infty} M_k$ converges, the original series of functions $\sum_{k=1}^{\infty}x^{k}(1-x)^{k}$ converges uniformly on the interval $[0,1]$ by the Weierstrass M-test.

---
