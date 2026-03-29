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
**False:**

Let's define our two sequences by their odd and even terms (where $k=1,2,3,\dots$):

- $a_{2k-1} = \frac{1}{k}$ and $a_{2k} = \frac{1}{k}$ (This creates the sequence $1, 1, \frac{1}{2}, \frac{1}{2}, \frac{1}{3}, \frac{1}{3}, \dots$)

- $b_{2k-1} = \frac{1}{\sqrt{k}}$ and $b_{2k} = -\frac{1}{\sqrt{k}}$ (This creates the sequence $1, -1, \frac{1}{\sqrt{2}}, -\frac{1}{\sqrt{2}}, \frac{1}{\sqrt{3}}, -\frac{1}{\sqrt{3}}, \dots$)

**1.$\sum_{n=1}^{\infty} b_n$ converge**

The series groups into pairs that exactly cancel each other out:

$$(1-1) + \left(\frac{1}{\sqrt{2}} - \frac{1}{\sqrt{2}}\right) + \dots = 0 + 0 + \dots$$

Because the running total (partial sums) settles exactly at $0$ and the individual terms shrink to $0$ as $k \to \infty$, the series converges.

**2. Is $\lim_{n \to \infty} \frac{a_n}{b_n} = 0$?**

Let's calculate the limit of the ratio by checking the odd and even pairs:

For odd terms:

$$\lim_{k \to \infty} \frac{a_{2k-1}}{b_{2k-1}} = \lim_{k \to \infty} \frac{\frac{1}{k}}{\frac{1}{\sqrt{k}}} = \lim_{k \to \infty} \frac{1}{\sqrt{k}} = 0$$

For even terms:

$$\lim_{k \to \infty} \frac{a_{2k}}{b_{2k}} = \lim_{k \to \infty} \frac{\frac{1}{k}}{-\frac{1}{\sqrt{k}}} = \lim_{k \to \infty} -\frac{1}{\sqrt{k}} = 0$$

Since both the positive and negative ratios go to $0$, the overall limit is $0$. The condition is satisfied.

**3. Does $\sum_{n=1}^{\infty} a_n$ converge?**

No. If we group the series into pairs to add them up, we get:

$$(1+1) + \left(\frac{1}{2} + \frac{1}{2}\right) + \left(\frac{1}{3} + \frac{1}{3}\right) + \dots = 2 + 1 + \frac{2}{3} + \frac{2}{4} + \dots = 2 \cdot \sum_{k=1}^{\infty} \frac{1}{k}$$

This is simply $2$ times the Harmonic Series, which we know diverges.