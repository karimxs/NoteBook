# 1
## a.
![[Pasted image 20260325205754.png]]
$$
\sum_{n=1}^\infty \frac{1}{\sqrt{ n } e^{-\sqrt{ n }}}
$$
According to The Direct Comparison Test (First Comparison)
$$
\frac{1}{\sqrt{ n } e^{-\sqrt{ n }}}=\frac{ e^{\sqrt{ n }}}{\sqrt{ n }}> \frac{1}{\sqrt{ n }}
$$
The smaller series $\sum_{n=1}^{\infty} \frac{1}{\sqrt{ n }}$ diverges so the bigger series $\sum_{n=1}^\infty \frac{1}{\sqrt{ n } e^{-\sqrt{ n }}}$ also diverges.

---
## b.
![[Pasted image 20260325211950.png]]
$$
\sum_{k=1}^\infty \frac{\sin ^{2}k}{2^{k}}
$$
According to The Direct Comparison Test (First Comparison)
$$
0\leq \sin ^{2}k\leq 1
$$
$$
\frac{\sin ^{2}k}{2^{k}}\leq\frac{1}{2^{k}}
$$
$$
\sum_{k=1}^\infty \frac{1}{2^k}=\sum_{k=1}^\infty \left( \frac{1}{2} \right)^{k}
$$
$$
\sum_{k=1}^\infty 0.5^{k} \Rightarrow x<1
$$
Therefore the series converges.
The bigger series $\sum_{k=1}^\infty \left( \frac{1}{2} \right)^{k}$ converges so the smaller series $\sum_{k=1}^\infty \frac{\sin ^{2}k}{2^{k}}$ also converges.

---
## c.
![[Pasted image 20260325215011.png]]
$$
\sum _{n=1}^{\infty } \frac{n(n+1)!}{2^{n}}
$$
According to The D'Alembert Test (Ratio Test)
$$
\lim_{ n \to \infty } \left| \frac{a_{n+1}}{a_{n}} \right| 
$$
$$
\lim_{ n \to \infty } \left| \frac{(n+1)(n+2)\cancel!}{2^{\cancel n+1}}\cdot\frac{\cancel{2^{n}}}{n\cancel{(n+1)!}} \right|  
$$
$$
\lim_{ n \to \infty } \left| \frac{(n+1)(n+2)}{2}\cdot\frac{1}{n} \right|  
$$
$$
\lim_{ n \to \infty } \left| \frac{n^2+3n+2}{2n} \right|  
$$$$
\lim_{ n \to \infty } \left| \frac{n}{2}+\frac{3}{2}+\frac{2}{2n} \right|  
\Rightarrow \infty
$$
Therefore the series diverges.

---
## d.
![[Pasted image 20260325220040.png]]
$$
\sum_{k=1}^{\infty} \frac{2+\sin k}{k^{2}+10}
$$
According to The Direct Comparison Test (First Comparison)
$$
1\leq2+\sin k\leq 3
$$
$$
 \frac{2+\sin k}{k^{2}+10} \leq \frac{3}{k^{2}+10}\leq \frac{3}{k^{2}}
$$
$$
\sum_{k=1}^\infty \frac{3}{k^2}=
3\cdot\sum_{k=1}^\infty \frac{1}{k^2}
$$
Therefore the series converges.
The bigger series $\sum_{k=1}^\infty \frac{3}{k^2}$ converges so the smaller series $\sum_{k=1}^{\infty} \frac{2+\sin k}{k^{2}+10}$ also converges.

---
## e.
![[Pasted image 20260325221216.png]]
$$
\sum_{k=1}^\infty \frac{\ln(k)}{k}
$$
$$
\ln(1)=0
$$
$$
\frac{\ln(k)}{k}\geq \frac{1}{k}
$$
According to The Direct Comparison Test (First Comparison)
$$
\sum _{k=1} ^{\infty} \frac{1}{k}
$$
, which we know diverges.
The smaller series $\sum _{k=1} ^{\infty} \frac{1}{k}$ diverges so the bigger series $\sum_{k=1}^\infty \frac{\ln(k)}{k}$ also diverfes.

---
# 2.
![[Pasted image 20260328223010.png]]
# false:

The statement is **False**.

You might be tempted to say it's true because it looks very similar to the Limit Comparison Test. However, there is a crucial detail missing: **the problem does not state that $a_n$ and $b_n$ are positive series.** Because they can be any real numbers, we can use an alternating series to create a counterexample that breaks the rule.

## The Counterexample

Let's define our two sequences:

- $$a_n = \frac{1}{n}$$
    
- $$b_n = \frac{(-1)^n}{\sqrt{n}}$$
    

Now, let's check if they satisfy all the conditions of the problem:

**1. Does $\sum_{n=1}^\infty b_n$ converge?**

Yes. The series $\sum_{n=1}^\infty \frac{(-1)^n}{\sqrt{n}}$ is an alternating series. Since $\frac{1}{\sqrt{n}}$ is positive, decreasing, and its limit as $n \to \infty$ is $0$, the series converges by the **Alternating Series Test (Leibniz Test)**.

**2. Is $\lim_{n \to \infty} \frac{a_n}{b_n} = 0$?**

Let's calculate the limit of the ratio:

$$\lim_{n \to \infty} \frac{a_n}{b_n} = \lim_{n \to \infty} \frac{\frac{1}{n}}{\frac{(-1)^n}{\sqrt{n}}} = \lim_{n \to \infty} \frac{\sqrt{n}}{n \cdot (-1)^n} = \lim_{n \to \infty} \frac{(-1)^n}{\sqrt{n}} = 0$$

The condition is satisfied.

**3. Does $\sum_{n=1}^\infty a_n$ converge?**

No. The series $\sum_{n=1}^\infty \frac{1}{n}$ is the Harmonic Series, which we know **diverges**.

## Summary

We found a case where $b_n$ converges, the limit of their ratio is $0$, but $a_n$ diverges. Therefore, the general statement is false.

_(Note: If the problem had explicitly stated "Let $a_n, b_n > 0$", then the statement would be **True** based on the Limit Comparison Test)._

Would you like to go over why the Limit Comparison Test fails when negative numbers are involved, or should we look at the next exercise?