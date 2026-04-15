![[Pasted image 20260415193515.png]]
$$
\sum ^{\infty}_{n=1} \frac{n^{2026}}{2026^{n}}
$$

  $$
  \lim_{n \to \infty} \left| \frac{a_{n+1}}{a_n} \right| = \lim_{n \to \infty} \frac{(n+1)^{2026}}{2026^{n+1}} \cdot \frac{2026^n}{n^{2026}} = \lim_{n \to \infty} \left( \frac{n+1}{n} \right)^{2026} \cdot \frac{1}{2026} = 1 \cdot \frac{1}{2026}
  $$

**Result:** Since $L = \frac{1}{2026} < 1$, the series **converges**.


---
# 2.
![[Pasted image 20260415195031.png]]
 $$
 \sum_{n=1}^{\infty} \frac{8+(-1)^n}{7^n}
 $$

$$
0 < \frac{7}{7^n} \leq \frac{8+(-1)^n}{7^n} \leq \frac{9}{7^n}
$$
 **Result:** The series $\sum \frac{9}{7^n}$ is a geometric series with $r = \frac{1}{7} < 1$, which converges. By the comparison test, this series **converges**.    

---
# 3.
![[Pasted image 20260415195043.png]]
$$
\sum_{n=1}^{\infty} \frac{2n}{n^2+1}
$$
$$
\lim_{n \to \infty} \frac{\frac{2n}{n^2+1}}{\frac{1}{n}} = \lim_{n \to \infty} \frac{2n^2}{n^2+1} = 2
$$

 **Result:** Since the limit is a positive constant and $\sum \frac{1}{n}$ diverges, this series **diverges**.

---
# 4.
![[Pasted image 20260415195058.png]]
 $$
 \sum_{n=1}^{\infty} \frac{\arctan n}{n^2+1}
 $$
$$
\frac{\arctan n}{n^2+1} < \frac{\pi/2}{n^2}
$$

 **Result:** The series $\sum \frac{1}{n^2}$ is a $p$-series with $p=2 > 1$, which converges. Therefore, this series **converges**.


---
# 5.
![[Pasted image 20260415195121.png]]
$$
\sum_{n=2}^{\infty} \frac{\arctan(2n \ln^2 n)}{n \ln^2 n}
$$

$$
0 < \frac{\arctan(2n \ln^2 n)}{n \ln^2 n} < \frac{\pi/2}{n \ln^2 n}
$$
 **Integration Test / Known Series:** The series $\sum \frac{1}{n \ln^p n}$ converges if $p > 1$. Here $p=2$.
 **Result:** The series **converges**.


---
# 6.
![[Pasted image 20260415195132.png]]
 $$
 \sum_{n=1}^{\infty} \frac{2^n n!}{n^n}
 $$
$$
\lim_{n \to \infty} \frac{a_{n+1}}{a_n} = \frac{2^{n+1} (n+1)!}{(n+1)^{n+1}} \cdot \frac{n^n}{2^n n!} = \frac{2(n+1) \cdot n^n}{(n+1)^{n+1}} = \frac{2 \cdot n^n}{(n+1)^n} = \frac{2}{(1 + \frac{1}{n})^n}
$$

**Limit:** As $n \to \infty$, the denominator approaches $e$. So the limit is $\frac{2}{e}$.
**Result:** Since $e \approx 2.718$, then $L = \frac{2}{e} < 1$. The series **converges**.

---
# 1.
![[Pasted image 20260415200926.png]]

$$\sum_{n=1}^{\infty} \frac{\ln\left(\frac{1}{n^7}+1\right) \cdot \sin(4^n)}{n}$$

$$\left| \frac{\ln\left(\frac{1}{n^7}+1\right) \sin(4^n)}{n} \right| \leq \frac{\ln\left(\frac{1}{n^7}+1\right)}{n} \approx \frac{1}{n^8}$$

**Result:** Since $\sum \frac{1}{n^8}$ is a convergent $p$-series ($p=8 > 1$), the series **converges absolutely**.

---
# 2.
![[Pasted image 20260415201051.png]]
 $$
 \sum_{n=1}^{\infty} (-1)^n \left(\sqrt{n^2 + 1} - n\right)
$$
$$
\sqrt{n^2+1}-n = \frac{(\sqrt{n^2+1}-n)(\sqrt{n^2+1}+n)}{\sqrt{n^2+1}+n} = \frac{1}{\sqrt{n^2+1}+n}
$$
 
1. The sequence $b_n = \frac{1}{\sqrt{n^2+1}+n}$ is clearly positive and decreasing.

2. $\lim_{n \to \infty} b_n = 0$.
 Therefore, the series **converges**.

 **Absolute Convergence?** $\sum \frac{1}{\sqrt{n^2+1}+n}$ behaves like $\sum \frac{1}{2n}$, which diverges (harmonic series).

**Result:** The series **converges conditionally**.

---
# 3.
![[Pasted image 20260415201236.png]]
$$
\sum_{n=1}^{\infty} \frac{\cos(n\pi) \ln(7n^3)}{n}
$$

1. $\lim_{n \to \infty} \frac{\ln 7 + 3\ln n}{n} = 0$ (by L'Hôpital's).
2. The sequence is decreasing for sufficiently large $n$.
**Absolute Convergence?** $\sum \frac{\ln(7n^3)}{n} > \sum \frac{1}{n}$ for $n$ large enough. Since $\sum \frac{1}{n}$ diverges, the absolute series diverges.
**Result:** The series **converges conditionally**.

---
## **3. Proofs**
## 1.
- **Proof:** Use the **AM-GM Inequality** (Arithmetic Mean - Geometric Mean) or the basic inequality $(|a_n| - |b_n|)^2 \geq 0$.

 Expanding the square gives: $a_n^2 - 2|a_n b_n| + b_n^2 \geq 0$, which rearranges to:
$$|a_n b_n| \leq \frac{1}{2}a_n^2 + \frac{1}{2}b_n^2$$

- Since $\sum a_n^2$ and $\sum b_n^2$ converge, their sum (and half their sum) converges. By the **Comparison Test**, $\sum |a_n b_n|$ must also converge.


### **ב. Prove that if $\sum a_n^2$ converges, then $\sum \frac{|a_n|}{n}$ converges.**

- **Proof:** This is a direct application of the proof in 3.א.
    
- Let $b_n = \frac{1}{n}$. We know from 3.א that if $\sum a_n^2$ and $\sum b_n^2$ converge, then $\sum |a_n b_n|$ converges.
    
- In this case, we have $|a_n \cdot b_n| = |a_n \cdot \frac{1}{n}|$.
    
- Wait! $\sum b_n^2 = \sum (\frac{1}{n})^2 = \sum \frac{1}{n^2}$, which is a **convergent** $p$-series ($p=2$).
    
- Since both $\sum a_n^2$ (given) and $\sum \frac{1}{n^2}$ converge, then by the result of 3.א, the series $\sum \frac{|a_n|}{n}$ **converges**.